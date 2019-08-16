pipeline {
    agent any 
    stages {
        stage ('deployment') {
            steps {
                node ('docker') {
                    sh label:'',script: 'sudo docker login --username kanishkaraju --password kanishka@13'
                    sh label: '',script: 'sudo docker pull kanishkaraju/raju:gol.4'
                    sh label: '',script: 'sudo docker container run -d --name kanishka -p 8086:8080 gol.4'
                }
            }
        }
        }
}
    
