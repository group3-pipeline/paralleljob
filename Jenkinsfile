pipeline{
	agent any
	stages{
		stage('First Parallel'){
			parallel{
				stage('1-Pretei Lemo'){
					steps{
						echo "subjob1 running"
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