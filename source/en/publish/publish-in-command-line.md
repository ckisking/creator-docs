# Publish in command line

Publish project in command line can help us build auto publish step, we can modify command line parameters to reach different goals.

## Command Reference
 - Mac - `/Applications/CocosCreator.app/Contents/MacOS/CocosCreator --path projectPath --build 'platform=android;debug=true'`
 - Windows - `CocosCreator/CocosCreator.exe --path projectPath --build "platform=android;debug=true"`

## Publish Parameters 
 - **path**: Project Path
 - **build**: Pulibsh project Parameters. Will use Build Panel parameters as the default publish parameters. If has specify other parameters, then will use the specified parameters to overlay the default parameters.
   Optional parameters:
   - **excludedModules**: The modules need remove from engine. Engine modules can find from [here](https://github.com/cocos-creator/engine/blob/master/modules.json)
   - **title**: Project title
   - **platform**: Publish platform [web-mobile, web-desktop, android, win32, ios, mac, runtime]
   - **buildPath**: Publish path
   - **startScene**: Start scene uuid
   - **debug**: Whether or not debug mode 
   - **previewWidth**: Web desktop window width
   - **previewHeight**: Web desktop window height
   - **sourceMaps**: Whether or not need add source maps
   - **webOrientation**: Orientation option on web mobile [landscape, portrait, auto]
   
   - **packageName**: Package Name
   - **useDebugKeystore**: Whether or not use debug keystore
   - **keystorePath**: Keystore path
   - **keystorePassword**: Keystore password
   - **keystoreAlias**: Keystore alias
   - **keystoreAliasPassword**: Keystore alias password
   - **orientation**: Orientation on native mobile [portrait, upsideDown, landscapeLeft, landscapeRight]  
      examples:    
    - orientation={"landscapeLeft": true} 
    - orientation={"landscapeLeft": true, "portrait": true}
   - **template**: Template on native platform [default, link, binary]
   - **androidStudio**: Whether or not use android studio to compile android project
   
   - **includeAnySDK**: Whether or not add AnySDK on web platform,
   
   - **autoCompile**: Whether or not auto compile project after publish project. Default is **true**.




