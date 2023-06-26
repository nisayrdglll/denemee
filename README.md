
<div align="center">
  <img src= "https://github.com/nisayrdglll/denemee/assets/115365248/6001fd62-1efa-48b9-8a9d-3bd92055ccbb"
  alt="Goo Web Server Logo">
  <hr>
</div>
<h2>What is Goo Web Server? </h2>
<p>
  "Goo Web Server" is a cross-platform web development environment available for both Windows and Linux operating systems. It allows you to develop web applications using the Apache2 web server, PHP programming language, and a MySQL database. Whether you are using Windows or Linux, Goo Web Server provides a user-friendly interface, including PhpMyAdmin, which simplifies the management of your databases. With Goo Web Server, you can seamlessly create and deploy web applications, taking advantage of the robust combination of Apache2, PHP, and MySQL on both Windows and Linux platforms.
</p>
<a href="https://www.linkedin.com/company/inosas/">
  <img src="https://camo.githubusercontent.com/1ffde4ea8d2869a62cdf80282516c524e1109befc83d6339aae7a55d94ff4ae5/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f2d4c696e6b6564496e2d626c61636b2e7376673f7374796c653d666f722d7468652d6261646765266c6f676f3d6c696e6b6564696e26636f6c6f72423d353535" alt="LinkedIn" data-canonical-src="https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&amp;logo=linkedin&amp;colorB=555" style="max-width: 100%; filter: invert(100%);"></a>

<hr>
<div>
  <h3>Why should we use the Goo Web Server?</h3>
  <ul>
  <li>
    <strong>Hosting Web Applications:</strong> The Goo Web Server allows you to host and serve your web applications, making them accessible to users over the internet.
  </li>
  <li>
    <strong>Platform for Dynamic Content:</strong> With the Goo Web Server, you can run server-side scripting languages like PHP, Python, or Node.js, enabling the creation of dynamic and interactive web pages.
  </li>
  <li>
    <strong>Database Integration:</strong> The Goo Web Server often comes with support for database systems like MySQL, PostgreSQL, or MongoDB. This integration allows you to store and retrieve data for your web applications.
  </li>
  <li>
    <strong>Scalability and Performance:</strong> The Goo Web Server is designed to handle multiple concurrent requests efficiently, ensuring high performance and scalability as your application grows.
  </li>
  <li>
    <strong>Security Features:</strong> The Goo Web Server may include security features such as SSL/TLS encryption, access control, and firewalls to protect your web applications and data.
  </li>
  <li>
    <strong>Cross-Platform Compatibility:</strong> The Goo Web Server supports multiple operating systems like Windows and Linux, allowing you flexibility in choosing your development and deployment environment.
  </li>
  <li>
    <strong>User-Friendly Interfaces:</strong> The Goo Web Server often comes with user-friendly interfaces or control panels that simplify the configuration, management, and monitoring of server settings.
  </li>
</ul>
</div>
<hr>
<div>
  <h3>Configuration Settings</h3>
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

