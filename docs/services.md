# Services

VARS is composed of nine backend microservices. All services are deployed via [vars-quickstart-public](https://github.com/mbari-org/vars-quickstart-public) and are accessible through the nginx reverse proxy.

| Service | Description | Repository |
|---------|-------------|------------|
| **annosaurus** | Manages video and image annotations, observations, and associations | [mbari-org/annosaurus](https://github.com/mbari-org/annosaurus) |
| **vampire-squid** | Video asset manager — handles video sequences, metadata, and references | [mbari-org/vampire-squid](https://github.com/mbari-org/vampire-squid) |
| **oni** | Knowledge base server providing consistent names for animals, equipment, and geology; also manages user accounts and preferences | [mbari-org/oni](https://github.com/mbari-org/oni) |
| **panoptes** | Manages framegrab images and their metadata | [mbari-org/panoptes](https://github.com/mbari-org/panoptes) |
| **raziel** | Centralized configuration and API gateway — aggregates service endpoints | [mbari-org/raziel](https://github.com/mbari-org/raziel) |
| **charybdis** | Cross-service query engine for complex data retrieval across annosaurus, vampire-squid, and oni | [mbari-org/charybdis](https://github.com/mbari-org/charybdis) |
| **beholder** | Extracts individual frames from video sources | [mbari-org/beholder](https://github.com/mbari-org/beholder) |
| **skimmer** | Image processing service | [mbari-org/skimmer](https://github.com/mbari-org/skimmer) |
| **pythia** | Applies machine learning models for automated image analysis | [mbari-org/pythia](https://github.com/mbari-org/pythia) |
