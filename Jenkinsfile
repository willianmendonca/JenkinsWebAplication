pipeline {
	agent any

	node('JenkinsLAB02'){
		stages{
			stage('inicial'){
			
				steps{
					sshagent(credentials: ['jenkinslab']){
						sh'''
							mkdir /home/jenkins/testandooutrabranch
							touch /home/jenkins/testandooutrabranch/testandooutrabranch.txt
							echo testando novamente >> /home/jenkins/testandooutrabranch/testandooutrabranch
						'''
					}
				}
			}
		}
	}
}