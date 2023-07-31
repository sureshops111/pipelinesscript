pipeline {
        agent any
        options{timestamps()}
        tools{maven 'maven-3.8.8'}
        parameters {
        string(defaultValue: '1.0.0', description: '', name: 'buildnumber')
        }
        stages{
                stage('Declarative-stage') {
                    steps {
                        // One or more steps need to be included within the steps block.
                        println "executing Declarative stage"
                        sh "mvn -v"
                        echo "The build number is: ${params.buildnumber}"
                    }
                }
         }
   }
