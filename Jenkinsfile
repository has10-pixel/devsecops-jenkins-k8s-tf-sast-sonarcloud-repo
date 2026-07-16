pipeline {
  agent any
  tools { 
        maven 'Maven_3.9.9'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asgbuggywebappmaher -Dsonar.organization=buggyapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=437038ad0495c1c2e9179c30656dfe6aa6fc2613'
			}
        } 
  }
}
