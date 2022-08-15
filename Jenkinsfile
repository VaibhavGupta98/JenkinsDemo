// node{

//   stage('Preparation'){
//     def mycontainer = docker.image('winamd64/openjdk')
//     mycontainer.pull()
//     mycontainer.inside{
//       sh 'System.out.println("Hello")'
//     }
//   }



// }

node {
    /* Requires the Docker Pipeline plugin to be installed */

    stage('Back-end') {
        docker.image('maven:3.8.1-adoptopenjdk-11').inside {
            sh 'mvn --version'
        }
    }

    stage('Front-end') {
        docker.image('node:16.13.1-alpine').inside {
            sh 'node --version'
        }
    }
}
