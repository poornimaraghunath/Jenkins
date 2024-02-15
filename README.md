# Jenkins

Jenkins build

In jenkins for building frontend applications that were developed using javascript will use build tools like npm ,yarn

For bulding applications will use maven,gradle for applications built using java

# What is jenkinsfile ?
   it is a concept of pipeline as code it is a scripted pipeline in a repository

Intially Jenkins pipeline was started with the # groovy scripting which has the advanced scripting capabilities but difficult to start.

Structure :

  node {
    // groovy scripting
  }


laterally declartive syntax was started it has pre-defined structure


structure :

pipeline {

    agent any

    stages {

        stage("build") {

            steps 
        }


    }
}


# Once the pipeline job is excecuted there is another attribute that needs to be executed 

Post
  # it has three conditions

   1. always : what ever the result of the job it should always execute
   2. success : if the pipeline is success then execute the block present inside this
   3. Failure : if the pipeline is failure then execute the block present inside this.

  pipeline {

    agent any

    stages {

        stage("build") {

            steps 
        }


    }

    post {
       always{
        //
       } 

       success{
        //
       }


    }
}  