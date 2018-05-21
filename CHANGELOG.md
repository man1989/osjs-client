# Changelog for osjs-client

## 3.0.0-alpha.24

* Added 'osjs/theme' service

## 3.0.0-alpha.23

* Added proper pathJoin method
* Prevent navigating away when dropping files on desktop
* Added 'showHiddenFiles' option for scandir transform
* Update z-index for loading overlay in window
* Add missing size property to special directory in vfs
* Fixed an issue with parentDirectory() resolve
* Added Application.destroyAll method
* Promise-ified Application#request
* Added proper mount/unmount in filesystem
* Cleaned up some async code
* Don't transform URIs in 'resource()' in application
* Added 'worker()' method for creation in application

## 3.0.0-alpha.22

* Remove 'registerDefault' from Core options

This requires the distribution to manually register base providers.
See 'index.js' in the base repository.

## 3.0.0-alpha.21

* Fixed an issue relating to input form field generation

## 3.0.0-alpha.20

* Added Application#emitAll for event broadcasting
* Improved login screen and customization options

## 3.0.0-alpha.19

* Added npmignore
* Added CHANGELOG

## v3.0.0-alpha.18

* Added a method for getting file icon from stat
* Remove previously registered packages
* Added relaunch of apps from server signal
* Fixed wrong assignment of getApplication in global namespace

## v3.0.0-alpha.17

* Added reconnection of websocket
* Added message handling of internal websocket
* Make sure file iters in VFS follow format
* Use Promise style in VFS

## v3.0.0-alpha.16

* A more functional aproach in VFS

## v3.0.0-alpha.15

* A more functional approach for Auth + Settings

## v3.0.0-alpha.13

* Prevent background scroll on iOS
* Updated boot flow
* Added some error handling for settings loading
* Fixed window buttons for iOS rendering issues
* Correction in default settings configuration

## v3.0.0-alpha.12

* Better default settings handling and configuration
* Added basic support for desktop settings
* Merged MergeServiceProvider into Desktop
* Emit events on settings actions
* Updated provider loading
* Strip some unwanted strings from built URLs
* Better auth flow
* Updated desktop provider exposed methods
* Standalone mode now works
* Separate Login UI from Auth adapter
* Better default Settings & Auth abstraction
* Added Settings adapter configuration.
* Removed an unused variable
* Allow setting Settings handler via bootstrap
* Split up Settings to own provider
* Better load/save in Settings
* Added default settings in Settings
* Export Settings class
* Return entire tree in Settings#get() when no key given
* Updated settings service
* Added some default user settings to the config tree
* Split default config + CoreBase update
* Now using '@osjs/common' module
* Added loading state to login and some UI improvements
* Properly handle authentication errors
* Added support for passing on default provider options
* Fixed some Safari incompabilities

## v3.0.0-alpha.11

* Updated some errors in stylesheets

## v3.0.0-alpha.10

* Renamed npm module to '@osjs/client'
* Added default 'home' mountpoint
* Add same-origin credentials to fetch()
* Moved 'message' event listener
* Updated mountpoint property generation
* Use 'deepmerge' for configs
* Make sure parent dir always ends with slash in resolver
* Update special folder creation in vfs
* Don't emit launch event in packages on singleton block
* Prefix VFS path with mountpoint names
* Added 'defaultPath' config to VFS
* Moved some VFS configuration to core
* Updated hyperapp dependency
* Updated auth login ui building
* Support for specifying what Auth class to use in provider
* Clean up 'running' in package manager whan application is destroyed
* Remove pointer events on iframes in un-focused windows
* Added singleton application support
* Fixed a pid check for message handling
* Update Application::getApplications() usage
* Updated args handling in 'message' sink
* Changed 'data' to 'args' in 'message' event sink
* Accept 'message' on window and route to appropriate proc
* Added 'emit()' for application in getApplications map

## v3.0.0-alpha.9

* Added default favicon
* Use destruct state in notification destructor
* Add proper z-index for notifications
* Added copy() VFS method
* Added proxy for vfs methods
* Fixed exception on theme provider destruct
* Update mountpoint initialization
* Updated exports and some docs
* Updated docs
* Started on VFS transport abstraction
* Implemented writefile() in VFS

## v3.0.0-alpha.8

* Added theme loading
* Updated application categories

## v3.0.0-alpha.7

* Added esdoc config
* Added more exports to index
* Removed DefaultServiceProvider
* Split up 'Desktop' and 'Auth' classes from providers
* Added 'sessionable' attribute to window
* Started on mountpoint/transport handling in FS
* Added some docs to register() method in core
* Added local media query support to windows
* Now using new request() for certain APIs
* Added Core::request() for fetch() wrapping
* Append resize/move result to event emit in behavior
* Moved a preventDefault in window behavior


## v3.0.0-alpha.6

* Updated verbosity of service provider registartion logs
* Prevent NaN in human readable size conversion
* Do not prevent mousedown default on inputs in window beahviour
* Added some cache busting for preloads
* Merged 'PackageServiceProvider' into 'CoreServiceProvider'
* Renamed 'PackageManager' to 'Packages'
* Added esdoc definitions for certain Window stuff
* Updated provider esdoc
* Re-arranged utils namespaces
* Moved utils to a subdirectory
* Updated esdoc
* Documented package metadata
* Application relaunch now also includes window sessions
* Updated esdoc
* Updated some logging
* Added simple debugging tray icon
* Fixed tray destruction
* Added relaunch() to application
* Fix FF issue with text selection
* Added application categories to config
* Added 'osjs/core' provder w/methods
* Added Core::config()
* Properly remove Window when destructed from application
* Added tray handling
* Added creation event in Application
* Changed some package-manager launch event names
* Await (ws) connection before proceeding with startup
* Split up configuration generation in core
* PackageManager now generates URLs via core
* Hide (context)menus when window event is triggered
* EventHandler now accepts comma spearated string or string[] as event names
* Corrected URLs in package.json

## v3.0.0-alpha.5

Initial public release