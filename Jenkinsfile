pipeline {
    agent any
    stages {
        stage('First step') {
            steps {
                echo 'Ejecutando first step'
            }
        }
        stage('Clone repo') {
            steps {
                echo 'Ejecutando Clone repo'
                sh 'rm -rf glowing-happiness'
                sh 'https://github.com/germanalvarez8/glowing-happiness.git'
                sh 'cd glowing-happiness'
                sh 'python3 myscript.py'
            }
        }
        stage('Exec script') {
            steps {
                echo 'Ejecutando ejecucion de script'
            }
        }
    }
}