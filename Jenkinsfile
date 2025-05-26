
pipeline {
    agent any
    stages {
        stage('Build & Deploy') {
            steps {
                bat '''
                    git clone https://github.com/abprakash405/war-web-project.git
                    cd war-web-project
                    mvn clean package
                    copy target\\*.war "C:\\Program Files\\Apache Software Foundation\\Tomcat 10.1\\webapps"
                    echo " script completed"
                '''
            }
        }
        stage('test') {
            steps {
                bat '''
                    echo " testing the pipeline"
                '''
            }
        }
        stage('verify') {
            steps {
                bat '''
                    echo " veritying the pipeline"
                '''
            }
        }
        
    }
}
