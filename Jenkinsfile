pipeline {
    agent any 
    stages {
        stage ('deployment') {
            steps {
                node ('docker') {
                    sh label:'',script: 'sudo docker login --username kanishkaraju --password kanishka@13'
                    sh label: '',script: 'sudo docker pull kanishkaraju/raju:gol.5'
                    sh label: '',script: 'sudo docker container run -d --name kani18 -p 8065:8080 kanishkaraju/raju:gol.5'
                    sh label: '',script: 'sudo docker exec -it kani18 /bin/bash'
                    sh label: '',script: 'sudo wget http://54.214.53.129:8081/artifactory/docker/gameoflife /usr/local/tomcat/webapps/'
                }
            }
        }
        }
}
    
