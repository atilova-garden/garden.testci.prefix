pipeline {
     agent any
 
     stages {
         stage('Show Git Info!') {
             steps {
                 script {
                     sh 'echo "Commit: $(git rev-parse HEAD)"'
                     sh 'echo "Repo: $(basename -s .git `git config --get remote.origin.url`)"'
                     sleep time: 20, unit: 'SECONDS'
                 }
             }
         }
     }
 }
