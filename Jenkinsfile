pipeline {
  agent any

  stages {
    
    stage('Clone') {
      steps {
        git url: 'https://github.com/djhrishikesh2003-design/jenkins-simple-demo.git' ,
          branch: 'main'
      }
    }
    
    stage('Run Script') {
      steps { 
        sh 'chmod +x script.sh'
        sh './script.sh'
      }
    }
  }
}
