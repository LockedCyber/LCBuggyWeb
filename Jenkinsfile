pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=lcbuggywebapp -Dsonar.organization=lcbuggywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=f5a37ad206db7ed906ac29d344a0b4f4f8907361'
			}
        } 
  }
}
