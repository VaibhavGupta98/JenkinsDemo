node{

  stage('Preparation'){
    def mycontainer = docker.image('openjdk')
    mycontainer.pull()
    mycontainer.inside{
      sh 'System.out.println("Hello")'
    }
  }



}
