# Changelog

## Unreleases
- Applied v2.4.2 changes @alangecker

## Release v2.4.0 (2021-12-29)
- BigBlueButton v2.4 @alangecker [#159](https://github.com/bigbluebutton/docker/pull/159)
- **Breaking change:** change nginx port from `8080` to `48087`. see [upgrade note](docs/upgrading.md) @alangeker [#133](https://github.com/bigbluebutton/docker/issues/133)
- Enable optimization for Prometheus Exporter when recording is enabled @omidmaldar [#161](https://github.com/bigbluebutton/docker/pull/161)
- Automatically remove old recordings after N days @omidmaldar [#162](https://github.com/bigbluebutton/docker/pull/162)


## Release v2.3.14-1 (2021-10-06)
- Applied changes v2.3.5-v2.3.14 @alangecker
- updated wget to not use proxies [#143](https://github.com/bigbluebutton/docker/pull/143) @mghadam
- fixed sed delimiter for CERTPATH and KEYPATH [#144](https://github.com/bigbluebutton/docker/pull/144) @mghadam
- https_proxy: fix setting of ALLOWED_DOMAINS [#145](https://github.com/bigbluebutton/docker/pull/145) @clandmeter
- coturn: expose ENABLE_HTTPS_PROXY env variable [#146](https://github.com/bigbluebutton/docker/pull/146) [#156](https://github.com/bigbluebutton/docker/pull/156) @clandmeter @omidmaldar

## Release v2.3.4-1 (2021-06-22) #131
- Applied v2.3.4 changes [#130](https://github.com/bigbluebutton/docker/pull/130) @alangecker 
- Reintegrate turn with default ports and support for external certificates [#126](https://github.com/bigbluebutton/docker/pull/126) @cjhille
- Fix freeswitch package names for languages with uppercase characters in the path  [#119](https://github.com/bigbluebutton/docker/pull/119) @lexuzieel
- Exclude CLIENT_TITLE when generating compose file [#118](https://github.com/bigbluebutton/docker/pull/118) @bb
- Fix for preuploaded presentations not working [#116](https://github.com/bigbluebutton/docker/pull/116) @manfred-w
- Add POSTGRESQL_SECRET as environement variable [#111](https://github.com/bigbluebutton/docker/pull/111) @caminsha


## Release v2.3.0
- :tada: **BigBlueButton 2.3** including all its changes
- Template based generation of docker-compose.yml [2.2.x#71](https://github.com/alangecker/bigbluebutton-docker/pull/71) [2.2.x#42](https://github.com/alangecker/bigbluebutton-docker/issues/42) @trickert76 @alangecker
- Removal of `core` and all dependencies on the bigbluebutton ubuntu repository. Seperate container for `bbb-web`, `fsesl-akka` and `apps-akka` [2.2.x#26](https://github.com/alangecker/bigbluebutton-docker/issues/26) @alangecker
- Fix recordings for Moodle BBB plugin: [2.2.x#110](https://github.com/alangecker/bigbluebutton-docker/pull/110) @danjesus
- Fixed recordings container restart setting [2.2.x#109](https://github.com/alangecker/bigbluebutton-docker/pull/109) @manfred-w
- Option for freeswitch language [2.2.x#85](https://github.com/alangecker/bigbluebutton-docker/pull/85) @alangecker @Daedalus3 
- Disabled integrated coturn [#73](https://github.com/bigbluebutton/docker/issues/73)

## Release v2.2.31-1 (2020-12-23) #84
- Applied v2.2.31 changes @alangecker
- Fix when presentation after recording unable to delete and change access rights #82 #63 @cardinalit
- Enable cameraQualityThresholds by default

## Release v2.2.30-1 (2020-12-01) #79
- Applied v2.2.30 changes @alangecker
- Applied v2.2.29 changes @alangecker
- Fix bug due to unnecessary port forward #81 @trickert76 @alangecker

## Release v2.2.28-1 (2020-10-22) #67
- Applied v2.2.28 changes @alangecker
- Etherpad skin & plugin #69 @alangecker
- Updated `development.md` docs (example config & note about issue #66) @alangecker
- Allow setting the breakout room limit @alangecker

## Release v2.2.27-2 (2020-10-16)
- Increase proxy timeout to avoid aborting websocket connections @alangecker
- Added a changelog

## Release v2.2.27-1 (2020-10-14)
- Applied BBB v2.2.27 changes https://github.com/bigbluebutton/bigbluebutton/releases/tag/v2.2.27 @alangecker
- Upgrade docker base images (etherpad and bigbluebutton-exporter) @alangecker

## Release v2.2.26-1 (2020-09-29)
- Applied changes from BBB v2.2.24 to v2.2.26 #58 #60 @alangecker

## Release v2.2.23-1 (2020-09-06)
- :tada: Recording #16 by @artemtech and @alangecker 
- v2.2.23 changes by @alangecker 
- sip_profile extension field #54 by @yksflip
- Remove greenlight container name #49 by @alangecker 

## Hotfix (2020-08-15)
- Allow imagemagick to convert to pdf/svg #51 #52 @alangecker

## Release v2.2.22-1 (2020-08-12) #50
- v2.2.22 changes by @alangecker 
- Disable freeswitch logfiles inside containers

## Release v2.2.21-1 (2020-7-18)
- Changes for v2.2.21 #44 @alangecker
- expose more BBB settings in .env file #34 @cjhille
- IPv6 Support #32 @alangecker
- Development Mode & Instructions #39 @alangecker
- Prometheus Exporter Integration #40 @alangecker
