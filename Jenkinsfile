pipeline {
    agent any
    stages {
        stage('path') {
            steps {
                bat 'echo %PATH%'
            }
        }
        stage('Run Python Script') {
            steps {
                bat 'python .\\sonarPromExporter\\prometheus_exporter.py'
            }
        }
    }
    // environment {

    // PATH = "C:\\Users\\riyazahmad.yaligar\\AppData\\Local\\Programs\\Python\\Python312;C:\\Windows\\System32"

    // }
}

// pipeline {
//     agent any
//     node {
//   stage('SCM') {
//     checkout scm
//   }
//   stage('SonarQube Analysis') {
//     def mvn = tool 'Default Maven';
//     withSonarQubeEnv() {
//       sh "${mvn}/bin/mvn clean verify sonar:sonar -Dsonar.projectKey=test1 -Dsonar.projectName='test1'"
//     }
//   }
// }

//     stages {
//         stage ('Compile Stage') {

//             steps {
//                 withMaven(maven : 'maven_3_5_0') {
//                     sh 'mvn clean compile'
//                 }
//             }
//         }

//         stage ('Testing Stage') {

//             steps {
//                 withMaven(maven : 'maven_3_5_0') {
//                     sh 'mvn test'
//                 }
//             }
//         }


//         stage ('Deployment Stage') {
//             steps {
//                 withMaven(maven : 'maven_3_5_0') {
//                     sh 'mvn deploy'
//                 }
//             }
//         }
//     }
// }
