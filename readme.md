# asset.json

A blueprint to create a descriptive json for a static web asset. Originally conceived for describing 3d geometry on the web, it can be extended to any static media (ex.textures, shaders, mocap, photos, videos...) that has re-usable value.


## Usage

The web app hosted in the repo may be used as an online generator at: http://makesites.org/asset-json

Alternatively it can be downloaded locally using bower: 
```
bower install asset.json
```
For the time being there is no certal repository planned as assets are usually consideed proprietery.


## Schema

Main goal of asset.json is to fit in the existing ecosystem of open source software and use existing conventions established by projects like: 

* NPM (package.json)
* Component (component.json)
* Bower (bower.json)

### Attributes

These are the main attributes any asset.json may contain: 

* ***name***: an alphanumeric (preferably lower case) name that can be used as an identifier for an asset
* ***version***: Standard thre number versioning of the asset that can help when upgrading an asset or one of its dependencies
* ***author***: The main creator of an asset
* ***contributors***: Additional information of people that controbuted to the creation of the asset
* ***domains***: The URLs of the hosts that are allowed to use this asset
* ***dependencies***: A list of other assets included as independent compoents
* ***license***: An array of licenses under which the asset is distributed

## Credits 

Maintained by Makis Tracend ( [@tracend](http://github.com/tracend) )

Project initiated after initial discussion at [glTF](https://github.com/KhronosGroup/glTF/issues/54) from the recomendation of Fabrice Robinet ( [@fabrobinet](https://github.com/fabrobinet) )

Distributed through [Makesites.org](http://makesites.org/)

Licensed under the [MIT license](htpp://makesites.org/licenses/MIT)

