#GWT Eclipse Plugin
This repository houses the source for the GWT Eclipse Plugin. 

## Thanks to our Sponsors
Sponsors that provide man power and equipment to help get the job done. 

### Google
The Google Cloud Tools team has put a significant amount of effort in helping bring the GWT Eclipse Plugin to market. 

* [Google Cloud Tools](https://cloud.google.com/)

### Sencha
Sencha provides man power to help update the plugin and the build server which automates the build. 

* [Sencha.com](http://sencha.com) 

  [![Sencha](http://cdn.sencha.com/img/gwt-eclipse-plugin-banner.png)](https://www.sencha.com/products/gxt/)


## Quality
* This plugin is Beta Quality. 

## Not Included
* This plugin does not include the [Google Cloud Tools Eclipse](https://github.com/GoogleCloudPlatform/google-cloud-eclipse) features.

## Reference
* [Documentation](http://gwt-plugins.github.io/documentation/)
* [GWT Eclipse Plugin Youtube Playlist](https://www.youtube.com/watch?v=DU7ZQVLR5Zo&list=PLBbgqtDgdc_TqzA-qXrjgTFMC_6DKAQyT)

## Features

* GWT SDK Selection
* GWT Compiler Launcher
* GWT Development Mode with Jetty Launcher (a.k.a DevMode Super Dev Mode)
* GWT Development Mode Launcher (a.k.a CodeServer Super Dev Mode)
* GWT Legacy Development Mode Launcher (a.k.a Classic Dev Mode or OOPHM Dev Mode)
* GWT Java Editor
* GWT UIBinder Editor
* OOPHM for Legacy Dev Mode
* CSS Resources Editor
* Maven integration

### Maven
Supports the two GWT Maven plugins.

* [Mojo GWT Maven Plugin](https://gwt-maven-plugin.github.io/gwt-maven-plugin/)
* [TBroyer GWT Maven Plugin](https://tbroyer.github.io/gwt-maven-plugin/)

## MarketPlace
Install from the Eclipse marketplace.

<a href="http://marketplace.eclipse.org/marketplace-client-intro?mpc_install=3107469" class="drag" title="Drag to your running Eclipse workspace to install GWT Eclipse Plugin"><img class="img-responsive" src="https://marketplace.eclipse.org/sites/all/themes/solstice/public/images/marketplace/btn-install.png" alt="Drag to your running Eclipse workspace to install GWT Eclipse Plugin" /></a>

* [https://marketplace.eclipse.org/content/gwt-eclipse-plugin](https://marketplace.eclipse.org/content/gwt-eclipse-plugin)


## Repository
The Eclipse repositories for this plugin. 

### Production
Release update site. 

* [http://storage.googleapis.com/gwt-eclipse-plugin/v3/release](http://storage.googleapis.com/gwt-eclipse-plugin/v3/release)

### Snapshot
Unstable update site

* [http://storage.googleapis.com/gwt-eclipse-plugin/v3/snapshot](http://storage.googleapis.com/gwt-eclipse-plugin/v3/snapshot)


## Development 

### Importing
Simply use Maven to import all the plugins and modules. 

* Use Eclipse Maven Import and import with recursion. 
* Select all the projects and import. 

### Target Definition
The target defintion build is based off of the Google Cloud Tools. Follow their instructions to build.

### Build
Sencha has provided an internal build agent to build. 
[Sencha Eclipse Build](https://teamcity.sencha.com/viewType.html?buildTypeId=Gxt3_Gwt_GwtEclipsePlugin)

* `mvn clean install`

### Deploy
Google storage write permissions are needed to deploy. 

* `sh ./build-deploy-release.sh` - deploy production version
* `sh ./build-deploy-snapshot.sh` - deploy snapshot version

### Testing
There are a couple of archetypes that are used to test. 

* [Single Module Mojo Archetype](https://github.com/branflake2267/Archetypes/tree/master/archetypes/gwt-test-gwt27)
* [Single Module TBroyer Archetype](https://github.com/branflake2267/Archetypes/tree/master/archetypes/gwt-basic) ([TBroyer GWT Maven Plugin](https://github.com/tbroyer/gwt-maven-plugin))

