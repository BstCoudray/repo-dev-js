node {
    def app
     stage('Clone-checkout'){
        checkout scm
     }
     stage('Build image'){
        app = docker.build("dev-js/apache")
     }
     stage ('Test'){
        withDockerContainer("dev-js/apache"){ 
            sh "echo 'bonjour ici javascript'" 
            }
            }
}
