pipeline {
  agent any
  stages {
    stage('git scm update'){
      steps{
        git url: 'https://github.com/hodae1212/ktinfratest.git', brach: 'master'

      }
    }
    
    stage('dockere build and push') {
      steps {
        sh '''
	sudo docker build -t daisukiii/ktcloudinfra:black .
	#sudo docker push daisukiii/ktinfra:black
	'''
      }
    }

  }

}

