# C2PA iOS Example

## Overview

This is an iOS example app "c2pa-cam" based on Apple's Sample Code [AVCam](https://developer.apple.com/documentation/avfoundation/avcam-building-a-camera-app)

It was augmented to demonstrate the usage of [official C2PA iOS SDK](https://github.com/contentauth/c2pa-ios/) to make an iOS application into a [C2PA Claim Generator](https://spec.c2pa.org/specifications/specifications/2.2/specs/C2PA_Specification.html#_technical_overview). You can access documentation and learn more about C2PA and the mobile SDKS on the [C2PA Open Source SDK Documentation Site](https://opensource.contentauthenticity.org/docs/introduction).

## How it works

When a image or video is captured by the camera, the sample app will create, embed and cryptographically sign a minimal C2PA v2.2+ Manifest stating the creation provenenace of the asset.

Please note, that this sample currently uses invalid test keys for its purpose.

## Validation

Validate your signed images and videos with the command line [c2patool](https://github.com/contentauth/c2patool) or use an online validator:

https://verify.contentauthenticity.org
https://check.proofmode.org

Note: If you are using a test certificate, some tools will display "untrusted" or "unknown" for the claim signer identity.

## Author, License

The modifications to Apple's c2pa-cam were authored by

Benjamin Erhart, [Die Netzarchitekten e.U.](https://die.netzarchitekten.com)
for [Guardian Project](https://guardianproject.info) and [Proofmode](https://proofmode.org).

Modifications licensed under [MIT](https://opensource.org/license/mit).

Original code licensed under special [Apple license](LICENSE.txt).
