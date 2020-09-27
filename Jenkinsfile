node('ec2-slave') {
  try {
	
    stage('Build'){
	sh 'rm -rf rajeshgit'
	sh 'git clone https://github.com/RajeshChouhan21/Jenkins-ec2-docker.git rajeshgit'
	    dir('rajeshgit/'){
	    sh 'pwd'
	    sh 'ls -ltr'
	    sh 'docker build -t webserver .'
	    sh 'docker run -it --rm -d -p 8080:80 --name web webserver'
	    }
	}
    
  } catch(Exception e) {
    throw e
  }
}
