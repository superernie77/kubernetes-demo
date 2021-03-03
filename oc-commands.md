# OpenShift and Minishift commands 

### add OS CLI to class path
```
minishift oc-env
```
Prints command to set path
### Login as admin
```
oc login -u system:admin
```
### Login as other user
```
oc login -u [username] -p [password]
```
### get Token for Rest API
```
oc whoami -t
```

### curl to Rest API
```
curl -k https://[host]:8443/oapi/v1/projects -H "Authorizatiob: Bearer [token]"
```


