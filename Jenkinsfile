pipeline {
  agent any
  tools { 
        maven 'Maven_3.9.9'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asgbuggywebappmaher -Dsonar.organization=buggyapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=feefdcd3227abe60cdc401af32cd1d40639e402a'
			}
        } 
  }
}
