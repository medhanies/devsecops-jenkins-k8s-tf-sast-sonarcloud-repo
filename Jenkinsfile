pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=medhaniewebapp -Dsonar.organization=medhaniewebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=43c5a913333965f6fef50468b6938edd80c0bdec'
			}
        } 
  }
}
