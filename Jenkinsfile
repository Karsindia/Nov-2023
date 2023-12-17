pipeline{
agent any
tools {
// Install the Maven version configured as "M3" and add it to the path.
maven "maven1"
}
stages{
stage('checkout'){
steps{
git branch: 'main', url:'https://github.com/Karsindia/Nov-2023.git'
}
}
stage('create binaries'){
steps{
sh "mvn clean install"
}
}
// stage('create docker image'){
// steps{
// sh "docker build -t siddeshg672/devopsapp:latest ."
// sh "docker tag siddeshg672/devopsapp:latest
// sh "docker push siddeshg672/devopsapp:test-deploy_${BUILD_NUMBER}"
}
}
}

