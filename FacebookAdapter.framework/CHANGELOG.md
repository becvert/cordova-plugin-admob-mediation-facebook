# Facebook Audience Network Mediation Adapter for Google Mobile Ads SDK for iOS

## Version 4.17.0.0
- Changed the version naming system to
  [FAN SDK version].[adapter patch version].
- Updated the minimum required Google Mobile Ads SDK to v7.12.0.
- Added support for native ads.

## Version 1.4.0
- Requires Google Mobile Ads SDK 7.8.0 or higher.
- Requires FAN SDK 4.13.1 or higher.
- Adapter now uses [kFBAdSizeInterstitial] instead of [kFBAdSizeInterstital].
- Enabled bitcode.

## Version 1.2.1
- Fixed a bug where interstitial presented and interstitial leaving application
  callbacks were not properly invoked.

## Version 1.2.0
- Sends callbacks when an ad is presented and dismissed.

## Version 1.1.0
- Added support for full width x 250 format when request is
  for `kGADAdSizeMediumRectangle`.

## Version 1.0.1
- Added support for `kGADAdSizeSmartBanner`.

## Version 1.0.0
- Initial release.
