pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asecurityguru123 -Dsonar.organization=asecurityguru -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=2741321102de44cc00829d6a82668253c626eccd'
			}
        } 
  }
}
