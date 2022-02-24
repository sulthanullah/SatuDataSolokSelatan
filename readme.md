<div id="top"></div>
<!--
*** Thanks for checking out the Best Sulthanullah. If you have a suggestion
*** that would make this better, please fork the repo and create a pull request
*** or simply open an issue with the tag "enhancement".
*** Don't forget to give the project a star!
*** Thanks again! Now go create something AMAZING! :D
-->


<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="http://satudata.solselkab.go.id">
    <img src="images/Lambang_Kabupaten_Solok_Selatan.png" alt="Logo" width="80" height="80">
  </a>

  <h3 align="center">Satu Data Kabupaten Solok Selatan</h3>

  <p align="center">
    An awesome Projects!
    <br />
    <a href="#"><strong>Explore the docs »</strong></a>
    <br />
    <br />
    <a href="http://satudata.solselkab.go.id">View Demo</a>
    ·
    <a href="#">Report Bug</a>
    ·
    <a href="#">Request Feature</a>
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

[![Product Name Screen Shot][product-screenshot]](https://satudata.solselkab.go.id)

Comprehensive Knowledge Archive Network (CKAN) adalah perangkat lunak open source untuk portal open data, CMS yang dapat membantu kita dalam mengelola dan menerbitkan sekumpulan data. CKAN digunakan oleh pemerintah pusat dan daerah, lembaga penelitian, dan organisasi lain untuk mempublikasikan data.

Contoh pemakaian di Indonesia yaitu Satu Data Indonesia (SDI) yang merupakan kebijakan tata kelola data pemerintah dengan tujuan untuk menciptakan data berkualitas, mudah diakses, dan dapat dibagipakaikan antar instansi pusat dan daerah. Kebijakan SDI ini tertuang dalam Peraturan Presiden No. 39 Tahun 2019 tentang Satu Data Indonesia. Melalu SDI, seluruh data pemerintah dan data instansi lain yang terkait dapat bermuara di Portal Satu Data Indonesia (data.go.id). 


<p align="right">(<a href="#top">back to top</a>)</p>



### Tech Stack

CKAN dikembangkan dengan menggunakan bahasa pemrograman Python sebagai backend, JavaScript sebagai frontend, database PostgreSQL dan search engine Solr. CKAN memungkinkan untuk ditambahkan ekstensi atau fitur tambahan karena memakai arsitektur modular. Selain itu CKAN juga memiliki fitur API.

* [Python](https://www.python.org/downloads/)
* [PostgreSQL](https://www.jetbrains.com/datagrip/features/?source=google&medium=cpc&campaign=15034928131&gclid=Cj0KCQiA09eQBhCxARIsAAYRiym4GpmfEQVKxJR41HXWfTV4lA1QN0q9-SPzHS1RVQN4CAPbVjqkv4EaArViEALw_wcB)
* [Solr](https://en.wikipedia.org/wiki/Apache_Solr)
* [Ubuntu](https://ubuntu.com)
* [Docker](http://docker.com)
* [Proxmox](https://www.proxmox.com/en/)

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- GETTING STARTED -->
## Getting Started

* Install Proxmox
* Install VM Ubuntu
* Install Docker
* Git Clone CKAN


### Prerequisites

- 👨‍💻 &nbsp; Step One
* Update Ubuntu
  ```sh
  apt update
  ```
* Upgrade Ubuntu
  ```sh
  apt upgrade -y
  ```
* Install alat bantu 
  ```sh
  apt-get install python3 python3-setuptools docker.io -y
  ```
* Install pip3
  ```sh
  apt-get install python3-pip -y
  ```
* Install curl
  ```sh
  apt-get install curl -y
  ```
  
### Installation

_Langkah - Langkah Install CKAN In Proxmox._

1. Upgrade docker-compose version
     ```sh
   sudo apt-get remove docker-compose
   ```
      ```sh
   sudo curl -L "https://github.com/docker/compose/releases/download/1.23.2/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
   ```
     ```sh
   sudo chmod +x /usr/local/bin/docker-compose
   ```
      ```sh
   sudo ln -s /usr/local/bin/docker-compose /usr/bin/docker-compose
   ```
2. Clone the repo
   ```sh
   git clone https://github.com/ckan/ckan.git
   ```
3. Install
   ```sh
   git checkout tags/ckan-2.9.0
   ```
      ```sh
   cd /ckan/contrib/docker
   ```
      ```sh
   cp -rp .env.template .env
   ```
      ```sh
     docker-compose up -d --build
   ```
4. Enter your API in `config.js`
   ```js
   const API_KEY = 'ENTER YOUR API';
   ```

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- USAGE EXAMPLES -->
## Usage

Use this space to show useful examples of how a project can be used. Additional screenshots, code examples and demos work well in this space. You may also link to more resources.

_For more examples, please refer to the [Documentation](https://example.com)_

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- ROADMAP -->
## Roadmap

- [x] Add Changelog
- [x] Add back to top links
- [ ] Add Additional Templates w/ Examples
- [ ] Add "components" document to easily copy & paste sections of the readme
- [ ] Multi-language Support
    - [ ] Chinese
    - [ ] Spanish

See the [open issues](https://github.com/othneildrew/Best-README-Template/issues) for a full list of proposed features (and known issues).

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

Your Name - [@your_twitter](https://twitter.com/your_username) - email@example.com

Project Link: [https://github.com/your_username/repo_name](https://github.com/your_username/repo_name)

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- ACKNOWLEDGMENTS -->
## Acknowledgments

Use this space to list resources you find helpful and would like to give credit to. I've included a few of my favorites to kick things off!

* [Choose an Open Source License](https://choosealicense.com)
* [GitHub Emoji Cheat Sheet](https://www.webpagefx.com/tools/emoji-cheat-sheet)
* [Malven's Flexbox Cheatsheet](https://flexbox.malven.co/)
* [Malven's Grid Cheatsheet](https://grid.malven.co/)
* [Img Shields](https://shields.io)
* [GitHub Pages](https://pages.github.com)
* [Font Awesome](https://fontawesome.com)
* [React Icons](https://react-icons.github.io/react-icons/search)

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/othneildrew/Best-README-Template.svg?style=for-the-badge
[contributors-url]: https://github.com/othneildrew/Best-README-Template/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/othneildrew/Best-README-Template.svg?style=for-the-badge
[forks-url]: https://github.com/othneildrew/Best-README-Template/network/members
[stars-shield]: https://img.shields.io/github/stars/othneildrew/Best-README-Template.svg?style=for-the-badge
[stars-url]: https://github.com/othneildrew/Best-README-Template/stargazers
[issues-shield]: https://img.shields.io/github/issues/othneildrew/Best-README-Template.svg?style=for-the-badge
[issues-url]: https://github.com/othneildrew/Best-README-Template/issues
[license-shield]: https://img.shields.io/github/license/othneildrew/Best-README-Template.svg?style=for-the-badge
[license-url]: https://github.com/othneildrew/Best-README-Template/blob/master/LICENSE.txt
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://linkedin.com/in/othneildrew
[product-screenshot]: images/screenshot.png
