# VARS Docs Redesign — Spec

**Date:** 2026-05-07
**Author:** Brian Schlining

## Goal

Expand the VARS documentation site from a single `index.md` into a structured multi-page reference aimed at external researchers and teams setting up their own VARS instance.

## Audience

External researchers and teams unfamiliar with VARS who need to understand the system and get it running.

## Build Tool

Zensical (replaces MkDocs). `zensical.toml` is the authoritative config. `mkdocs.yml` remains but is no longer the primary build config.

## Page Structure

```
docs/
  index.md            # Overview: what VARS is, key capabilities, links forward
  getting-started.md  # Prerequisites, brief setup summary, link to vars-quickstart-public
  architecture.md     # System layer diagram (Mermaid) + layer descriptions
  services.md         # Backend services reference table
  applications.md     # Client applications reference table
```

## Page Content Spec

### index.md
- Brief, clear description of what VARS/M3 is and what it enables
- Bulleted list of key capabilities (annotation, video asset management, taxonomy, ML, framegrabs, querying)
- Link to Getting Started and Architecture pages

### getting-started.md
- Prerequisites: Docker Engine 20.10+, Docker Compose V2, ~8GB RAM, Bash, network access
- One-paragraph overview of the `varsq` CLI workflow (configure → mkcert → start)
- Link to [vars-quickstart-public](https://github.com/mbari-org/vars-quickstart-public) for full details
- No inline command walkthroughs

### architecture.md
- Prose overview of the four layers
- Mermaid diagram showing: nginx → services → three PostgreSQL databases
- Layer descriptions: Orchestration (`varsq`), Web (nginx reverse proxy + URL routing), Application (microservices), Data (PostgreSQL)

### services.md
- Intro sentence
- Table: Service | Description | GitHub
- All nine services: annosaurus, vampire-squid, oni, panoptes, raziel, charybdis, beholder, skimmer, pythia

### applications.md
- Intro sentence
- Table: Application | Description | GitHub
- All apps: vars-annotation, vars-query, kb-editor (via oni), vars-gridview, mondrian, jsharktopda, Sharktopoda

## zensical.toml Changes

Add nav section:
```toml
[project.nav]
"Home" = "index.md"
"Getting Started" = "getting-started.md"
"Architecture" = "architecture.md"
"Services" = "services.md"
"Applications" = "applications.md"
```

## Out of Scope

- Inline command walkthroughs (defer to vars-quickstart-public)
- API reference documentation
- Internal MBARI-specific deployment details
- Troubleshooting guides
