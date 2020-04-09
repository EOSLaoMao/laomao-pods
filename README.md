# laomao-pods
Private cocoapods spec repo for laomao team

### create a private spec repo

`
pod repo add laomao-pods git@github.com:EOSLaoMao/laomao-pods.git
`

Then the repo will be installed at: `~/.cocoapods/repos/laomao-pods`

### add your Podspec to the repo

`
pod repo push laomao-pods xxxxx.podspec
`

This command will validate the podspec file, and push the spec file to the repo after validation.

### usage

Add the following line the Podfile:

`
source 'git@github.com:EOSLaoMao/laomao-pods.git'
source 'https://github.com/CocoaPods/Specs.git'
`
Remember, you should put the private source at the head of the public cocoapods repo!
