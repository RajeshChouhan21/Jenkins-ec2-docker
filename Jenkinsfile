node('ec2-slave') {
  try {
	
    stage('Build'){
	sh 'rm -rf rajeshgit'
	sh 'git clone https://github.com/RajeshChouhan21/Jenkins-ec2-docker.git rajeshgit'
	    dir('rajeshgit/'){
	    sh 'pwd'
	    sh 'ls -ltr'
	    sh 'sudo docker build -t webserver .'
	    }
	}
    
  } catch(Exception e) {
    throw e
  }
}
