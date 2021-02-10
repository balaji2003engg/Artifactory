# Artifactory

1. Create the account in the Jfrog 
https://jfrog.com

2. Creat the repo in the libs-snapshot-local and libs-release-local in the jfrog account

3. Place the arifacts using the below account and update the your credentials.Pass the version number as paramaeter from Jenkins. BUILD_NUMBER and WORKSPACE are the jenkins environment variables

curl -u chbalaji080186@gmail.com:Ch683212@ -X PUT https://chbalaji080186.jfrog.io/artifactory/libs-snapshot-local/application1/myweb-${version}.${BUILD_NUMBER}.jar -T ${WORKSPACE}build/libs/HelloWorld-0.0.1-SNAPSHOT.war
