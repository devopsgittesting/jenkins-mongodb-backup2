pipeline {
    agent any
    stages {
        stage('execute') {
            steps {
		script {
			echo 'Using remote command over ssh'
			sh 'echo "Today is:" date'
			echo '*** Executing remote commands ***'
	 		sh '''#!/bin/bash
				date
				ssh root@192.168.0.108 >> ENDSSH
				j
			    	date
			    	cd /tmp
			    	pwd
ENDSSH


                }
            }
        }
    }
}
