pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asecurityguruubuggy -Dsonar.organization=asecurityguruubuggy -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=5262af7e9407b5b109e956591b597d638b586a24'
			}
        } 
  }
}
