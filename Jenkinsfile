@Library('pipeline-shared-library') _
pipeline {
    agent any
    parameters {
        string(name: 'Manu')
    } 
    stages {
        stage('Paso 1') {
            steps {
                parallel(
                  first: {
                    sayHello(params.name)
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
