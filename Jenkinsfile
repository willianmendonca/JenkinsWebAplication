pipeline {
	agent jenkinslab

	stages{
		stage('inicial'){
			steps{
				sshagent(credentials: ['jenkinslab']){
					sh'''
						mkdir /home/jenkins/cenoura
						touch /home/jenkins/cenoura/testandooutrabranch_homologacao.txt
					'''
				}
			}
		}
	}
}