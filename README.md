# Useful information for python3

## Some random informations of packages installed via yum or pip3
## Package location installed via 'setup.py' file
```bash
cd .local/lib/python3.X/site-packages/
```

## Suppose you have installed Python3.X in a custom path and you want to use pip3.X, then.....
You have to install pip3.X first if it is not installed
If you are behind proxy, then first set proxy of wget and pip
Set proxy for pip3.X
```bash
export https_proxy=http://username:password@proxy_server:port
export http_proxy=http://username:password@proxy_server:port
```
Install pip3.X for Python3.X
```bash
wget https://bootstrap.pypa.io/get-pip.py
python3.8 get-pip.py
```
Install some package via pip3.X
```bash
/path/to/prefix/python3.X/bin/pip3.X install package_name
```
To get the location of 'package_name'
```bash
/path/to/prefix/python3.X/bin/pip3.X show package_name
```
You will see the location of the package under 'location' category

```bash
cd ~/path/to/prefix/python3.X/lib/python3.X/site-packages
```
/path/to/prefix ----> Custom location of python3.X installed.

## Location of packages installed via yum on CentOS
```bash
rpm -ql package_name
```
then export the directory....
```bash
export package_DIR=/path/to/prefix
```
/path/to/prefix is the path of the package
