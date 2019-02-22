node {
stage('GIT') {
   git 'https://github.com/g0t4/jenkins2-course-spring-boot.git'
}


stage('Maven clean package') {
   sh 'mvn -f spring-boot-samples/spring-boot-sample-atmosphere/pom.xml clean package'
}
stage('Archive') {
   archiveArtifacts "spring-boot-samples/spring-boot-sample-atmosphere/target/*.jar"
}
}
