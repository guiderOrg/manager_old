# Guider Manager
![guider-web-dashboard](https://user-images.githubusercontent.com/15862689/67160178-0024ed80-f389-11e9-9a09-6a8eb96e2785.png)
![guider-web-commandtab](https://user-images.githubusercontent.com/15862689/67160180-03b87480-f389-11e9-8a91-033f74d103dc.png)
### Setting
Set publicPath to the IP of your web server
```shell script
$ vi ./django_vue/vue.config.js
```
This is Example. Change 211.10.52.1 to Your Server`s Public IP!
```js
module.exports = {
  publicPath: 'http://211.10.52.1:8080/', 
  outputDir: "../static",
  ....
}
```

### Install Python Dependencies
It is recommended to use virtualenv.
```shell script
$ pip3 install virtualenv
```
```shell script
$ virtualenv venv 
```
```shell script
$ source ./venv/bin/activate
```
If you don't want to use virtualenv, just run this command.
```sh
$ pip3 install -r requirements.txt
```

### Build Frontend Codes
```sh
$ cd ./django_vue/ && npm install && npm run build && cd ..
```

### Run
Run frontend
```
$ cd ./django_vue/ && npm run serve
```
Run backend
```sh
$ python3 manage.py runserver 0.0.0.0:8000
```
