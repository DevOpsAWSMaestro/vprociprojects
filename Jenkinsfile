pipeline {

    agent any

    tools {

        maven "maven3"

        jdk "jdk8"

    }

    environment {

        SNAP_REPO = 'vprofile-snapshot'

        NEXUS_USER = 'admin'

        NEXUS_PASS = 'admin@123'

        RELEASE_REPO = 'vprofile-release'

        CENTRAL_REPO = 'vprofile-maven-central'

        NEXUSIP = '44.211.67.163'

        NEXUSPORT = '8081'

        NEXUS_GRP_REPO = 'vprofile-maven-group'

        NEXUS_LOGIN = 'nexuslogin'

    }

    stages {

        stage('build') {

            steps {

                script {

                    sh "mvn -s settings.xml -DskipTests install"

                }

            }

        }

    }

}