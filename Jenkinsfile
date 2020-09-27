node('ec2-slave') {
  try {
	
    stage('Build'){
	sh 'rm -rf rajeshgit'
	sh 'git clone https://github.com/RajeshChouhan21/Jenkins-ec2-docker.git rajeshgit'
	    dir('rajeshgit/'){
	    sh 'pwd'
	    sh 'ls -ltr'
	    }
	}
    
  } catch(Exception e) {
    throw e
  }
}
