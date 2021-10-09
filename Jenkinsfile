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
                    echo "on FEATURE branch"
               }
          }
		  stage("Unit test") {
               steps {
                    sh "./gradlew test"
               }
          }
          stage("Static code analysis") {
               steps {
                    sh "./gradlew checkstyleMain"
               }
          }
     }
}
