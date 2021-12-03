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

This project aims to use real-time data of people's sentiments from social networks to create a Legitimacy Index for International Institutions like the UN. The goal is to be able to use the index in various other studies.

### Built With
The above project uses the following works by other authors.

* [Twint](https://github.com/twintproject/twint)
* [VADER](https://github.com/cjhutto/vaderSentiment)

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- GETTING STARTED -->
## Getting Started

The following code has been made into a PyPi package for ease of use.

### Prerequisites

Prerequisites should be automatically downloaded, but in case it isn't use:

* Manual Setup (Do not recommend)
  ```sh
  pip install -r requirements.txt
  ```
* Install Vader Lexicon
  ```sh
  pip install nltk
  import nltk
  nltk.download('vader_lexicon')
  ```
### Installation

* Install the package
   ```sh
   pip install emiliaworks
   ```
<p align="right">(<a href="#top">back to top</a>)</p>


<!-- USAGE EXAMPLES -->
## Usage

```sh
from emiliaworks import emilia
a = emilia.custom("UN","2021-11-01","2021-11-21")
a.get_tweets()
a.clean_data()
a.siamod()
df = a.clean_df
print(df)
```
<p align="right">(<a href="#top">back to top</a>)</p>

<!-- LICENSE -->
## License

Distributed under the MIT License. See `LICENSE.txt` for more information.

<p align="right">(<a href="#top">back to top</a>)</p>

<!-- ACKNOWLEDGMENTS -->
## Acknowledgments
* Dr. Durgesh Chandra Pathak - Economics Professor @ BITS Hyderabad
<p align="right">(<a href="#top">back to top</a>)</p>
