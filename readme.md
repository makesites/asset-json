# asset.json

A blueprint to create a descriptive json for a static web asset. Originally conceived for describing 3d geometry on the web, it can be extended to any static media (ex.textures, shaders, mocap, photos, videos...) that have re-usable value.


## Examples

In the examples folder there are few real-world uses of the spec.

* [3D model](./examples/3d.json) A sample of the schema [Construct.js](http://constructjs.org/) uses
* [Video](./examples/video.json) Used in conjunction with the [video-stream](https://github.com/makesites/video-stream) component for displaying multiple resolutions of a video

It's useful to note that the ```sources``` structure is the main area that changes between the different media types. In fact this is by design, allowing any application to define a suitable schema for the asset's sources.


## Usage

The web app hosted in the repo may be used as an online generator at: http://makesites.org/asset-json

Alternatively it can be downloaded locally using bower:
```
bower install asset.json
```
For the time being there is no certal repository planned as assets are usually considered proprietary.


## Schema

Main goal of asset.json is to fit in the existing ecosystem of open source software and use existing conventions established by projects like:

* NPM (package.json)
* Component (component.json)
* Bower (bower.json)


### Attributes

These are the main attributes any asset.json may contain:

* *name*: an alphanumeric (preferably lower case) name that can be used as an identifier
* *version*: Standard thre number versioning of the asset that can help when upgrading an asset or one of its dependencies
* *author*: The main creator of an asset
* *contributors*: Additional information of people that controbuted to the creation of the asset
* *format*: An insight on the specific format of the asset. It may be something generic like _video_ or more specific like _avi_
* *sources*: An array of folder paths or an object with a more detailed file list, defining the asset location(s)
* *domains*: The URLs of the hosts that are allowed to use this asset
* *dependencies*: A list of other assets included as independent components
* *resources*: A list of folders of files that may be related to the asset as raw sources
* *license*: An array of licenses under which the asset is distributed


## Showcase

Featured applications that use the schema:

* [Construct.js](http://constructjs.org/)
* [ComicsGL](http://comicsgl.com/)
* Assetorium


## Trivia

Project initiated after initial discussion at [glTF](https://github.com/KhronosGroup/glTF/issues/54) from the recommendation of Fabrice Robinet ( [@fabrobinet](https://github.com/fabrobinet) )


## Credits

Initiated by Makis Tracend ( [@tracend](http://github.com/tracend) )

Distributed through [Makesites.org](http://makesites.org/)


## License

Released under the [MIT license](htpp://makesites.org/licenses/MIT)
