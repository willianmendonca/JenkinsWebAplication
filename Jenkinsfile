pipeline {
	agent any

	stages{
		stage('inicial'){
			steps{
				sshagent(credentials: ['jenkinslab']){
					sh'''
						mkdir /home/jenkins/teste
						touch /home/jenkins/teste/sucesso.txt
						echo o teste foi um sucesso >> /home/jenkins/teste/sucesso.txt
					'''
				}
				
				echo 'segundo teste multibranch'
			}
		}
	}
}