pipeline {
  agent any
  tools { 
        maven 'Maven_3_6_3'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=dubcygoat -Dsonar.organization=dubcygoat -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=44a88fd48f3b572c9a2ca39da30ceef635d992ee'
			}
        } 
  }
}
