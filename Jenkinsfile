pipeline {
	agent any

	stages{
		stage('inicial'){
			steps{
				sshagent(credentials: ['jenkinslab']){
					sh'''
						mkdir /home/jenkins/teste
						touch /home/jenkins/testandooutrabranch
						echo o teste dessa branch foi um sucesso >> /home/jenkins/teste/testandooutrabranch
					'''
				}
				
				echo 'segundo teste multibranch'
			}
		}
	}
}