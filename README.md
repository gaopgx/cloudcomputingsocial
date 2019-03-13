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
### Installation
This project provides code standards for various programming languages that widely used in Daimler.
### Install
Code standard depends on different code analysis tools listed below. To run the tests of the project, you need to install below static analysis tools using set-env.sh on linux
```
echo "Installing pmd and cpd ..."
cd $HOME
curl -OL https://github.com/pmd/pmd/releases/download/pmd_releases%2F6.4.0/pmd-bin-6.4.0.zip
unzip pmd-bin-6.4.0.zip
cd -
echo "Finished pmd and cpd installation."


echo "Installing NVM and Node ..."
curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.33.11/install.sh | bash
source .bashrc
echo "Installing Node"
nvm install 7.7.0
nvm use 7.7.0
echo "Finished NVM and Node installation."

echo "Installing eslint ..."
npm install babel-eslint eslint -g
echo "Finished eslint installation."

echo "installing tslint ..."
npm install typescript@2.1.5 -g
npm install tslint@5.11.0 -g
npm install tslint-clean-code@0.2.7 -g
echo "Finished tslint installation."

```

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


### Reference
## Licence

