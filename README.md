<div id="top"></div>
[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![MIT License][license-shield]][license-url]
[![LinkedIn][linkedin-shield]][linkedin-url]



<!-- PROJECT LOGO -->
<br />


<h3 align="center">PHP Advanced Security</h3>

  <p align="center">
    Advanced Security is Register/Login and User Management System with high security, developed using pure PHP and MySQL database.
    <br />
    <a href="https://github.com/ridhoariefmuharram"><strong>Explore the docs »</strong></a>
    <br />
    <br />
    <a href="https://github.com/ridhoariefmuharram">View Demo</a>
    ·
    <a href="https://github.com/ridhoariefmuharram">Report Bug</a>
    ·
    <a href="https://github.com/ridhoariefmuharram">Request Feature</a>
  </p>
</div>



<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#roadmap">Roadmap</a></li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="#acknowledgments">Acknowledgments</a></li>
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## About The Project

[![Product Name Screen Shot][product-screenshot]](https://example.com)

Advanced Security is Register/Login and User Management System with high security, developed using pure PHP and MySQL database.

Lets say you have your own website and you want to extend it by adding user registration and login system. Insted of coding for few days and thinking about all security holes, you can just take this system, install it, and your work is done.

Just add two lines of code on top of your old pages to allow only registred users to access them and that's it. 

Advanced Security classes offer you a lot of built in methods, and you can add your own if you want. `github_username`, `repo_name`, `twitter_handle`, `linkedin_username`, `email`, `email_client`, `project_title`, `project_description`

<p align="right">(<a href="#top">back to top</a>)</p>



### Built With

* [Next.js](https://nextjs.org/)
* [React.js](https://reactjs.org/)
* [Vue.js](https://vuejs.org/)
* [Angular](https://angular.io/)
* [Svelte](https://svelte.dev/)
* [Laravel](https://laravel.com)
* [Bootstrap](https://getbootstrap.com)
* [JQuery](https://jquery.com)

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- GETTING STARTED -->
## Getting Started

SQL Injection
Advanced Security System has own database class that extends PDO and use prepared statements to prevent SQL Injection attacks.

Session Security
Your session cookies are very important while you are logged in. If someone still you a session cookie, he can log in and do whatever he wants, logged in like you!

Advanced Security creates secure, HTTP only cookies, whitch can't be accessed via JavaScript and session Id will be regenerated every time (if you selected that option during installation process).

Also, there is an option to enable "login fingerprint". This basically means that every time you log in. hash of your IP address and name of browser you are using are stored inside $_SESSION variable, and if someone somehow steal your session cookie, this will protect you.

CSRF protection is also included. That means that forms can only be submited from your website, so you don't have to worry if someone will spam your website or perform some malicios actons.

Password Encryption
Password encryption is, of course, very important factor. 

Advanced Security System encrypts your password twice.

Password is encrypted on client side using Javascript before it is event sent through the network, so you don't have to worry if you don't have HTTPS (but, to improve your security, it's recommended that you get HTTPS).

Password is encrypted on server side with encryption method you have selected during the installation process. 

Available encryption methods are Bcrypt with selected cost (using salt of course) and SHA-512 with salt and thousands of iterations. 

Salt is random generated string during the registration process.

Brute Force Attack
System prevents brute force attacks too by blocking user IP address for one day, if there are specific number of invalid login attempts. You can set number of login attempts during installation wizard..

### Prerequisites

This is an example of how to list things you need to use the software and how to install them.
* npm
  ```sh
  npm install npm@latest -g
  ```

### Installation

Extract and upload downloaded zip file
When you download zip file with source code, first thing you need to do is to extract it and upload extracted content to your web server using FTP or web uploader.
 
Create database
Now you need to create database where you want to Advanced Security Installation Wizard to create necessary tables.
 
NOTE: If you already have database created for your website, you don't need to create new database. Installation wizard will create all database tables prefixed with as_
 
NOTE: All tables that will be created by the installation wizard use utf8 encoding and utf8_unicode_ci collation. You will have to set your database to use utf8_unicode_ci collation, so it can work properly.  However, if you are not going to use utf caracter set, you can skip this.
Start installation wizard
Everything is prepared now, you can start installation wizard by accessing install.php or index.php file inside install folder. 
 
Example: If your domain is www.example.com, and you have uploaded Advanced Security files into root directory, you can start installation wizzard by accessing www.example.com/install/install.php or  www.example.com/install/index.php 
 
NOTE: Make sure you have set permission for ASEngine folder to 777 before you proceed. That's because wizard will create configuration file inside that directory.
 
Now you need to follow installation wizard and customize Advanced Security installation. Here is an WAMP instalation example for this version:

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- USAGE EXAMPLES -->
## Usage

Use this space to show useful examples of how a project can be used. Additional screenshots, code examples and demos work well in this space. You may also link to more resources.

_For more examples, please refer to the [Documentation](https://example.com)_

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- ROADMAP -->
## Roadmap

- [] Feature 1
- [] Feature 2
- [] Feature 3
    - [] Nested Feature

See the [open issues](https://github.com/github_username/repo_name/issues) for a full list of proposed features (and known issues).

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- CONTRIBUTING -->
## Contributing

Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
Don't forget to give the project a star! Thanks again!

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- LICENSE -->
## License

Distributed under the MIT License. See `LICENSE.txt` for more information.

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- CONTACT -->
## Contact

Ridho Arief Muharram - [@twitter_handle](https://twitter.com/twitter_handle) - email@email_client.com

Project Link: [https://github.com/github_username/repo_name](https://github.com/github_username/repo_name)

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- ACKNOWLEDGMENTS -->
## Acknowledgments

* []()
* []()
* []()

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/github_username/repo_name.svg?style=for-the-badge
[contributors-url]: https://github.com/github_username/repo_name/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/github_username/repo_name.svg?style=for-the-badge
[forks-url]: https://github.com/github_username/repo_name/network/members
[stars-shield]: https://img.shields.io/github/stars/github_username/repo_name.svg?style=for-the-badge
[stars-url]: https://github.com/github_username/repo_name/stargazers
[issues-shield]: https://img.shields.io/github/issues/github_username/repo_name.svg?style=for-the-badge
[issues-url]: https://github.com/github_username/repo_name/issues
[license-shield]: https://img.shields.io/github/license/github_username/repo_name.svg?style=for-the-badge
[license-url]: https://github.com/github_username/repo_name/blob/master/LICENSE.txt
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://linkedin.com/in/linkedin_username
[product-screenshot]: images/screenshot.png
