pipeline {
    agent any
    tools{
    maven ' Maven 3.8.6 '
    jdk 'jdk 1.8.0'}
    
   //  parameters{
     //   choice(name: 'VERSION', choices:['1.1.0','1.2.0','1.3.0'], description: '')
       // booleanParam(name: 'executeTests', defaultValue: true, description: '')
    //}
    stages {
        stage('Build') {
            steps {
                sh 'mvn clean package'
            }
        }
    
   
        stage('Test') {
           // when {
             //   expression{
               //     params.executeTests
               // }
            // }
           
            steps {
                echo 'Hello world!' 
                sh 'java -version'
                echo "Test"
            }
        
           // steps {
            ///    echo 'Testing the application....'
            //}
        }

       // stage('Deploy') {
          //  steps {
             //   echo 'Deploying the application....'
            //    echo "deploying the version ${params.VERSION}"
                
           // }
       // }
        
        stage('Deploy') {
            steps {
                echo 'Deploying the application....'
            }
        }
    }
}
