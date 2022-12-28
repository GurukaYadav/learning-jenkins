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
  environment {
    avinash_URL='avinash.guruka.com'
    SSH=credentials('SSH')
  }

  stages {
    stage(avinash_URL) {
      steps {
        sh 'echo "${avinash_URL}"'
        echo avinash_URL
        echo SSH
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
