# AI Tag Remover

AI Tag Remover is a lightweight iOS privacy utility that creates cleaned copies
of selected photos and videos with removable metadata stripped from the output.
Processing is designed to happen locally on the device.

This repository contains a cloud-ready Xcode project package and a Codemagic
workflow for compiling and testing an unsigned iOS Simulator build. The build
artifact can be uploaded to Appetize for browser-based testing without an Apple
Developer Program membership.

## Testing status

The source structure and cloud configuration have been validated on Windows.
The Codemagic workflow performs the first real Xcode compilation and automated
test run on macOS. Do not treat the app as release-ready until that workflow
passes and the photo and video flows are manually verified in Appetize and on a
physical iPhone.

## Important limitation

Removing embedded metadata does not guarantee that a social platform will stop
labeling media as AI-generated. Platforms may use content credentials,
watermarks, account history, or their own detection systems in addition to file
metadata.
