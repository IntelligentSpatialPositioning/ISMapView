# ISMapView.framework

`ISMapView.framework` is an iOS framework providing a mechanism for displaying an SVG map as a high-quality OpenGL render.

## Downloading the Framework

`ISMapView.framework` can be downloaded in a ZIP file from [here](https://github.com/IntelligentSpatialPositioning/ISMapView/releases/download/initial/ISMapView.framework.zip). 

The framework needs to then be placed in a subdirectory beneath your app.

## Embedding in an iOS Application

Once `ISMapView.framework` has been placed in a subdirectory beneath your app, drag it into your Xcode project; it will show up as a linked framework.

Add the following additional frameworks to your project by clicking on your Target, choosing the "Build Phases" tab, and using the `+` button at the bottom of the "Linked Libraries" section:

* GLKit
* ISMapView

[DemoApp](https://github.com/IntelligentSpatialPositioning/DemoApp) is an example of an iOS application built using `ISMapView.framework`.

### External Dependencies

[JSONKit](https://github.com/johnezang/JSONKit) is required for JSON parsing within the framework.

JSONKit can be downloaded in a ZIP file from [here](https://github.com/johnezang/JSONKit/archive/master.zip). Once you have downloaded and unzipped the ZIP file, you will need to drop JSONKit.h and JSONKit.m in your Xcode project.

JSONKit needs some specific compile flags. To set these do the following;

1. Go to your Xcode project settings, under Build Phases > Compile Sources
2. Select JSONKit and add `-fno-objc-arc -Wno-deprecated-objc-isa-usage` as compiler flags. 

## Support

`ISLocation.framework` is fully supported by Intelligent Spatial Positoning. If you have any questions, comments, or bug reports, please contact us at [support@intelligentspatialpositioning.com](mailto:support@intelligentspatialpositioning.com).
