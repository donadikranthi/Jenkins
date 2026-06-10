pipeline {
    agent {
        node {
            label 'AGENT' // Replace with your actual node label
        }

    stages {
    stage "Create build output"
    
    // Make the output directory.
    sh "mkdir -p output"

    // Write an useful file, which is needed to be archived.
    writeFile file: "output/usefulfile.txt", text: "This file is useful, need to archive it."

    // Write an useless file, which is not needed to be archived.
    writeFile file: "output/uselessfile.md", text: "This file is useless, no need to archive it."

    stage "Archive build output"
    
    // Archive the build output artifacts.
    archiveArtifacts artifacts: 'output/*.txt', excludes: 'output/*.md'
}
    }
}



// pipeline {
//        agent {
//             node {
//                label 'AGENT' // Replace with your actual node label
//        }
//  }

//     stages {  
//         stage('Build') {
//             steps {
//                 echo 'Building...'
//                 // Add your build commands here, e.g., sh 'mvn clean install'
//             }
//         }
//         stage('Test') {
//             steps {
//                 echo 'Testing...'
//                 // Add your test commands here, e.g., sh 'mvn test'
//             }
//         }
//         stage('Deploy') {
//             steps {
//                 echo 'Deploying...'
//                 // Add your deploy commands here, e.g., sh 'mvn deploy'
//             }
//         }
//     }
// }