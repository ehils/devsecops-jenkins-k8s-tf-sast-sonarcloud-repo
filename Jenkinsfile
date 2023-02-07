pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=abuggywebapp -Dsonar.organization=abuggywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=b53fa493b82455e652aab386d23948d3f7fe9072'
			}
        } 
  }
}
