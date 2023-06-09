<!-- Improved compatibility of back to top link: See: https://github.com/othneildrew/Best-README-Template/pull/73 -->
<a name="readme-top"></a>
<!--
*** Thanks for checking out the Best-README-Template. If you have a suggestion
*** that would make this better, please fork the repo and create a pull request
*** or simply open an issue with the tag "enhancement".
*** Don't forget to give the project a star!
*** Thanks again! Now go create something AMAZING! :D
-->



<!-- PROJECT SHIELDS -->
<!--
*** I'm using markdown "reference style" links for readability.
*** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
*** See the bottom of this document for the declaration of the reference variables
*** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.
*** https://www.markdownguide.org/basic-syntax/#reference-style-links
-->
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]



<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="https://github.com/haruchannn/reftion">
    <img src="public\assets\img\icon.png" alt="Logo" width="80" height="80">
  </a>

<h3 align="center">Reftion</h3>

  <p align="center">
    Reference list generation from Notion 
    <br />
    <a href="https://github.com/haruchannn/reftion"><strong>Explore the docs »</strong></a>
    <br />
    <br />
    <a href="https://github.com/haruchannn/reftion">View Demo</a>
    ·
    <a href="https://github.com/haruchannn/reftion/issues">Report Bug</a>
    ·
    <a href="https://github.com/haruchannn/reftion/issues">Request Feature</a>
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

<img src="public\assets\img\desc_overall.png" width="500">

Reftion provides a quick and easy way to generate a reference list based on information on your Notion database. Reftion currently employs the format "American Psychological Association 6th edition".

<p align="right">(<a href="#readme-top">back to top</a>)</p>



### Built With
* [![Laravel][Laravel.com]][Laravel-url]
* [![Bootstrap][Bootstrap.com]][Bootstrap-url]
* [![JQuery][JQuery.com]][JQuery-url]

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- GETTING STARTED -->
## Getting Started (for developers)
### Prerequisites
- Composer is installed
- Laravel is installed
- PHP is installed
- DB is created
- You already are signed up with Google Cloud Platform for OAuth verification.

### Installation

1. Clone the repo
2. Install npm packages & vite
   ```sh
   npm install
   npm install vite
   ```
3. Create user authorization function
   ```
   php artisan make:auth
   ```
4. Install Laravel Socialite
   ```
   composer require laravel/socialite
   ```
5. Create & modify DB
   ```
   php artisan migrate
   ```
6. Go to your DB and rename users.emailverified_at to users.lastlogin_at
7. Generate the app key
    ```
    php artisan key:generate
    ```
8. Add information below to the .env file
    ```
    GOOGLE_CLIENT_ID=XXXXXXXXXXXX
    GOOGLE_CLIENT_SECRET=YYYYYYYYYYY
    GOOGLE_CALLBACK_URL=http://ZZZZZZZZZ/login/google/callback

    GUEST_USER_EMAIL=reftionguest@gmail.com
    GUEST_USER_TOKEN=secret_z279aEnqy7FZEo8rVkEuQtcpxsSgJEQ4AwICJpkIUvw
    GUEST_USER_DBID=422fed2fabc04532a7930787a3d1809b
    ```
9. Modify the DB info of your .env file if necessary 

## Getting Started (for users)

You have to complete 4 steps below to use Reftion. 
1. Set up Notion DB Columns
2. Share API key of your Notion DB with Reftion
3. Set to Share your Notion DB
4. Share your Notion DB ID with Reftion

For more detailed information for each step, see [our user guide](https://reftion.com/onboarding).

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- USAGE EXAMPLES -->
## Usage

Reftion can generate a reference list for you based on Notion's database as long as it has "doi" and "tag" column. This saves time for academic writtings! 

_For more examples, please refer to the [Documentation](https://example.com)_

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- ROADMAP -->
## Roadmap

- [ ]  Support Japanese language
- [ ]  Support other citation formats
- [ ]  Support the case when users want to generate a list with articles which does not have doi

See the [open issues](https://github.com/haruchannn/reftion/issues) for a full list of proposed features (and known issues).

<p align="right">(<a href="#readme-top">back to top</a>)</p>



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

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- LICENSE -->
## License

Distributed under the MIT License. See `LICENSE.txt` for more information.

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- CONTACT -->
## Contact

haruchannn  - reftioncs@gmail.com

Project Link: [https://github.com/haruchannn/reftion](https://github.com/haruchannn/reftion)

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- ACKNOWLEDGMENTS -->
## Acknowledgments

* [CiteAs (API to generate citation)](https://citeas.org/api)
* [Notion API](https://developers.notion.com/)

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/haruchannn/reftion.svg?style=for-the-badge
[contributors-url]: https://github.com/haruchannn/reftion/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/haruchannn/reftion.svg?style=for-the-badge
[forks-url]: https://github.com/haruchannn/reftion/network/members
[stars-shield]: https://img.shields.io/github/stars/haruchannn/reftion.svg?style=for-the-badge
[stars-url]: https://github.com/haruchannn/reftion/stargazers
[issues-shield]: https://img.shields.io/github/issues/haruchannn/reftion.svg?style=for-the-badge
[issues-url]: https://github.com/haruchannn/reftion/issues
[license-shield]: https://img.shields.io/github/license/haruchannn/reftion.svg?style=for-the-badge
[license-url]: https://github.com/haruchannn/reftion/blob/master/LICENSE.txt
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://linkedin.com/in/linkedin_username
[product-screenshot]: images/screenshot.png
[Next.js]: https://img.shields.io/badge/next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white
[Next-url]: https://nextjs.org/
[React.js]: https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB
[React-url]: https://reactjs.org/
[Vue.js]: https://img.shields.io/badge/Vue.js-35495E?style=for-the-badge&logo=vuedotjs&logoColor=4FC08D
[Vue-url]: https://vuejs.org/
[Angular.io]: https://img.shields.io/badge/Angular-DD0031?style=for-the-badge&logo=angular&logoColor=white
[Angular-url]: https://angular.io/
[Svelte.dev]: https://img.shields.io/badge/Svelte-4A4A55?style=for-the-badge&logo=svelte&logoColor=FF3E00
[Svelte-url]: https://svelte.dev/
[Laravel.com]: https://img.shields.io/badge/Laravel-FF2D20?style=for-the-badge&logo=laravel&logoColor=white
[Laravel-url]: https://laravel.com
[Bootstrap.com]: https://img.shields.io/badge/Bootstrap-563D7C?style=for-the-badge&logo=bootstrap&logoColor=white
[Bootstrap-url]: https://getbootstrap.com
[JQuery.com]: https://img.shields.io/badge/jQuery-0769AD?style=for-the-badge&logo=jquery&logoColor=white
[JQuery-url]: https://jquery.com 
