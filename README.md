# Code-standard
#### A static analysis tool for multiple development languages
This project provides code standards for various programming languages that widely used in Daimler.
#### Rev 1 features
Static Analysis tools by language
* Java
* JavaScript
* golang
* TypeScript
## Introduction and usage
### Introduction
This project provides code standards for various programming languages that widely used in Daimler.
### Install


### Usage
```
# check java project
python ./src/see.py --action checkstyle --basepath ~/daimler-git/china/its/cd/otr/account-management --language java --ignoredir use,comma,split,your,path,exclude
# check javascript react-native project
python ./src/see.py --basepath ~/daimler-git/china/its/cd/otr/dms-helper-frontend --language js --platform react-native --action checkstyle --ignoredir test,tests,target,build,dist,node_modules,i18n,metronic*,dwz*,Microsoft*.js,jquery*,jquery*.js,*.min.js,*-min.js,assets,dms-helper,swagger,miniui,angular*,SiteAssets/JS/sp.js,sp*.js,FrogTMS/FrogTMS.WebUI/obj,layui,Plugins,*spec.js
# check javascript project
python ./src/see.py --basepath ~/daimler-git/china/its/cd/otr/dms-helper-frontend --language js --action checkstyle --ignoredir test,tests,target,build,dist,node_modules,i18n,metronic*,dwz*,Microsoft*.js,jquery*,jquery*.js,*.min.js,*-min.js,assets,dms-helper,swagger,miniui,angular*,SiteAssets/JS/sp.js,sp*.js,FrogTMS/FrogTMS.WebUI/obj,layui,Plugins,*spec.js
# check typescript project
python3 ./src/see.py --action checkstyle --basepath ~/daimler-git/china/its/cd/otr/website/src/**/*.ts --language typescript

```

### Command line options
```
usage: see.py [-h] [--action ACTION] [--notified] [--language LANGUAGE]
              [--platform PLATFORM] [--basepath BASEPATH]
              [--ignoredir IGNOREDIR] [--hub_username USERNAME]
              [--hub_password PASSWORD] [--name NAME] [--version VERSION]
              [--path PATH] [--cov_url COV_URL] [--cov_username COV_USERNAME]
              [--cov_password COV_PASSWORD] [--stream_name COV_STREAM_NAME]

```
### Examples of usage
![example of java static analysis](https://github.com/gaopgx/cloudcomputingsocial/blob/master/example-of-code.PNG?raw=true)

### Test code quaility for code-standard

#### coverage
run the coverage.sh for code coverage
The minimum requirment is 90
##todo



#### CheckStyle
run the CheckStyle for static analysis code quaility of code-standard
##todo
### Future Job
coverity
blackduck
more language support
csharp, python ....

### Reference


## Licence


