pipeline {
  agent {
    label 'maven'
  }

  parameters {
    booleanParam name: 'CLEAN_BEFORE_BUILD', description: 'Limpar o workspace antes de rodar o build' 
  }


  stages {
    stage('Clean') {
      when {
        expression { params.CLEAN_BEFORE_BUILD }
      }

      steps {
        echo 'Stage Clean'
      }
      
    }

    stage('Compile') {
      steps {
        echo 'Stage Compile'
      }
    }

    stage('Test') {
      steps {
        echo 'Stage Test'
      }
    }

  }

}