# YARN BASIC COMMANDS

## GET VERSION
yarn -v (or --version)

## GET HELP
yarn help

## CREATE PACKAGE.JSON
yarn init
yarn init -y // Use defaults

## SET DEFAULTS
yarn config set init-license ISC

## GET DEFAULTS
yarn config get init-license

## REMOVE DEFAULTS
yarn delete init-license

## INSTALLING LOCAL PACKAGES
yarn add lodash
yarn add moment

## INSTALL FROM PACKAGE.JSON
(add "gulp":"*")
yarn install

## REMOVING MODULES
yarn remove lodash

## INSTALL CERTAIN VERSIONS
yarn add lodash@4.17.3

## FIND OUTDATED VERSIONS
yarn outdated lodash
yarn outdated

## UPGRADE
yarn upgrade lodash
yarn upgrade

## INSTALL GLOBAL MODULE (global must be put right after yarn)
yarn global add nodemon

## FIND ROOT FOLDER
yarn global bin

## REMOVE GLOBAL PACKAGES
yarn global remove nodemon

## LISTING PACKAGES
yarn list
yarn list --depth=0
yarn list --depth=1
yarn list --pattern gulp

## INSTALLING AS DEV DEPENDENCY
yarn add gulp -D or --dev

## REMOVE DEV DEPENDENCY
yarn remove gulp

#VERIFY THAT VERSIONS MATCH LOCK FILE
yarn check

## CREATE YARN.LOCK FILE
yarn import

## ADD SCRIPT
"scripts": {
    "dev": "nodemon index.js"
  },

## RUN SCRIPT
yarn run dev

## GET LICENSES
yarn license

## CREATE GZIP ARCHIVE OF DEPENDENCIES
yarn pack
yarn pack mydep

## LIST GLOBAL CACHE PACKAGES
yarn cache list
yarn cache list --pattern lodash