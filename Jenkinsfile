pipeline {
  agent any

  stages {
    
    stage('Clone') {
      steps {
        git url: 'https://github.com/djhrishikesh2003-design/jenkins-simple-demo.git',
            branch: 'main'
      }
    }
    
    stage('Run Script') {
      steps { 
        sh 'chmod +x script.sh'
        sh './script.sh'
      }
    }

    stage('Staging') {
      steps {
        sh 'python3 --version'     // optional: verify python installed
        sh 'python3 main.py'       // run your python script
      }
    }
    stage('Staging1') {
      steps {
        sh 'python3 --version'     // optional: verify python installed
        sh 'python3 bin.py'
      }
    }
  }
}
