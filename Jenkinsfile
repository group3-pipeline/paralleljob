pipeline{
	agent any
	stages{
		stage('First Parallel'){
			when {
				branch 'develop'
			}
			parallel{
				stage('1-Pretei Lemo'){
					steps{
						echo "subjob1 running"
						sh 'bash -x /var/lib/jenkins/workspace/group3paralleljob/pretei.sh'
					}
				}
				stage('2-Gerald Agbonye'){
					steps{
						echo "subjob2 running"
					}
				}
			}
		}
		stage('Second Parallel'){
			when{
				branch 'feature'
			}
			parallel{
				stage('1-Odile Domingo'){
					steps{
						echo "subjob3 running"
					}
				}
				stage('2-Benoit Konango-Nyobe'){
					steps{
						echo "subjob4 running"
					}
				}
			}
		}
	}
}