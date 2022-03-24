# UD-Viz-electron
The [UD-Viz examples](https://github.com/VCityTeam/UD-Viz/tree/master/examples) packaged as an [electron](https://en.wikipedia.org/wiki/Electron_(software_framework)) application.

## How to build
First setup an npm application environment :
```
git clone https://github.com/VCityTeam/UD-Viz-electron.git
cd UD-Viz-electron
npm i
npm run build
npm run make
```

The resulting binary file will be created in the `./out` folder.

## Technical notes
* Tools: [electron-forge vs electron-builder](https://github.com/electron-userland/electron-builder/issues/1193)?
  - they are both tools to build 
  - electron-forge provides in addition a [ultra-minimal](https://github.com/electron-userland/electron-builder/issues/1193#issuecomment-276589056) boilerplate to create electron app (yet electron-forge d boilerplate code)
* Electron apps need to use a webpack bundle to import UD-Viz. Hence the `npm run build` script in the `package.json` file.
