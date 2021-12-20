pipeline {
	agent any

	stages{
		stage('inicial'){
			steps{
				sshagent(credentials: ['jenkinslab']){
					sh'''
						mkdir /home/jenkins/testandooutrabranch
						touch /home/jenkins/testandooutrabranch/testandooutrabranch.txt
						echo o teste dessa branch foi um sucesso >> /home/jenkins/testandooutrabranch/testandooutrabranch
					'''
				}
			}
		}
	}
}