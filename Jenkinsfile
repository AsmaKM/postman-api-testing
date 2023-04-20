pipeline{
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Building....'
      }
    }
    stage('Test'){
      steps {
        echo 'Testing...'
        bat label: 'API POSTMEN COLLECTION tests', script: 'newman run Postman Collections/api-testing-automation-exc.json -d Postman Collections/data.csv'
      }
    }
    stage('Deploy'){
      steps {
        echo 'Deploying....'
      }
    }
  }
}
