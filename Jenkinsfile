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

pipeline {
  agent any
  environment {
    avinash_URL='avinash.guruka.com'
  }

  stages {
    steps {
      sh 'echo "${avinash_URL}"'
      echo avinash_URL
    }
  }


}
