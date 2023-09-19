pipeline{
  agent any
  stages{
    stage("one"){
    steps{
      echo ' hi this is lavanya '
    }
    }
    stage("two"){
      steps{
        input ('do you want to proceed?')
      }
    }
    stage("three")
    when{
      not{
        brancg "master"
      }
    }
    steps{
      echo "hello"
    }
  }
  stage("four")
  parallel {
    stage ('unit test'){
      steps{
        echo "running the unit-test "
      }
    }
    stage("integration test'){
          agent {
            docker {
              reusenode false
              ' image ubuntu '
            }
          }
          steps{
            echo"running the integration test"
          }
          }
          }
          }
          }
          }
