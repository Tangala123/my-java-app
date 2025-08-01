pipeline{
  agent any
  stages{
    stage("Git"){
      when {
        branch 'develop'
      }
      steps{
        echo "Git Repo coming"
    }
    }
    stage("sonar"){
      when {
        branch 'test'
      }
      steps{
        echo "Sonarqube"
    }
    } 
     stage("build"){
      when {
        branch 'uat'
      }
      steps{
        echo "build artifacts coming"
    }
    }
     stage("nexus"){
      when {
        branch 'main'
      }
      steps{
        echo "nexus upload artifacts coming"
    }
    }
  }
}
