# iOS StartKit with Jenkins and FastLane

## Installation

Make sure you have the latest version of the Xcode command line tools installed:

```bash
xcode-select --install
```

Install _fastlane_:

```bash
[sudo] gem install fastlane -NV
```

or alternatively:

```bash
brew cask install fastlane
```

## Available Actions

### iOS

#### ios custom_lane

```bash
bundle exec fastlane ios custom_lane
```

## Available Actions

### iOS

#### ios test: Run all tests

```bash
bundle exec fastlane ios test
```

#### ios beta: Submit a new Beta Build to Apple TestFlight

```bash
bundle exec fastlane ios beta
```

This will also make sure the profile is up to date.

#### ios release: Deploy a new version to the App Store

```bash
bundle exec fastlane ios release
```

----

This README.md is auto-generated and will be re-generated every time [fastlane](https://fastlane.tools) is run.

More information about fastlane can be found on [fastlane.tools](https://fastlane.tools).
The documentation of fastlane can be found on [docs.fastlane.tools](https://docs.fastlane.tools).