pipeline {
  agent any
  tools { 
        maven 'Maven_3_2_5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=trinitechbuggywebapp -Dsonar.organization=trinitechbuggywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=822c0e1ccaf740142b0555e4ddb054de7b2c4712'
			}
        } 
  }
}
