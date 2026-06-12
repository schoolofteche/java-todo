pipeline{
    agent any
    
    tools{
        gradle "gradle"
    }
    stages{
        stage('clone code'){
            steps{
                git branch: "master", url: "https://github.com/schoolofteche/java-todo.git"
            }
        }
        
        stage('build code'){
            steps{
                sh "gradle build"
            }
        }
        stage('test code '){
            steps{
                sh "gradle test"
            }
        }
        stage('deploy code '){
            steps{
                echo 'Deploying to server......'
            }
        }
      
    }
}