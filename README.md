# PEPK - Export Encrypted Private Key Tool

## Usage

Use the command below to run the tool, which will export and encrypt your private key and its public certificate. Ensure that you replace the arguments highlighted in bold. Then enter your store and key passwords when prompted.

```
java -jar pepk.jar --keystore=foo.keystore --alias=foo --output=output.zip --encryptionkey=xxx --include-cert
```

## Development

```
./gradlew run --args='--keystore=foo.keystore --alias=foo --output=output.zip --encryptionkey=xxx --include-cert'
```

or

```
./gradlew shadowJar
java -jar build/libs/pepk.jar --keystore=foo.keystore --alias=foo --output=output.zip --encryptionkey=xxx --include-cert
```

## Deployment

```
./gradlew shadowJar
```

Upload build/libs/pepk.jar into [releases](releases)

## Installation

Download pepk.jar from [releases](releases)

## Build

```
./gradlew assemble
```

## Changelogs

Latest known pepk.jar/build-data.properties:

```
build.target=blaze-out/k8-opt/bin/third_party/java/pepk/ExportEncryptedPrivateKeyTool_deploy.jar
main.class=com.google.wireless.android.vending.developer.signing.tools.extern.export.ExportEncryptedPrivateKeyTool
build.gplatform=gcc-4.X.Y-crosstool-v18-llvm-grtev4-k8
build.depot.path=//depot/branches/play-apps-publisher-app-signing-encryption-tool_release_branch/229150960.1/google3
build.client_mint_status=1
build.client=build-secure-info\:source-uri
build.verifiable=1
build.location=play-apps-publisher-releaser@iojf11.prod.google.com\:/google/src/files/229167424/depot/branches/play-apps-publisher-app-signing-encryption-tool_release_branch/229150960.1/OVERLAY_READONLY/google3
build.tool=Blaze, release blaze-2018.12.11-3 (mainline @224801075)
build.label=play-apps-publisher-app-signing-encryption-tool_20190114_RC00
build.timestamp.as.int=1547473306
build.versionmap=map 0 { // }
build.changelist.as.int=229167424
build.baseline.changelist.as.int=229150960
build.timestamp=1547473306
build.build_id=1221793a-c127-4962-815a-1f6b61ad2cca
build.changelist=229167424
build.time=Mon Jan 14 05\:41\:46 2019 (1547473306)
build.citc.snapshot=-1
```

## License

Android 2.0 - Google Inc, 2017
