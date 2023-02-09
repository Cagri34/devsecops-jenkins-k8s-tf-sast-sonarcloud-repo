pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asgbuggywebapp123 -Dsonar.organization=asgbuggywebapp123 -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=6851f9b327c12a2e4b3d87976e2aaf1ec66b62e9' 
			}
        } 
  }
}
