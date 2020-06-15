# core-config-as-code
Master config bundles for Core CasC

### Export example YAML files
Export YAML files from an existing master by adding `core-casc-export` to URL

### Load these configs on OC via a freestyle job like this:
```
rm -rf core-config-as-code/
rm -rf $JENKINS_HOME/jcasc-bundles-store/*
 
git clone https://github.com/BillGarrett/core-config-as-code
cd core-config-as-code
mv * $JENKINS_HOME/jcasc-bundles-store/
```
Note, freestyle job is necessary because OC doesn't support pipeline jobs.
