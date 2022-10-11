pipeline {
      agent{
	      label{
		        label'built-in'
				customWorkspace'/mnt/assignmet4/22Q3'
		  } 
	  }
	  stages{
	       /* stage('stage1-22Q3'){
			    steps {
				       sh "docker kill 22Q3-httpd"
				       sh "docker rm 22Q3-httpd"
				       
				}
			} */
			stage('docker-stage-22Q3'){
			      steps{
				        
						sh "docker run --name 22Q2-httpd -itdp 70:80 httpd"
				               sh "chmod -R 777 /mnt/assignmet4/22Q2/index.html"
						sh "cd /mnt/assignmet4/22Q2 && docker cp index.html 22Q2-httpd:/usr/local/apache2/htdocs/"
				  }
			}
	  }
	  
}
