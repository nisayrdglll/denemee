
<div align="center">
  <img src= "https://github.com/nisayrdglll/denemee/assets/115365248/6001fd62-1efa-48b9-8a9d-3bd92055ccbb"
  alt="Goo Web Server Logo">
  <hr>
</div>

<h1>What is GOO Web Server?  </h1>


<p>
  "GOO Web Server" is a cross-platform web development environment available for both Windows and Linux operating systems. It allows you to develop web applications using the Apache2 web server, PHP programming language, and a MySQL or PostgreSQL database. Whether you are using Windows or Linux, GOO Web Server provides a user-friendly interface, including PhpMyAdmin, which simplifies the management of your databases. With GOO Web Server, you can seamlessly create and deploy web applications, taking advantage of the robust combination of Apache2, PHP, and MySQL on both Windows and Linux platforms.
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
    <strong>Platform for Dynamic Content:</strong> With the GOO Web Server, you can run server-side scripting languages like PHP, Python, or Node.js, enabling the creation of dynamic and interactive web pages.
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
  
 <ul>
  <li><strong>Define app_dir "C:\Program Files\INOSAS\GOO":</strong>
    <ul>
      <li>This line defines a macro <code>app_dir</code> with the value <code>"C:\Program Files\INOSAS\GOO"</code>.</li>
      <li>Macros allow you to define reusable variables in the configuration.</li>
    </ul>
  </li>

  <li><strong>ServerRoot "${SRVROOT}":</strong>
    <ul>
      <li>This directive sets the server's root directory to the value of the <code>SRVROOT</code> macro.</li>
      <li>The <code>SRVROOT</code> macro is defined as <code>"${app_dir}\bin\Apache24"</code>.</li>
      <li>The server's configuration, error, and log files will be stored in this directory.</li>
    </ul>
  </li>

  <li><strong>Listen 80:</strong>
    <ul>
      <li>This directive specifies that the server should listen on port 80 for incoming requests.</li>
    </ul>
  </li>

  <li><strong>LoadModule:</strong>
    <ul>
      <li>These directives load modules (extensions) that provide additional functionality to the server.</li>
      <li>Each <code>LoadModule</code> directive loads a specific module by specifying its shared object file (.so file) or equivalent for Windows.</li>
      <li>The listed modules include modules for authentication, authorization, SSL/TLS, PHP, and more.</li>
    </ul>
  </li>

  <li><strong>&lt;IfModule unixd_module&gt;:</strong>
    <ul>
      <li>This section contains directives specific to the <code>unixd_module</code>.</li>
      <li>The <code>unixd_module</code> is responsible for configuring the server to run as a specific user and group.</li>
      <li>In this case, the user and group are set to <code>daemon</code>.</li>
    </ul>
  </li>

  <li><strong>&lt;Directory&gt;:</strong>
    <ul>
      <li>This section specifies the configuration options for a specific directory.</li>
      <li>The given directory is <code>${app_dir}\www</code>.</li>
      <li>The options include allowing directory indexes (<code>Options +Indexes</code>) and overriding options in <code>.htaccess</code> files (<code>AllowOverride All</code>).</li>
    </ul>
  </li>

  <li><strong>DocumentRoot "${app_dir}\www":</strong>
    <ul>
      <li>This directive sets the document root directory to <code>${app_dir}\www</code>.</li>
      <li>This is the directory from which the server will serve web content.</li>
    </ul>
  </li>

  <li><strong>DirectoryIndex index.php index.html:</strong>
    <ul>
      <li>This directive specifies the default filenames to use when a directory is requested.</li>
      <li>In this case, the server will look for <code>index.php</code> and <code>index.html</code> files.</li>
    </ul>
  </li>

  <li><strong>&lt;Files ".ht*"&gt;:</strong>
    <ul>
      <li>This section restricts access to files starting with <code>.ht</code>.</li>
      <li>In this case, it denies access to such files.</li>
    </ul>
  </li>

  <li><strong>ErrorLog "logs/error.log":</strong>
    <ul>
      <li>This directive sets the location of the error log file to <code>"logs/error.log"</code>.</li>
      <li>This file will contain error messages generated by the server.</li>
    </ul>
  </li>

  <li><strong>LogLevel error:</strong>
    <ul>
      <li>This directive sets the log level to <code>error</code>.</li>
      <li>Only error-level messages will be logged.</li>
    </ul>
  </li>

  <li><strong>LogFormat:</strong>
    <ul>
      <li>These directives define the log file format for the access logs.</li>
      <li>The combined and common formats are defined here.</li>
    </ul>
  </li>
</ul>

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
        <li>Select the required components. Besides the GOO Web Server, you can choose optional modules or features.</li>
        <li>Start the installation and wait for it to complete.</li>
      </ul>
    </li>
    <li>Once the installation is complete, the GOO Web Server will be successfully installed. You can find the installed directory by navigating to the location you specified during the installation process.</li>
    <li>Customize your server by editing the configuration file (httpd.conf). This file is typically located in the "conf" subdirectory of the installation directory.</li>
    <li>Start the GOO Web Server. You can start it by running the startup file or managing services.</li>
    <li>Verify that the GOO Web Server is running by visiting <a href="http://localhost">http://localhost</a> in your browser. By default, you should see the GOO Web Server 3.2.8 installation page with the configuration settings.</li>
  </ol>

  <h3>Linux</h3>
  <ol>
    <li>First, go to <a href="https://httpd.apache.org/docs/2.4/platform/unix.html">https://httpd.apache.org/docs/2.4/platform/unix.html</a> and review the complete documentation.</li>
    <li>Download the necessary dependencies. Install the dependencies for Apache HTTP Server using the package manager specific to your Linux distribution.</li>
    <li>Download Apache HTTP Server. Use the following commands to download the source code:
      <ul>
        <li>$ wget https://archive.apache.org/dist/httpd/httpd-2.4.46.tar.gz</li>
        <li>$ tar -xf httpd-2.4.46.tar.gz</li>
        <li>$ cd httpd-2.4.46</li>
      </ul>
    </li>
    <li>Perform the compilation and installation:
      <ul>
        <li>$ ./configure --prefix=/usr/local/apache2</li>
        <li>$ make</li>
        <li>$ sudo make install</li>
      </ul>
    </li>
    <li>Customize your server by editing the

<hr>

<div>
  <h2>License</h2>

  <p>This project is licensed under the <a href="https://www.apache.org/licenses/LICENSE-2.0">Apache License 2.0</a>. The license text can be found below:</p>

  <pre>
  Apache License, Version 2.0 (ALv2)
  </pre>

  <p>You can also find the license text in the project's root directory in the <code>LICENSE</code> file. For more details, please refer to the <a href="https://github.com/nisayrdglll/denemee/blob/main/LICENCE">LICENSE</a> file.</p>
</div>

