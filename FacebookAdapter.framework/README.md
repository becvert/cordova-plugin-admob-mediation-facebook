# Facebook Audience Network Mediation Adapter for Google Mobile Ads SDK for iOS

## Prerequisites
- Xcode 6.0 or higher
- Deployment target of 6.0 or higher
- Google Mobile Ads SDK 7.12.0 or higher
- FAN SDK 4.13.1 or higher

## Instructions
- Add the Google Mobile Ads SDK. See the
  [quick start guide](https://firebase.google.com/docs/admob/ios/quick-start)
  for detailed instructions on how to integrate the Google Mobile Ads SDK.
- Add or drag the adapter .framework into your Xcode project.
- Add the FAN SDK into your Xcode project. You can find the FAN SDK setup
  guide [here](https://developers.facebook.com/docs/audience-network/ios/native-api).
- Add Facebook to the mediation configuration for your AdMob ad unit.
- Please see the [set up guide](https://support.google.com/admob/answer/3124703)
  for detailed instructions on how to set up mediation.

You can optionally register a `GADFBNetworkExtras` class in the ad request to
configure whether or not the FAN AdChoices icon should be expandable:

<pre><code>GADRequest *request = [GADRequest request];
GADFBNetworkExtras *extras = [[GADFBNetworkExtras alloc] init];
extras.adChoicesExpandable = YES;
[request registerAdNetworkExtras:extras];</code></pre>

You can use the sub-title and social context at ad response callback.
<pre><code>NSString *subTitle = nativeAppInstallAd.extraAssets[GADFBSubtitle];
NSString *socialContext = nativeAppInstallAd.extraAssets[GADFBSocialContext];
</code></pre>

The latest documentation and code samples for the Google Mobile Ads SDK are
available [here](https://firebase.google.com/docs/admob/ios/quick-start).
