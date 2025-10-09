pipeline{
  agent {
    label 'slave'
  }

  stages{
    stage('install httpd'){
      steps{
        sh '''sudo yum install httpd -y
        sudo systemctl enable httpd
        sudo systemctl start httpd
        '''
      }
    }
    stage('copy the web file'){
      steps{
        sh 'cp index.html /var/www/html'
      }
    }
  }
}
