pipeline {
          agent any 
          stages {
            stage ('VALIDATE') {
              steps {
                  sh '''
                        #!/bin/bash
                        echo "validates the project is correct and all necessary infomation is available or not"
                        
                     '''   
                    }
                 }
            stage ('COMPILE') {
              steps {
                  sh '''
                        #!/bin/bash
                        echo "complies the complete source code which is present is src directory."
                        
                     '''   
              }
            }  
            stage ('TEST') {
              steps {
                 sh ''' 
                       #!/bin/bash
                       echo "test the compiled source code with unit testing if it present."
                    '''
              }
            }
            stage ('PACKAGE') {
              steps {
                 sh ''' 
                       #!/bin/bash
                       echo "take the compiled code and it packages it into a distributable format such as jar, war, ear"
                    '''
              }
            }
             stage ('INTEGRATION TEST') {
              steps {
                 sh ''' 
                       #!/bin/bash
                       echo "deploy the package into an environment and run integration test "
                    '''   
              }
            }
            stage ('VERIFY') {
              steps {
                 sh ''' 
                       #!/bin/bash
                       echo "verify the package is valid and meets quality criteria"
                    '''   
              }
            }
            stage ('INSTALL') {
              steps {
                 sh ''' 
                       #!/bin/bash
                       echo "install the package into local repository."
                    '''   
              }
            }
            stage ('DEPLOY') {
              steps {
                 sh ''' 
                       #!/bin/bash
                       echo "deploy the package to relese environment."
                    '''   
              }
            }
            
            
   }

}
