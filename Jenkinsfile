pipeline{
    agent any
    stages {
        stage("test"){
            steps{
                sh '''
                        echo "welcome to the test"

                    '''
            }
        }


         stage("production"){
            steps{
                sh '''
                        echo "welcome to the production. Added Jenkins"


                        sudo apt-get install nginx -y

                        sudo systemctl enable nginx

                        sudo systemctl start nginx
                        

                        sudo apt update -y

                        cd /var/www

                        mkdir html

                        sudo rm -rf html

                        git clone https://github.com/OnlySalam/WebDevproject.git html

                        

                    '''
            }
        }

    }
}