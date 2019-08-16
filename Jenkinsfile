pipeline {
    agent any 
    stages {
        stage ('deployment') {
            steps {
                node ('docker') {
                    sh label:'',script: 'sudo docker login --username kanishkaraju --password kanishka@13'
                    sh label: '',script: 'sudo docker pull kanishkaraju/raju:gol.5'
                    sh label: '',script: 'sudo docker container run -d --name kani -p 8082:8080 kanishkaraju/raju:gol.5'
                    sh label: '',script: 'sudo winpty docker exec -it kani bash'
                }
            }
        }
        }
}
    
