node {
    stage('scm') {
        checkout scm
    }

    stage('build') {
        withEnv(["PATH+MAVEN=${tool 'maven-3.3.9'}/bin"]) {
            sh "mvn -B clean install"
        }
    }
}
