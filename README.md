# Classpip Mobile Application
[![Classpip Badge](https://img.shields.io/badge/classpip-dashboard-brightgreen.svg)](https://github.com/rocmeseguer/classpip-dashboard)
[![Classpip Badge](https://img.shields.io/badge/classpip-mobile-brightgreen.svg)](https://github.com/rocmeseguer/classpip-mobile)
[![Classpip Badge](https://img.shields.io/badge/classpip-services-brightgreen.svg)](https://github.com/rocmeseguer/classpip-services)
[![license](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/classpip/classpip/blob/master/LICENSE)

Classpip is a software architecture for teachers and students to perform school gamification activities inside the school environment through different platforms such as mobiles, tablets and computers.

The software architecture is composed by a mobile application for performing “quick” class activities oriented to teachers and students. For “long” operations such as deep into reports and setup the platform there is an administration dashboard accessible from every computer. These two pieces shares the information through a service-oriented architecture that exposes the main methods for data manipulation.

![classpip-arch](https://github.com/classpip/classpip/raw/master/images/project-architecture.png)

## NodeJS

Make sure you have NodeJS installed. Download the installer or use your favorite package manager. It's best to get the 10x version of node. This offers the best in stability and speed for building.

You may also need development tools to build native addons.

```
node -v
> v10.13.0
```

### To build native addons on Linux (Ubuntu)

```
sudo apt-get install gcc g++ make
```

### To build native addons on Windows

```
npm install -g windows-build-tools
```

## Global dependencies

You have to install Ionic and Cordova tooling for managing the model:
```
npm install -g ionic@4.6.0
npm install -g cordova@8.1.2
```

## Local dependencies

All the project dependencies are manage through [npmjs](https://www.npmjs.com/). This command will also download the typings configured in the **typings.json** file. To install this dependencies you should run:

```
npm install
```

## Development server

For development purposes, you have to restore the cordova state of the application. All the platforms and plugins files are not uploaded into the repo but you could download with the following command:

```
mkdir www
cordova prepare
```

To see all the **HTML5 development** you could run the following command to see with livereload all the changes on the browser. 

```
ionic serve --lab
```

## License

Classpip is released under the [Apache2 License](https://github.com/classpip/classpip-mobile/blob/master/LICENSE).
