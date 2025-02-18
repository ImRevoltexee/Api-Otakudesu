# UnOfficial Otakudesu API 👀🔥

---

[![GitHub ariear](https://github.com/ariear.png?s=100)](https://github.com/ariear)  
**Special Credit To:** [ariear](https://github.com/ariear)

<p align="center">
  <img src="https://otakudesu.cloud/wp-content/uploads/2019/08/otakudesu.png" alt="Otakudesu" />
</p>

<p align="center">
  <b>I made this API using the technologies below</b>
</p>

<p align="center">
  <a href="https://hono.dev/?kawaii=true">
    <img src="https://hono.dev/images/logo-small.png" width="60px" alt="Hono" />
  </a>
  <a href="https://cheerio.js.org/">
    <img src="https://cheerio.js.org/img/orange-c.svg" width="60px" alt="Cheerio" />
  </a>
</p>

---

An unofficial API from Otakudesu. I built this API using web scraping techniques with the help of the [Cheerio](https://cheerio.js.org/) library. I hope this helps you develop awesome anime streaming applications! 😉

---

- [UnOfficial Otakudesu API 👀🔥](#unofficial-otakudesu-api-)
  - [Documentation](#documentation)
  - [Installation](#installation)
  - [Let's Contribute](#lets-contribute)

## Documentation

### Parameters
| Parameter | Example | Description |
|-----------|---------|-------------|
| `:page`   | `1`     | The page number for pagination |
| `:slug`   | `kusuriya-hitorigoto-sub-indo` or `knh-batch-sub-indo` | The slug for the anime title or batch download |
| `:eps`    | `knh-episode-1-sub-indo` | The slug for a specific anime episode |
| `?q`      | `yahaha` | Query parameter for searching anime by title |

### Endpoints
| Endpoint | Method | Example | Description |
|----------|--------|---------|-------------|
| `/api/home` | GET | `/api/home` | Retrieve a list of ongoing and finished anime |
| `/api/anime-list` | GET | `/api/anime-list` | Retrieve all anime in alphabetical order |
| `/api/anime/:slug` | GET | `/api/anime/kusuriya-hitorigoto-sub-indo` | Retrieve anime details |
| `/api/anime/episode/:eps` | GET | `/api/anime/episode/knh-episode-1-sub-indo` | Retrieve episode details including streaming and download links |
| `/api/anime/batch/:slug` | GET | `/api/anime/batch/knh-batch-sub-indo` | Retrieve download link for anime batch |
| `/api/anime/search` | GET | `/api/anime/search?q=yahahah` | Search for anime by title |
| `/api/release-schedule` | GET | `/api/release-schedule` | Retrieve anime release schedule |
| `/api/genre-list` | GET | `/api/genre-list` | Retrieve list of genres |
| `/api/ongoing-anime` | GET | `/api/ongoing-anime` | Retrieve a list of ongoing anime |
| `/api/complete-anime` | GET | `/api/complete-anime` | Retrieve a list of finished anime |

## Installation

You can run this API using Docker:

[![Docker Image](https://img.shields.io/badge/Docker-2CA5E0?style=for-the-badge&logo=docker&logoColor=white)](https://hub.docker.com/r/arieakbarull/otakudesu-api)

#### OR

Clone this repository:

```sh
git clone https://github.com/ariear/otakudesu-api.git
