pipeline {
	agent any

	stages {

	  stage('Avinash'){
      steps {
	      echo 'This is Avinash'
	    }
	  }

	  stage('Arun'){
       steps {
    	  echo 'This is Arun'
    	 }
    }

    stage('Anusha'){
       steps {
        echo 'This is Anusha'
       }
    }
	}
	post {
	  changed {
	    echo "This is changed"
	  }
	  unstable {
	    echo "This is not stable"
	  }
	  cleanup {
	    echo "This is Guruka Avinash"
	  }
	}
	
}

