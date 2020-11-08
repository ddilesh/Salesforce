pipeline {
  agent any
  stages {
    stage('Development') {
      steps {
        echo 'Development Completed'
      }
    }

    stage('QA ') {
      steps {
        git(url: 'https://github.com/ddilesh/Salesforce', branch: 'master')
      }
    }

    stage('Deployment') {
      steps {
        input(message: 'Manual Approval for Deployment', ok: 'Yes')
        echo 'Deployment Completed'
      }
    }

  }
}