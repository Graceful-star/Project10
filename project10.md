# Documentation of project10
## Step1
1. I created an EC2 VM based on ubuntu and named it 'nginx-lb'
    
    ![ubuntu](images/image1.PNG)

2. I updated ubuntu
   
   `sudo apt update`
   ![ubuntu](images/image2.PNG)

3. I installed nginx

    `sudo apt install nginx`

    ![ubuntu](images/image3.PNG)

4.  I updated '/etc/hosts' file with web servers name

    ![ubuntu](images/image4.PNG)

5. I updated the configuration file too
    
    ![ubuntu](images/image5.PNG)

6. I restarted Nginx and ensured it was up and running

## Step2
1. I registered a new domain name and hosted it

    ![ubuntu](images/image6.PNG)

2. I linked it to an elastic ip that I just created
      
      ![ubuntu](images/image7.PNG)

3.  I confirmed that my webserver can connect on my browser using the domain name
     
     ![ubuntu](images/image12.PNG)

4.  I ensured snapd service was up and running
   
   ![ubuntu](images/image13.PNG)

5.  I installed certbot

   ![ubuntu](images/image14.PNG)

6.  I requested for my certificate

    ![ubuntu](images/image15.PNG)

7.  I accessed my website on the browser and clicked on the padlock pictogram on my browser's search string
    ![ubuntu](images/image16.PNG)

8.  I tested the renewal command in dry mode

     `sudo certbot renew --dry-run`
  ![ubuntu](images/image17.PNG)
    
9.  I configured a 'crownjob' to run renew command periodically
    `crontab -e`
    ![ubuntu](images/image18.PNG)
    

