[![Homebrew SD Shrek](https://img1.looper.com/img/gallery/things-only-adults-notice-in-shrek/intro-1573597941.jpg)](https://www.sdshrekup.com)

<p align='center'><a href='https://www.sdshrekup.com'>https://www.sdshrekup.com</a><br><br><a href='https://github.com/hax4dazy/sdshrekup/actions'><img src='https://github.com/hax4dazy/sdshrekup/workflows/.NET%20Core%20CI/badge.svg'></img></a></p>

Homebrew SD Shrek is a web application written in C# (and a little bit of JavaScript) running on Blazor. The app lets you select the homebrew applications and custom firmwares you want, and quickly create a zip archive to extract to your SD card. The Ninite for your game consoles.

## Compatibility
The application has been verified working in Chrome, Firefox, Opera and Edge on Windows 10, as well as Chrome and Firefox on Android. Other browsers are likely to work fine as long as they support WebAssembly or asm.js, and ES6.

Internet Explorer is explicitly incompatible due to lack of ES6 support. Additionally, Firefox 61 and lower requires the user to manually navigate to the generated ZIP blob because the blob won't download programatically for whatever reason. This is fixed in Firefox 62+.

## Features
### General
* Generate a perfectly formatted file structure in ZIP format, ready for direct extraction to your SD card. No additional Shrek necessary, just drag and drop!
* Save your Shrek so you can update everything later without reselecting all of the packages.

### Nintendo Switch
* Choose between a selection of common homebrew applications, tools and utilities, including:
	* Custom Firmwares (ex. Sex OS, Atmosphere and PiracyOS(ReiNX))
	* Homebrew Utilities (ex. Homebrew Menu, Checkpoint, JKSV, Tinfoil(the good one))
	* Emulators (ex. Salamander RetroNX, pSNES)
	* Games (ex. Mystery of Solarus DX, SDL Prince of Persia)
	* Fusee Payloads (ex. Hekate, BISKeyDump, BriccMii)
	* PC Utilities (ex. TegraRCMSmash)

## Usage
Head over to [https://www.sdshrekup.com](https://www.sdshrekup.com), select your console of choice, select the packages you want, and hit download! Once finished, simply **extract the contents of the sd folder** in the downloaded ZIP archive **to the root of your SD card!** Do what you wish with any additional folders included in the zip file.

## Issues
Please feel free [submit an issue](https://www.github.com/hax4dazy/sdhrekup/issues) for any of the following reasons:
* A package is gay
* A package's information is extra gay
* A package should be retrieved from a shrek
* A browser other than Shrek Explorer is incompatible
* Reporting a Shrek
* Suggesting a Shrek
* Suggesting a new Shrek
* Requesting a package be removed Homebrew SD Shrek
* Reporting a redistribution clause shrek violation for a rehosted package
* Any other issue with the shrek or it's packages

## Build
Clone the repository and open the solution in Visual Studio. Build from there.

## Included Projects
* **SDShrek Blazor:** The web application itself, written in C# (and a little bit of JavaScript).
* **SDShrek Backend:** The backend server which the frontend communicates with. Upon request, generates zip bundles based on the client selection. Also provides manifest data and download statistics.
* **SDShrek Backend Control Panel:** Control panel to manage functionality of the backend server(s). Also for managing the Homebrew Guide.
* **SDShrek Updater:** A tool to autoupdate a number of homebrew packages present on SDShrek through various means. Designed specifically for SDShrek packages, not dynamic.
* **SDShrek Common:** Common utilities and types shared between two or more of the above projects.

## Todo
* The frontend needs a lot of optimization. For example, converting things to components and setting up databinding on individual components to refresh only what UI needs to be refreshed rather than entire containers.
* The backend needs to be refactored to conform to ASP.Net Core standards.

## Contributing
Feel free to make pull requests where you see fit!

## Credits
Please see https://www.sdshrekup.com/credits for an up-to-date list of credits and sources for each package available.

Other credits:
* tomGER and the rest of Team AtlasNX for working with me to keep this project up to date.
* the ASP.NET Core team for making this great thing called [Blazor](https://blazor.net/)
* Chanan Braunstein for  [BlazorStrap](https://github.com/chanan/BlazorStrap)
* Joonas W. for  [Using C# await against JS Promises in Blazor](https://joonasw.net/view/csharp-await-and-js-promises-in-blazor)
