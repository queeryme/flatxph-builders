# DO NOT USE THIS PACKAGE
This is just a sample project to study npm publishing of angular builder projects.
This is forked from the original by @angular-builders/timestamp and any changes to this
code will not reflect the orignal one.

# Timestamp builder for Angular build facade
[![npm version](https://img.shields.io/npm/v/@angular-builders/timestamp.svg) ![npm](https://img.shields.io/npm/dm/@angular-builders/timestamp.svg)](https://www.npmjs.com/package/@angular-builders/timestamp)  

This builder is an example from the Medium article [Angular CLI 6 under the hood — builders demystified](https://medium.com/@meltedspark/angular-cli-6-under-the-hood-builders-demystified-f0690ebcf01).

## Usage

  1. In the root of your Angular application:
        ```
        npm i -D @angular-builders/timestamp
        ```
  2. In your _angular.json_ add the following to _architect_ section of the relevant project:
  
        ```
        "timestamp": {
          "builder": "@angular-builders/timestamp:file",
          "options": {}
        },
        ```
  3. Run: `ng run [relevant-project]:timestamp`
     Where _[relevant-project]_ is the project to which you've added the target 

## Options

 - `path` - path to the file with timestamp, defaults to `./timestamp`
 - `format` - timestamp date format, defaults to `dd/mm/yyyy`
