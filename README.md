# Mule-JAR-deployment
This is the example for mule 4 project JAR deployment using maven plugin.

Configuration required :

1) anypoint cloudhub uri
2) mule version
3) user credentials
4) environment
5) application name
6) worker type
7) workers
properties config like private key (encryption key for secured property encryption)
after adding required maven plugin and cloudhub configuration execute following mvn command to deploy jar on cloudhub

mvn clean deploy -DmuleDeploy -DskipTests -Dmule.version=4.3.0 -Dusername= -Dpassword= -Denv=Sandbox -DencryptKey= -DworkerType=Micro -Dworkers=1

for e.g : mvn clean deploy -DmuleDeploy -DskipTests -Dmule.version=4.3.0 -Dusername=user1 -Dpassword=****** -Denv=Sandbox -DencryptKey=abcxvyrte12893 -DworkerType=Micro -Dworkers=1
