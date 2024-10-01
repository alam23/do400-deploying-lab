pipeline{
    agent{
        node { label "maven" }
    }
    stages{
        stage("Prepare") {
            steps {
                sh "chmod +x mvnw"
            }
        }
        stage("Tests"){
            steps{
                sh "./mvnw verify"
            }
        }
    }
}