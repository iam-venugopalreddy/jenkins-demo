pipeline {
    agent any
    environment {
        dockerHome = tool "myDocker" //myDocker is given name by me when i added docker tool
        mavenHome = tool "myMaven"
        PATH = "$dockerHome/bin:$mavenHome/bin:$PATH"
    }
    stages {
        stage("Chekout") {
            steps {
                echo "checkout success"
            }
        }
        stage("Build") {
            steps {
                echo "This is Build stage"
                echo "Build_id - $env.BUILD_ID"
                echo "Build_name - $env.BUILD_NAME"
                echo "Build_tag - $env.BUILD_TAG"
                echo "PATH = $env.PATH"

            }
        }
    }
}
