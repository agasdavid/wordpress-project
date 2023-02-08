Documentation of steps I took  to create a WordPress website on an EC2 instance connected to an RDS:

Launch an EC2 instance: I Started by launching a new EC2 instance using the AWS Management Console. I Choosed an Ubuntu AMI, and select the appropriate instance type for my needs.

Connect to the EC2 instance: I connect to the EC2 instance using SSH. You will need the private key associated with the instance and the public IP of the instance.

Install LAMP stack: Once you are connected to the EC2 instance, install a LAMP (Linux, Apache, MySQL, PHP) stack on the instance. This can be done using the following command: sudo yum install -y httpd php php-mysqlnd.

Create an RDS instance: Create a new RDS instance in the AWS Management Console. Choose MySQL as the database engine, and select the appropriate instance type and storage size.

Connect to the RDS instance: Once the RDS instance is up and running, you can connect to it from the EC2 instance using the MySQL client. You will need the endpoint and credentials for the RDS instance.

Create a database for WordPress: Use the MySQL client to create a new database for your WordPress installation. You can use the following command: CREATE DATABASE wordpress;

Download and install WordPress: Download the latest version of WordPress from the official website and install it on the EC2 instance. You will need to configure WordPress to use the database created in the RDS instance.

Configure the Apache web server: Configure the Apache web server to serve the WordPress installation by creating a virtual host and updating the DocumentRoot directive.

Test the WordPress site: Test the WordPress site by accessing it using the public IP of the EC2 instance.

Configure security:y Configure security for the EC2 and RDS instances by setting up firewall rules, securing the SSH access, and implementing SSL/TLS encryption.


Note: This is a high-level overview of the steps involved in creating a WordPress website on EC2 connected to an RDS. The actual process may vary depending on the specific requirements and configurations.

