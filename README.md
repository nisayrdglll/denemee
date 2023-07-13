
<div align="center">
  <img src= "https://github.com/nisayrdglll/denemee/assets/115365248/6001fd62-1efa-48b9-8a9d-3bd92055ccbb"
  alt="Goo Web Server Logo">
  <hr>
</div>

<h1>What is GOO Web Server?  </h1>


<p>
  "GOO Web Server" is a cross-platform web development environment available for both Windows and Linux operating systems. It allows you to develop web applications using the Apache2 web server, PHP programming language, and a MySQL or PostgreSQL database. Whether you are using Windows or Linux, GOO Web Server provides a user-friendly interface. With GOO Web Server, you can seamlessly create and deploy web applications, taking advantage of the robust combination of Apache2, PHP, MySQL or PostgreSQL on both Windows and Linux platforms.
</p>
<p dir="auto">

  <a href="https://superset.apache.org" rel="nofollow"><img src="https://camo.githubusercontent.com/d65d51704b287e5d73f4c937a6268e674949aa7d61aa10478003d9d7c0461272/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f646f63732d6170616368652e6f72672d626c75652e737667" alt="Documentation" data-canonical-src="https://img.shields.io/badge/docs-apache.org-blue.svg" style="max-width: 100%;"></a>
  <a><img src="https://camo.githubusercontent.com/2a2157c971b7ae1deb8eb095799440551c33dcf61ea3d965d86b496a5a65df55/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f4c6963656e73652d417061636865253230322e302d626c75652e737667" alt="License" data-canonical-src="https://img.shields.io/badge/License-Apache%2.4.57-blue.svg" style="max-width: 100%;">
  </a>
<a>
<img src="https://camo.githubusercontent.com/cd8d1278950d417149d42b9c5e47795a19afce997b390ba6668f35abde0b09a5/68747470733a2f2f696d672e736869656c64732e696f2f7061636b61676973742f646570656e64656e63792d762f6d657966612f7068702d7376672f7068703f7374796c653d706c6173746963" alt="Packagist PHP Version" data-canonical-src="https://img.shields.io/packagist/dependency-v/meyfa/php-svg/php?style=plastic" style="max-width: 100%;">
</a>
<a href="https://codeclimate.com/github/meyfa/php-svg/maintainability" rel="nofollow"><img src="https://camo.githubusercontent.com/61e5e28c2aec895e6c83bcc02da4c7f780c619eff615f36cc18e0cfabb3b92c4/68747470733a2f2f6170692e636f6465636c696d6174652e636f6d2f76312f6261646765732f38663733343638363031613635336166663065382f6d61696e7461696e6162696c697479" alt="Maintainability" data-canonical-src="https://api.codeclimate.com/v1/badges/8f73468601a653aff0e8/maintainability" style="max-width: 100%;"></a>

</p>

<hr>
<div>
  <h2>Why should we use the GOO Web Server?</h2>
  
  <ul>
  <li>
    <strong>Hosting Web Applications:</strong> The GOO Web Server allows you to host and serve your web applications, making them accessible to users over the internet.
  </li>
  <li>
    <strong>Platform for Dynamic Content:</strong> With the GOO Web Server, you can run server-side scripting languages like PHP, enabling the creation of dynamic and interactive web pages.
  </li>
  <li>
    <strong>Database Integration:</strong> The GOO Web Server often comes with support for database systems like MySQL and PostgreSQL.This integration allows you to store and retrieve data for your web applications.
  </li>
  <li>
    <strong>Scalability and Performance:</strong> The GOO Web Server is designed to handle multiple concurrent requests efficiently, ensuring high performance and scalability as your application grows.
  </li>
  <li>
    <strong>Security Features:</strong> The GOO Web Server may include security features such as SSL/TLS encryption, access control, and firewalls to protect your web applications and data.
  </li>
  <li>
    <strong>Cross-Platform Compatibility:</strong> The GOO Web Server supports multiple operating systems like Windows and Linux, allowing you flexibility in choosing your development and deployment environment.
  </li>
  <li>
    <strong>User-Friendly Interfaces:</strong> The GOO Web Server often comes with user-friendly interfaces or control panels that simplify the configuration, management, and monitoring of server settings.
  </li>
</ul>
</div>
<hr>
<div>
   <h2>Configuration Settings</h2>
   <h3>Apache Configuration Settings</h3>
  <li><strong>Step 1: Locate the Configuration File</strong></li>

  <p>Find the Apache configuration file named <code>httpd.conf</code>. The location of this file may vary depending on your system and installation method. Typically, it is located in one of the following paths:</p>
  <ul>
    <li><code>C:\Program Files\INOSAS\GOO\bin\Apache24\conf\httpd.conf</code></li>
  </ul>
<li><strong>Step 2: Edit the Configuration File</strong></li>

  <p>Open the <code>httpd.conf</code> file in a text editor. You may need superuser privileges to edit this file.</p>
<li><strong>Step 3: Configure Server Settings</strong></li>

  <p>Modify the relevant server settings to meet your requirements. Here are some common configuration options:</p>
  <ul>
    <li><code>ServerName</code>: Set the hostname or IP address for the server.</li>
    <li><code>Listen</code>: Specify the port number on which the server listens for incoming connections.</li>
    <li><code>DocumentRoot</code>: Set the directory where the server should look for files to serve.</li>
    <li><code>DirectoryIndex</code>: Specify the default file to serve when a directory is accessed.</li>
    <li><code>ErrorLog</code>: Set the file path where error logs will be written.</li>
  </ul>
<li><strong>Step 4: Save and Restart Apache</strong></li>

  <p>Save the changes to the <code>httpd.conf</code> file and exit the text editor. Then, restart Apache for the new configuration to take effect.</p>
  <pre><code>sudo systemctl restart apache2</code></pre>
<li><strong>Step 5: Test the Configuration</strong></li>
  <p>Open a web browser and access your server using its hostname or IP address. Verify that the changes you made in the configuration file are applied correctly.</p>

  <p>For more detailed information about Apache configuration options, refer to the <a href="https://httpd.apache.org/docs/2.4/">Apache documentation</a>.</p>
<h3>PHP Configuration Settings</h3>
<ul>
  <li><strong>LoadModule:</strong> You can load the PHP module by adding a <code>LoadModule</code> directive specific to PHP. The directive should specify the path to the PHP module shared object file. For example:</li>
</ul>
<pre><code class="bash">LoadModule php7_module modules/libphp7.so</code></pre>
<ul>
  <li><strong>&lt;FilesMatch&gt;:</strong> You can use the <code>&lt;FilesMatch&gt;</code> directive to apply specific configurations to PHP files. For example, to set the PHP handler for files with a <code>.php</code> extension, you can use the following:</li>
</ul>
<pre><code class="php">&lt;FilesMatch \.php$&gt;
    SetHandler application/x-httpd-php
&lt;/FilesMatch&gt;</code></pre>
<ul>
  <li><strong>DirectoryIndex:</strong> The <code>DirectoryIndex</code> directive specifies the default filenames to use when a directory is requested. You can include PHP files in the list of default filenames. For example:</li>
</ul>
<pre><code>DirectoryIndex index.php index.html</code></pre>
<ul>
  <li><strong>AddType:</strong> The <code>AddType</code> directive can be used to associate the <code>.php</code> file extension with the PHP handler. This ensures that Apache recognizes PHP files and processes them accordingly. For example:</li>
</ul>
<pre><code class="bash">AddType application/x-httpd-php .php</code></pre>
<p>These are just a few examples of customizations you can make in the Apache configuration file to tailor it for PHP. Remember to restart the GOO Web Server after making any changes to the configuration file for the changes to take effect.</p>

<h3>Database Configuration Settings </h3>
<h3>PHP MySQL Configuration Settings</h3>
<ul>
  <li>
    <strong>MySQL Database Connection:</strong> To connect to a MySQL database, you'll need to provide the following configuration settings:
    <ul>
      <li>Database Host: The hostname or IP address where the MySQL server is running.</li>
      <li>Database Port: The port number on which the MySQL server is listening (usually 3306 by default).</li>
      <li>Database Name: The name of the MySQL database you want to connect to.</li>
      <li>Database User: The username for authenticating with the MySQL server.</li>
      <li>Database Password: The password for the MySQL user.</li>
    </ul>
    Here's an example of how you can specify these settings in the Apache configuration file using environment variables:
  </li>
</ul>
<pre><code class="apache">
SetEnv DB_HOST localhost
SetEnv DB_PORT 3306
SetEnv DB_NAME mydatabase
SetEnv DB_USER myusername
SetEnv DB_PASS mypassword
</code></pre>
<h3>PHP PostgreSQL Configuration Settings</h3>
<ul>
  <li>
    <strong>PostgreSQL Database Connection:</strong> To connect to a PostgreSQL database, you'll need to provide the following configuration settings:
    <ul>
      <li>Database Host: The hostname or IP address where the PostgreSQL server is running.</li>
      <li>Database Port: The port number on which the PostgreSQL server is listening (usually 5432 by default).</li>
      <li>Database Name: The name of the PostgreSQL database you want to connect to.</li>
      <li>Database User: The username for authenticating with the PostgreSQL server.</li>
      <li>Database Password: The password for the PostgreSQL user.</li>
    </ul>
    Here's an example of how you can specify these settings in the Apache configuration file using environment variables:
  </li>
</ul>
<pre><code class="apache">
SetEnv DB_HOST localhost
SetEnv DB_PORT 5432
SetEnv DB_NAME mydatabase
SetEnv DB_USER myusername
SetEnv DB_PASS mypassword
</code></pre>
<p>
Make sure to customize the settings based on your specific MySQL or PostgreSQL database setup. Remember to restart the GOO Web Server after making any changes to the configuration file for the changes to take effect.
</p>

</div>
<hr>

<div>
  <h2>Installation </h2>
  <h3>Windows</h3>
  <ol>
    <li>First, go to <a href="https://httpd.apache.org/docs/2.4/platform/windows.html">https://httpd.apache.org/docs/2.4/platform/windows.html</a> and review the complete documentation.</li>
    <li>Download the necessary resources:
      <ul>
        <li>Download the latest version of the GOO Web Server from <a href="https://inosas.com/downloads/GooWS-3.2.8-Win_x64-Server.exe">https://inosas.com/downloads/GooWS-3.2.8-Win_x64-Server.exe</a>.</li>
      </ul>
    </li>
    <li>Run the downloaded installation file. The installation wizard will start.</li>
    <li>Follow the steps guided by the installation wizard. The installation typically includes the following steps:
      <ul>
        <li>Accept the license agreement.</li>
        <li>Select the installation type. Usually, you should choose the "Typical" installation option.</li>
        <li>Specify the installation location. You can accept the default value or choose a different location.</li>
        <li>Start the installation and wait for it to complete.</li>
      </ul>
    </li>
    <li>Once the installation is complete, the GOO Web Server will be successfully installed. You can find the installed directory by navigating to the location you specified during the installation process.</li>
    <li>Customize your server by editing the configuration file (httpd.conf). This file is typically located in the "conf" subdirectory of the installation directory.</li>
    <li>Start the GOO Web Server. You can start it by running the startup file or managing services.</li>
    <li>Verify that the GOO Web Server is running by visiting <a href="http://localhost">http://localhost</a> or <a href="https://localhost">https://localhost</a> in your browser. By default, you should see the GOO Web Server info page with the configuration settings.</li>
  </ol>
<div>
  <h3>Linux</h3>

 <ol>
  <li><strong>Install Required Dependencies</strong></li>
  <p>Open a terminal and use the following command to update the system's package list:</p>
  <pre><code>sudo apt update</code></pre>
  <li><strong> Install Apache Web Server</strong></li>
  <p>Use the following command to install the Apache web server:</p>
  <pre><code>sudo apt install apache2</code></pre>
  <p>During the installation, your system may ask you to confirm permissions or install additional dependencies. Confirm any prompted actions and wait for the installation to complete.</p>
  <li><strong>Start Apache Web Server</strong></li>
  <p>Use the following command to start the Apache web server:</p>
  <pre><code>sudo systemctl start apache2</code></pre>
  <li><strong>Enable Automatic Startup</strong></li>
  <p>To ensure Apache automatically starts when the system boots up, use the following command:</p>
  <pre><code>sudo systemctl enable apache2</code></pre>
  <li><strong>Verify the Installation</strong></li>
  <p>Open your web browser and visit the following URL:</p>
  <pre><code>http://localhost/ or https://localhost/ </code></pre>
  <p>You should see the default Apache web page. If you can see it, that means Apache web server has been successfully installed.</p>
</ol>


</div>
<hr>


<div>
  <h2>License</h2>

  <p>This project is licensed under the <a href="https://www.apache.org/licenses/LICENSE-2.0">Apache License 2.0</a>. The license text can be found below:</p>

  <pre>
Apache License
Version 2.0, January 2004
http://www.apache.org/licenses/
  </pre>

  <p>You can also find the license text in the project's root directory in the <code>LICENSE</code> file. For more details, please refer to the <a href="https://github.com/nisayrdglll/denemee/blob/main/LICENCE">LICENSE</a> file.</p>
</div>

