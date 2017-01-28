node {
    stage "scm" {
        checkout scm
    }

    stage "build" {
        def mvnHome = tool 'maven-3.3.9'
        sh "${mvnHome}/bin/mvn clean install"
    }
}
