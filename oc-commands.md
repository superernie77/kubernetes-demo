# OpenShift and Minishift commands 

### add OS CLI to class path
```
minishift oc-env
```
Prints command to set path
### Login as admin
No password needed if minishift env is used.
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
### List Projects
```
oc get projects
```

### List Users
```
oc get users
```
### Add cluster admin role to users
```
oc adm policy add-cluster-role-to-user cluster-admin [username]
```

