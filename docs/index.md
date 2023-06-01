# MBARI's Video Annotation and Reference System (VARS)

##### Note

This is the start of public documentation for VARS and is currently a work-in-progress. Completed documentation is planned to be completed by the end of 2023.

## About VARS

VARS was originally developed in 2004 to create and manage video annotations on video tape recorded from MBARI's remotely operated vehicles. Since then, VARS has evolved into MBARI's Media Management system (M3), a comprehensive set of applications for managing scientific video and image assets.

## Code Repositories

### Services

At the core of M3/VARS is a suite of web services. These services can be started using the [m3-quickstart](https://github.com/mbari-org/m3-quickstart) project. The individual services are:

- [annosaurus](https://github.com/mbari-org/annosaurus) - A web-service for managing image and video annotations.
- [panoptes](https://github.com/mbari-org/panoptes) - A web-service for managing image archiving.
- [pythia](https://github.com/mbari-org/pythia) - A web-service for automated image analysis using machine learning.
- [raziel](https://github.com/mbari-org/raziel) - A centralized configuration server for VARS.
- [vampire-squid](https://github.com/mbari-org/vampire-squid) - A video asset manager
- [vars-kb-server](https://github.com/mbari-org/vars-kb-server) - A knowlegebase server to provide consistent names for animals, equipment, geology, etc.
- [vars-user-server](https://github.com/mbari-org/vars-user-server) - A web service for access user accounts and preferences.

### Applications

These applications are used for various annotation operations.

- [mondrian](https://github.com/mbari-org/mondrian) - An image annotation application (alpha-release)
- [vars-annotation](https://github.com/mbari-org/vars-annotation) - A video annotation application
  - [Sharktopda](https://github.com/mbari-org/Sharktopoda) - A MacOS video player that integrates with vars-annotation. Allows users to localized annotations using bounding boxes by drawing directly on the video.
  - [jsharktopda] - A cross-platform (MacOS, Windows, Linux) video player that integrates with vars-annotation.
- [vars-gridview](https://github.com/mbari-org/vars-gridview) - A tool for reviewing and correcting VARS localizations in bulk
- [vars-localize](https://github.com/mbari-org/vars-localize) - An tool for adding localizations to images.
