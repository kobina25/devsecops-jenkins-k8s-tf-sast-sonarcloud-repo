pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=Kobinabuggywebapp -Dsonar.organization=Kobinabuggywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=785834a292a94be9ea6a81a4d0a5e1d6c274a85d'
			}
        } 
  }
}
