# Mule-JAR-deployment
This is the example for mule 4 project JAR deployment using maven plugin.

Configuration required :

anypoint cloudhub uri
mule version
user credentials
environment
application name
worker type
workers
properties config like private key (encryption key for secured property encryption)
after adding required maven plugin and cloudhub configuration execute following mvn command to deploy jar on cloudhub

mvn clean deploy -DmuleDeploy -DskipTests -Dmule.version=4.3.0 -Dusername= -Dpassword= -Denv=Sandbox -DencryptKey= -DworkerType=Micro -Dworkers=1

for e.g : mvn clean deploy -DmuleDeploy -DskipTests -Dmule.version=4.3.0 -Dusername=user1 -Dpassword=****** -Denv=Sandbox -DencryptKey=abcxvyrte12893 -DworkerType=Micro -Dworkers=1
