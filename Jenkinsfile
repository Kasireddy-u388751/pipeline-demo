pipeline {
    agent any
    environment {
        PATH="\opt\apache-maven-3.8.5/bin:$PATH"
    }
    stages {
        stage('clone') {
            steps {
                // Get some code from a GitHub repository
                git credentialsId: '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', url: 'https://github.com/Kasireddy-u388751/pipeline-demo.git'

                // Run Maven on a Unix agent.
                   sh "mvn -Dmaven.test.failure.ignore=true clean package"
		       rm -r /mnt/x/some/directory/Problem\ 1.0/path
                // To run Maven on a Windows agent, use
                // bat "mvn -Dmaven.test.failure.ignore=true clean package"
            }
        }
	 stage('build') {
            steps {
                // Get some code from a GitHub repository
                // git 'https://github.com/Kasireddy-u388751/pipeline-demo.git'

                // Run Maven on a Unix agent.
                   sh "mvn -Dmaven.test.failure.ignore=true clean package"

                // To run Maven on a Windows agent, use
                // bat "mvn -Dmaven.test.failure.ignore=true clean package"
            }
        }
        stage('install') {
            steps {
                // Get some code from a GitHub repository
                // git 'https://github.com/Kasireddy-u388751/pipeline-demo.git'

                // Run Maven on a Unix agent.
                // sh "mvn -Dmaven.test.failure.ignore=true install"

                // To run Maven on a Windows agent, use
                // bat "mvn -Dmaven.test.failure.ignore=true clean package"
            }
			   
        }
	stage('deploy') {
            steps {
		 	  // deploy adapters: [tomcat7(credentialsId: 'c4180bcd-b1de-4150-a7a8-e74b27c9e656', path: '', url: 'http://65.0.100.114:8090/')], contextPath: 'jof', war: '**/*.war'
                
				
            
			}
			   
        }
		
	}
}
