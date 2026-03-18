pipeline{

		agent {
			
			label {

				label "slave-2"
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

					sh "sudo cp -r index.html /var/www/html/"
					sh "sudo chmod -R 777 /var/www/html/index.html"
			    		}

			
				}





	
			}
	}
