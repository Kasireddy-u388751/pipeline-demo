pipeline {
    agent any
    environment {
                PATH= "opt/apache-maven-3.8.5-bin:$PATH"
    }
        stages {
        stage('clone code') {
            steps {
                git credentialsId: 'git-credentials', url: 'https://github.com/Kasireddy-u388751/pipeline-demo.git'
            }
        }
		stage('build code') {
            steps {
                 sh "mvn clean install"
           
	            }
            }
	 }
 }
