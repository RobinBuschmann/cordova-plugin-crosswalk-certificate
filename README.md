Cordova Plugin Crosswalk Certificate
====================================

[Cordova](http://cordova.apache.org) plugin to enable the use of untrusted (self-signed) SSL Certificates.

This fork is compatible with the [crosswalk web view](https://crosswalk-project.org/) v10.x used with cordova-android v3.6.x
Support for crosswalk v11+ (cordova-android v4.x) will be coming in a different fork -- or this plugin will get a major version bump.

## Install

Install directly from git:
```
cordova plugin add https://github.com/danjarvis/cordova-plugin-crosswalk-certificate
```

Note: this plugin will be published to [NPM](https://cordova.apache.org/announcements/2015/04/21/plugins-release-and-move-to-npm.html) shortly.

## Usage

Activate insecure certificates
```
cordova.plugins.certificates.trustUnsecureCerts(true);
```

Dectivate insecure certificates
```
cordova.plugins.certificates.trustUnsecureCerts(false);
```

## Development

### Running integration tests

execute the `runIntegrationTests.sh` script for a specific platform:

```
PLATFORM='android' ./runIntegrationTests.sh
```

```
PLATFORM='ios' ./runIntegrationTests.sh
```

