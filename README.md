install python 2.6 or 2.7 for your serverside

this project uses argparse to figure out what you type in, please install argparse plugin
```
easy_install argparse
```
# How to use
```
./gitlab-webhook.py -p 9090 git@172.19.1.253:/wei/pandan.git /opt/pandan
```
./gitlab-webhook-pandan.py is a webhook prototype for pandan 

# start
```
./gitlab-webhook-pandan.py git@172.19.1.253:wei/pandan.git /opt/pandan
```
use git clone git@172.19.1.253:wei/gitlabAutoCloneDeploy.git && rm -rf gitlabAutoCloneDeploy/.git to deploy without .git

if you want deploy project without .git message automatically

you should use -d option like
```
./gitlab-webhook-pandan-deploy.py git@172.19.1.253:wei/pandan.git /opt/pandan -d True
```
this option default is "False"

the program will told you how to use those option
```
usage: gitlab-webhook-pandan-deploy.py [-h] [-p 9090] [-d]
                                       repository branch_dir
gitlab-webhook-pandan-deploy.py: error: argument -d/--deploynogit: expected one argument
```
