pipeline {
    agent any 
    stages {
        stage ('deployment') {
            steps {
                node ('docker') {
                    sh label:'',script: 'sudo docker login --username kanishkaraju --password kanishka@13'
                    sh label: '',script: 'sudo docker pull kanishkaraju/raju:gol.5'
                    sh label: '',script: 'sudo docker container run -d --name kani4 -p 8099:8080 kanishkaraju/raju:gol.5'
                }
            }
        }
        }
}
    
