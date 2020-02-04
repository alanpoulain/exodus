# εxodus
[![Build Status](https://travis-ci.org/Exodus-Privacy/exodus.svg?branch=v1)](https://travis-ci.org/Exodus-Privacy/exodus) [![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/Exodus-Privacy/exodus.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/Exodus-Privacy/exodus/context:python)

**εxodus** is a privacy auditing platform for Android applications. It detects behaviors which can be dangerous for user privacy like ads, tracking, analytics, …

The official instance of εxodus is available [here](https://reports.exodus-privacy.eu.org/).

## Contribute to the identification of trackers

All data about trackers are stored on [ETIP](https://etip.exodus-privacy.eu.org) (εxodus tracker investigation platform).

If you wish to help us identify new trackers, you can request an ETIP account by sending a username and an email address to [etip@exodus-privacy.eu.org](mailto:etip@exodus-privacy.eu.org)

## Getting Started

### Installing

You have 3 different ways of setting up your development environment:

- [Manual](doc/install/manual.md)
- [Docker](doc/install/docker.md)
- [Vagrant](doc/install/vagrant.md) (Deprecated)

### Configuring your locale instance

The following options can be configured in `exodus/exodus/settings/`:

| Setting                             | Description                                  | Default         |
|-------------------------------------|----------------------------------------------|-----------------|
| EX_PAGINATOR_COUNT                  | Number of elements per page                  | 25              |
| TRACKERS_AUTO_UPDATE                | Whether to update automatically trackers     | False           |
| TRACKERS_AUTO_UPDATE_TIME           | Trackers update frequency (in seconds)       | 345600          |
| TRACKERS_AUTO_UPDATE_FROM           | Exodus instance to update trackers from      | <live instance> |
| ANALYSIS_REQUESTS_AUTO_CLEANUP_TIME | Requests cleanup frequency (in seconds)      | 86400           |
| ANALYSIS_REQUESTS_KEEP_DURATION     | Requests keep duration (in days)             | 4               |
| ALLOW_APK_UPLOAD                    | Whether to allow APK file upload             | False           |
| GOOGLE_ACCOUNT_USERNAME             | Username for Google account to download apps | /               |
| GOOGLE_ACCOUNT_PASSWORD             | Password for Google account to download apps | /               |

### Analyzing an application

Browse to [the analysis submission page](http://127.0.0.1:8000/analysis/submit/) and start a new analysis (ex: `fr.meteo`).
When the analysis is finished, compare the results with the same report from [the official instance](https://reports.exodus-privacy.eu.org).

### FAQ

Check the [FAQ](doc/faq.md) if you encounter any problem or need an extended documentation about εxodus.

## API documentation

You can find the εxodus API documentation [here](doc/api.md).

## License

This project is licensed under the GNU AGPL v3 License - see the [LICENSE](LICENSE) file for details.
