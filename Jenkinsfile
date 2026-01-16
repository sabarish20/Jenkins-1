pipeline {
    agent any

    tools {
        // Install the Maven version configured as "M398" and add it to the path.
        maven "M398"
    }

    stages {
        stage("Echo Version"){
            steps {
                sh 'echo Print Maven Version'
                sh 'mvn -version'
            }
        }
        stage('Build') {
            steps {
                // Get some code from a GitHub repository
                // git branch: 'main', changelog: false, poll: false, url: 'https://github.com/sidd-harth/jenkins-hello-world.git'

                // Run Maven Clean Package.
                sh "mvn clean package -DskipTests=true"
            }
        }    
        stage('Unit Test') {
            steps {
                sh "mvn test"
            }
        }
    }
}


            }
        }
        stage('Build') {
            steps {
                // Get some code from a GitHub repository
                // git branch: 'main', changelog: false, poll: false, url: 'https://github.com/sidd-harth/jenkins-hello-world.git'

                // Run Maven Clean Package.
                sh "mvn clean package -DskipTests=true"
            }
        }    
        stage('Unit Test') {
            steps {
                sh "mvn test"
            }
        }
    }
}

