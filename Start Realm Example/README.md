#Install Realm

```
pod repo update
```
```
pod init
```
```
vi Podfile
```

###Edit Podfile
```
# Uncomment the next line to define a global platform for your project
# platform :ios, '9.0'

target 'Start Realm Example' do
  # Comment the next line if you're not using Swift and don't want to use dynamic frameworks
  use_frameworks!
  pod 'RealmSwift'

  # Pods for Start Realm Example

end
```

```
Pod install
```

###After Pod install
- ```use projectName.xcworkspace``` for this project


### Install Realm Plug-In
- install the plugin manually by opening plugin/RealmPlugin.xcodeproj contained in the [release zip](https://static.realm.io/downloads/swift/realm-swift-2.4.2.zip) and clicking build. 

####Ref
https://realm.io/docs/swift/2.3.0/#xcode-plugin

https://realm.io/kr/news/realm-swift-mobile-database/
