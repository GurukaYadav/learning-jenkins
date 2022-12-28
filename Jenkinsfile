// pipeline {
// 	agent any
//
// 	stages {
//
// 	  stage('Avinash'){
//       steps {
// 	      echo 'This is Avinash'
// 	    }
// 	  }
//
// 	  stage('Arun'){
//        steps {
//     	  echo 'This is Arun'
//     	 }
//     }
//
//     stage('Anusha'){
//        steps {
//         echo 'This is Anusha'
//        }
//     }
// 	}
// 	post {
// 	  changed {
// 	    echo "This is changed"
// 	  }
// 	  unstable {
// 	    echo "This is not stable"
// 	  }
// 	  cleanup {
// 	    echo "This is Guruka Avinash"
// 	  }
// 	}
//
// }

// Environment directive:

// Declarative pipeline

pipeline {
  agent any
//   Here Environment can be used in 2 ways: 1. to hardcode the environment variables (2). to read the passwords
  environment {
    avinash_URL='avinash.guruka.com'
    SSH=credentials('SSH')
  }

  parameters {
          string(name: 'PERSON', defaultValue: 'Mr Jenkins', description: 'Who should I say hello to?')

          text(name: 'BIOGRAPHY', defaultValue: '', description: 'Enter some information about the person')

          booleanParam(name: 'TOGGLE', defaultValue: true, description: 'Toggle this value')

          choice(name: 'CHOICE', choices: ['One', 'Two', 'Three'], description: 'Pick something')

          password(name: 'PASSWORD', defaultValue: 'SECRET', description: 'Enter a password')
   }
  stages {
    stage(avinash_URL) {
      steps {
        sh 'echo "${avinash_URL}"'
        echo avinash_URL
        echo SSH
        echo person
        sh 'echo "${person}"
      }
    }
  }


}

// Scripted pipeline

// env.avinash_URL='avinash.guruka.com'
// node() {
//   stage(avinash_URL){
//     sh 'echo "${avinash_URL}"'
//     echo avinash_URL
//   }
//
// }
