pipeline {
    agent any
    tools {
    maven 'mavenhome'
  }
    stages {
       stage('Checkout ') {
    steps {
        git branch: 'master',
            url: 'https://github.com/mupparajuvamsi/awsprojectdemo.git'

       
    }
}
        stage('Build') {
      steps {
          dir('mavewebappdemo'){
           sh 'mvn -B -DskipTests clean package'
          }
       
      }
    }
    }
    
}
