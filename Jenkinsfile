pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=security-app -Dsonar.organization=securityapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=6c505c594c46b901fea1d16adc2cc6da1fab003d'
			}
        } 
  }
}
