pipeline {
      agent{
	      label{
		        label'built-in'
				customWorkspace'/mnt/assignmet4/22Q2'
		  } 
	  }
	  stages{
	       /* stage('stage1-22Q2'){
			    steps {
				       sh "docker kill 22Q2-httpd"
				       sh "docker rm 22Q2-httpd"
				       
				}
			} */
			stage('docker-stage-22Q2'){
			      steps{
				        
						sh "docker run --name 22Q2-httpd -itdp 90:80 httpd"
				               sh "chmod -R 777 /mnt/assignmet4/22Q2/index.html"
						sh "cd /mnt/assignmet4/22Q2 && docker cp index.html 22Q2-httpd:/usr/local/apache2/htdocs/"
				  }
			}
	  }
	  
}

