pipeline {

agent any

 tools {



    maven 'maven3.6.3'

    jdk 'jdk11'



 }

stages {
    stage ('Cleaning'){

        steps{

            sh """

            mvn clean

            """

        }



    }



    stage ('Code Compile'){

        steps{

            sh """

            mvn compile

            """

        }



    }

    

     stage ('Run unit test'){

        steps{

            sh """

            mvn test

            """

        }



    }

    stage ('packaging '){

        steps{

            sh """

            mvn package

            """

        }



    }



}

}




