pipeline {
  agent any
  tools { 
        maven 'Maven_3_2_5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=devsecops-cloudlab_devsecops-cloudlab -Dsonar.organization=devsecops-cloudlab -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=6acdfbf92392bd2716283012edccc951e6c08d1e'
			}
        } 
  }
}
