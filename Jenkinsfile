
pipeline {
      agent{
	      label{
		        label'built-in'
				customWorkspace'/mnt/assignmet4/22Q1'
		  } 
	  }
	  stages{
	       /* stage('stage1-22Q1'){
			    steps {
				       sh "docker kill 22Q1-httpd"
				       sh "docker rm 22Q1-httpd"
				       
				}
			} */
			stage('docker-stage-22Q1'){
			      steps{
				        
						sh "docker run --name 22Q1-httpd -itdp 80:80 httpd"
				               sh "chmod -R 777 /mnt/assignmet4/22Q1/index.html"
						sh "cd /mnt/assignmet4/22Q1 && docker cp index.html 22Q1-httpd:/usr/local/apache2/htdocs/"
				  }
			}
	  }
	  
}
