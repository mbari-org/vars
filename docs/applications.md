# Applications

VARS includes several client applications for annotation, querying, and knowledge base management. All clients authenticate via JWT tokens through the nginx proxy.

| Application | Platform | Description | Repository |
|-------------|----------|-------------|------------|
| **vars-annotation** | Desktop (Java) | Primary video annotation application with timeline-based interface | [mbari-org/vars-annotation](https://github.com/mbari-org/vars-annotation) |
| **vars-query** | Web (Vue 3) | Search and retrieval interface for annotation data | [mbari-org/vars-query-vue](https://github.com/mbari-org/vars-query-vue) |
| **kb-editor** | Web (React) | Knowledge base editing tool for managing taxonomic concepts | [mbari-org/kb](https://github.com/mbari-org/kb) |
| **vars-gridview** | Desktop | Bulk editing tool for reviewing and correcting VARS localizations and bounding boxes | [mbari-org/vars-gridview](https://github.com/mbari-org/vars-gridview) |
| **vars-localize** | Desktop | Tool for creating localizations within the VARS database | [mbari-org/vars-localize](https://github.com/mbari-org/vars-localize)
| **mondrian** | Desktop | Image annotation application (alpha release) | [mbari-org/mondrian](https://github.com/mbari-org/mondrian) |
| **Sharktopoda** | macOS | Video player that integrates with vars-annotation, supporting bounding box localization directly on video | [mbari-org/Sharktopoda](https://github.com/mbari-org/Sharktopoda) |
| **jsharktopoda** | Cross-platform | Cross-platform (macOS, Windows, Linux) video player with vars-annotation integration | [mbari-org/jsharktopoda](https://github.com/mbari-org/jsharktopoda) |
