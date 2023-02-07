pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=abuggywebapp -Dsonar.organization=abuggywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=fc0b34a7257c68be81f9054daad08cfb4ea35f54'
			}
        } 
  }
}
