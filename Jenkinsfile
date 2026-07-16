pipeline {
  agent any
  tools { 
        maven 'Maven_3.9.9'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asgbuggywebappmaher -Dsonar.organization=asgbuggywebappmaher -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=7c7240c83754c5f42dd1df72abf7044333557f1d'
			}
        } 
  }
}
