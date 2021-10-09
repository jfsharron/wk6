pipeline {
     agent any
     stages {
          stage("Compile") {
               steps {
                    sh "./gradlew compileJava"
               }
          }
          stage("echo branch") {
               steps {
                    echo "on PLAYGROUND branch"
               }
          }
     }
}
