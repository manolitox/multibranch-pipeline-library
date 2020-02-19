@Library('pipeline-shared-library') _
pipeline {
    agent any 
    stages {
        stage('Paso 1') {
            steps {
                parallel(
                  first: {
                    sayHello(params.NAME)
                    sleep 2
                  },
                  second: {
                    sayHello(params.NAME)
                    sleep 2
                  }
                )
            }
        }
    }
}
