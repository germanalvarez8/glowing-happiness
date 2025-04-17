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
                sh 'git clone https://github.com/germanalvarez8/glowing-happiness.git'
                dir('glowing-happiness') {  // Cambia al directorio del repo
                    sh 'python3 myscript.py'
                }
            }
        }
        stage('Exec script') {
            steps {
                echo 'Ejecutando ejecucion de script'
            }
        }
    }
}