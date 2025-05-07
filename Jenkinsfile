pipeline {
  agent any
  tools { 
        maven 'Maven 3.2.5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=testabhi_buggyapp -Dsonar.organization=testabhi -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=b3e6a98879e0e4b156ca97ec21bbe198c2980368'
			}
        } 
  }
}
