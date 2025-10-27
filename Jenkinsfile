pipeline {
  agent any
  tools { 
        maven 'Maven_3_8_4'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asamba -Dsonar.organization=Asamba -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=c0461eff7944646e45f916f95741acfacf41ff02'
			}
        } 
  }
}
