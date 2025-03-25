pipeline {
  agent any
  tools { 
        maven 'Maven_3_2_5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=devsecops-cloudlab_devsecops-cloudlab -Dsonar.organization=devsecops-cloudlab -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=63262f858c46da885de958fba59b3114c93e5e88'
			}
        } 
  }
}
