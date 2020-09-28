node('ec2-slave') {
  try {
	
    stage('Build'){
	sh 'rm -rf rajeshgit'
	sh 'git clone https://github.com/RajeshChouhan21/Jenkins-ec2-docker.git rajeshgit'
	    dir('rajeshgit/'){
	    sh 'pwd'
	    sh 'ls -ltr'
	    sh 'docker build -t webserver .'
	    sh 'docker stop web'
	    sh 'docker ps'
	    sh 'docker run -it --rm -d -p 80:80 -v /apps/workspace/log:/var/log/nginx --name web webserver'
	

	    }
	}
    
  } catch(Exception e) {
    throw e
  }
}
