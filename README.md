# Certification App

## Dev, Build and Test

## Resources

## Description of Files and Directories

## Issues

## Unlock Packegs
sfdx force:package:create -n Certa -d "Using certification to track certs and courses" -r force-app -t Unlocked -v DevHub
 :Para
-n is the package name. This name is an alias you can use when running subsequent packaging commands.
-r is the directory that contains the contents of the package.
-t is the package type, in this case, unlocked.

    ##update sfdx-json version number 
sfdx force:package:version:create -p Certa -d force-app -k test123 --wait 10 -v DevHub

:paras
-p is the package alias that maps to the package ID (0Ho).
-d is the directory that contains the contents of the package.
-k is the installation key that protects your package from being installed by 
    ##ifSucces
Successfully created the package version [08c46000]. Subscriber Package Version Id: 04t4600
Package Installation URL: https://login.salesforce.com/packaging/installPackage.apexp?p0=04t46000002FHMDAA4
As an alternative, you can use the "sfdx force:package:install" command.

sfdx force:package:install --wait 10 --publishwait 10 --package Certa@1.0.0-1 -k test12 --noprompt
