node{

  stage('Preparation'){
    def mycontainer = docker.image('winamd64/openjdk')
    mycontainer.pull()
    mycontainer.inside{
      sh 'System.out.println("Hello")'
    }
  }



}
