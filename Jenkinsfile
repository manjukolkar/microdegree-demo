pipeline{
  agent {
    label 'slave'
  }

  stages{
    stage('install httpd'){
      steps{
        sh 'sudo yum install httpd -y'
      }
    }
    stage('copy the web file'){
      steps{
        sh 'cp index.html /var/www/html'
      }
    }
  }
}
