pipeline{

		agent {
			
			label {

				label "built-in"
				customWorkspace "/mnt/vel-app-1"
				}

		}
			
		stages {
				stage ("install httpd"){

				steps  {

					sh "sudo yum install httpd -y"
			    		}

				}
				
				stage ("start httpd"){

				steps  {

					sh "sudo service start httpd"
			    		}

			
				}

				stage ("deploy index.html"){

				steps  {

					sh "cp -r index.html /var/www/html/"
					sh "chmod -R 777 /var/www/html/index.html"
			    		}

			
				}





	
			}
	}
