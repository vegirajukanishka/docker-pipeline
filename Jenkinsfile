pipeline {
    agent any 
    stages {
        stage ('deployment') {
            steps {
                node ('docker') {
                    sh label:'',script: 'sudo docker login --username kanishkaraju --password kanishka@13'
                    sh label: '',script: 'sudo docker pull kanishkaraju/raju:gol.5'
                    sh label: '',script: 'sudo docker container run -d --name kani199 -p 8089:8080 kanishkaraju/raju:gol.5'
                    sh label: '',script: 'sudo docker exec -it kani199 /bin/bash'
                }
            }
        }
        }
}
    
