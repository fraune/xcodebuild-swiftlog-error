# xcodebuild-swiftlog-error
### Description
There was an error occurring with a Swift package, swift-log, when I was running an iOS CLI Build on Xcode 14.
### GitHub Issue
- https://github.com/apple/swift-log/issues/234
### To replicate error:
```bash
cd AppDemo
xcodebuild -quiet
```
### Output
```bash
2022-09-16 11:29:03.907 xcodebuild[49112:584860] [MT] IDEFileReferenceDebug: [Load] <IDESwiftPackageCore.IDESwiftPackageSpecialFolderFileReference, 0x600000f6d100: name:Docs.docc path:group:Docs.docc> Failed to load container at path: /Users/username/Library/Developer/Xcode/DerivedData/AppDemo-anoodlawrvyhrmetgbxanczinynu/SourcePackages/checkouts/swift-log/Sources/Logging/Docs.docc, Error: Error Domain=com.apple.dt.IDEContainerErrorDomain Code=6 "Cannot open "Docs.docc" as a "Swift Package Folder" because it is already open as a "Folder"." UserInfo={NSLocalizedDescription=Cannot open "Docs.docc" as a "Swift Package Folder" because it is already open as a "Folder".}
```
