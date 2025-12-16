# C2PA iOS Example

## Overview

This is an iOS example app "c2pa-cam" based on Apple's Sample Code [AVCam](https://developer.apple.com/documentation/avfoundation/avcam-building-a-camera-app)

It was augmented to demonstrate the usage of the [C2PA iOS library](https://github.com/contentauth/c2pa-ios/) to make an iOS application into a [C2PA claim generator](https://spec.c2pa.org/specifications/specifications/2.2/specs/C2PA_Specification.html#_technical_overview). 

<div style={{display: 'none'}}>

For more information about C2PA and the mobile libraries, see the [C2PA open-source SDK documentation site](https://opensource.contentauthenticity.org/docs/introduction).

</div>

## How it works

When a image or video is captured by the camera, the sample app will create, embed, and cryptographically sign a minimal C2PA v2.2+ manifest stating the creation provenance of the asset.

NOTE: This sample currently uses invalid test keys.

## Validation

Validate your signed images and videos with the command line [c2patool](https://github.com/contentauth/c2patool) or use an online validator such as [ACA Inspect](https://inspect.cr) or [ProofCheck](https://check.proofmode.org).

Note: If you are using a test certificate, some tools will display "untrusted" or "unknown" for the claim signer identity.

## Author, License

The modifications to [Apple's AvCam sample](https://developer.apple.com/documentation/avfoundation/avcam-building-a-camera-app) were authored by Benjamin Erhart, [Die Netzarchitekten e.U.](https://die.netzarchitekten.com) for [Guardian Project](https://guardianproject.info) and [Proofmode](https://proofmode.org).

Licensed under [MIT](LICENSE-MIT) and [Apache](LICENSE-APACHE) licenses.

Some components may be licensed under the [Apple license](LICENSE.txt); check the license terms for each file for details.

