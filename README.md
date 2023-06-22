<div align="center">
  <a href="#">
    <img src="https://graph.org/file/f04fb6b4cd450eaf3ec60.jpg" alt="Logo">
  </a>

  <h1 align="center">Z-Anime</h1>

  <p align="center">
    <h3>An unoffitial <a href="sanji.to">zoro.to </a>fetcher NPM package </h3>
    <br />
    <a href="#table-of-contents"><strong>Explore the docs »</strong></a>
    <br />
    <br />
    <a href="#get-trending-anime-list">View Code Example</a>
    ·
    <a href="https://github.com/FantoX001/Z-Anime/issues">Report a Bug</a>
    ·
    <a href="https://github.com/FantoX001/Z-Anime/issues">Request a Feature</a>
  </p>
</div>

## About Z-Anime

Sometimes while creating and **anime information** website or **anime news website**, we require some data so this NPM pacakge will help you fetch data from <a href="sanji.to">zoro.to </a> and return as a **JSON** with the power of web scraping.

**Features:**
- [x] Lite weight, fast ( Execution time: 0.05ms - 0.5s average ) and realtime scraping.
- [x] Written on simple **ES5** JavaScript which ensures compatibility.
- [x] Open Source MIT license.

**Advantages:**
- [x] Saves your time and money of creating a whole anime database yourself.
- [x] Requirs no additional configuration from user's end.
- [x] Contains all featues of <a href="sanji.to">zoro.to </a> website.

**Limitations:**
- [ ] No anime video **play/download** feature to avoid IP ban.
- [ ] Can take upto **1.25s** in certain functions to preform some heavy scraping ( Ex: Anime details functionality is heavy ).
- [x] Let me know if you found anything else.


<a name="table-of-contents"></a>

## Table of Contents

<ol>
  <li>Getting started</li>
  <ul>
    <li><a href="#installation">Installation</a></li> <br />
  </ul>
  <li>Usage</li>
  <ul>
    <li><a href="#get-trending-anime-list">Get Trending Animes List</a></li>
    <li><a href="#get-spotlight-animes-list">Get Spotlight Animes List</a></li>
    <li><a href="#get-recently-updated-animes-list">Get Recently Updated Animes List</a></li>
    <li><a href="#get-recently-added-animes-list">Get Recently Added Animes List</a></li>
    <li><a href="#get-currently-airing-animes-list">Get Currently Airing Animes List</a></li>
    <li><a href="#get-most-popular-animes-list">Get Most Popular Animes List</a></li>
    <li><a href="#get-most-favourite-animes-list">Get Most Favourite Animes List</a></li>
    <li><a href="#get-completed-animes-list">Get Completed Animes List</a></li>
    <li><a href="#search-an-anime-genere">Search an Anime Genre</a></li>
    <li><a href="#search-an-anime">Search an Anime</a></li>
    <li><a href="#get-full-details-of-any-anime">Get Full Details of any Anime</a></li>
    <li><a href="#get-anime-movies-list">Get Anime Movies List</a></li>
    <li><a href="#get-ona-animes-list">Get ONA Animes List</a></li>
    <li><a href="#get-ova-animes-list">Get OVA Animes List</a></li>
    <li><a href="#get-tv-animes-list">Get TV Animes List</a></li>
    <li><a href="#get-specials-animes-list">Get Specials Animes List</a></li>
    <li><a href="#get-dubbed-animes-list">Get Dubbed Animes List</a></li>
    <li><a href="#get-subbed-animes-list">Get Subbed Animes List</a></li> <br />
</ul>
  <li>Types of Outputs</li>
  <ul>
    <li><a href="#search-output">Search Output</a></li>
    <li><a href="#anime-details">Anime Details</a></li>
    <li><a href="#anime-pages-output">Anime Pages Output</a></li> <br />
  </ul>
</ol>


<!-- GETTING STARTED -->
## Getting Started

This is how you can setup Z-Anime.

### Installation

Using NPM:

```sh
npm install z-anime
```

Using YARN:

```sh
yarn add z-anime
```


## Usage

### Get Trending anime list:

* Use `trending()` function to get top 10 trending anime list of Zoro.to.

```JS
const anime = require("z-anime");

(async () => {
  
  const trending = await anime.trending(); // It will return top 10 trending anime.
  
  console.log(trending);
})();
```

### Get Spotlight anime list:

* Use `spotlight()` function to get top 12 spotlight anime list of Zoro.to.

```JS
const anime = require("z-anime");

(async () => {
  
  const spotlight = await anime.spotlight();  // It will return top 12 spotlight anime.
  
  console.log(spotlight);
})();
```

### Get Recently Updated anime list:

* Use `updated()` function to get Recently Updated anime list of page 1 of Zoro.to.
* You can get a particular page number of Recently Updated by using `updated(3)` ( To get Recently Updated page 3 ).

```JS
const anime = require("z-anime");

(async () => {
  
  const data1 = await anime.updated(); // It will return Recently Updated anime page 1
  
  const data2 = await anime.updated(3); // It will return Recently Updated anime page 3
  
  console.log(data1);
  console.log(data2);
})();
```

### Get Recently Added anime list:

* Use `latest()` function to get Recently Added anime list of page 1 of Zoro.to.
* You can get a particular page number of Recently Added by using `updated(3)` ( To get Recently Added page 3 ).

```JS
const anime = require("z-anime");

(async () => {
  
  const data1 = await anime.latest(); // It will return Recently Added anime page 1
  
  const data2 = await anime.latest(3); // It will return Recently Added anime page 3
  
  console.log(data1);
  console.log(data2);
})();
```

### Get Top Airing anime list:

* Use `airing()` or `ongoing()` or `topAiring()` function to get Top Airing  anime list of page 1 of Zoro.to.
* You can get a particular page number of Top Airing by using `airing(3)` ( To get Top Airing page 3 ).

```JS
const anime = require("z-anime");

(async () => {
  
  const data1 = await anime.airing(); // It will return Top Airing anime page 1
  
  const data2 = await anime.airing(3); // It will return Top Airing anime page 3
  
  console.log(data1);
  console.log(data2);
})();
```

### Get Most Popular anime list:

* Use `popular()` function to get Most Popular anime list of page 1 of Zoro.to.
* You can get a particular page number of Most Popular anime by using `popular(3)` ( To get Most Popular page 3 ).

```JS
const anime = require("z-anime");

(async () => {
  
  const data1 = await anime.popular(); // It will return Most Popular anime page 1
  
  const data2 = await anime.popular(3); // It will return Most Popular anime page 3
  
  console.log(data1);
  console.log(data2);
})();
```

### Get Most Favourite anime list:

* Use `favourite()` or `mostFavourite()` function to get Most Favourite anime list of page 1 of Zoro.to.
* You can get a particular page number of Most Favourite anime by using `popular(3)` ( To get Most Popular page 3 ).

```JS
const anime = require("z-anime");

(async () => {
  
  const data1 = await anime.favourite(); // It will return Most Favourite anime page 1
  
  const data2 = await anime.favourite(3); // It will return Most Favourite anime page 3
  
  console.log(data1);
  console.log(data2);
})();
```

### Get Completed anime list:

* Use `completed()` function to get Completed anime list of page 1 of Zoro.to.
* You can get a particular page number of Completed anime by using `completed(3)` ( To get Completed page 3 ).

```JS
const anime = require("z-anime");

(async () => {
  
  const data1 = await anime.completed(); // It will return Completed anime page 1
  
  const data2 = await anime.completed(3); // It will return Completed anime page 3
  
  console.log(data1);
  console.log(data2);
})();
```

### Search any Genere:

* Use `genere("Action", 3)` function to get list of Action genere animes on page 3 of Zoro.to.

```JS
const anime = require("z-anime");

(async () => {
  
  const action_animes = await anime.genere("Action", 1); // It will return Action genere animes on page 1 of Zoro.to.
  
  console.log(action_animes);
})();
```

### Search any Anime:

* Use `search("anime name")` function to search on Zoro.to and get all search results.

```JS
const anime = require("z-anime");

(async () => {
  
  const results = await anime.search("high school dxd"); // It will return all search results from Zoro.to
  
  console.log(results);
})();
```

### Get full details of any anime:

* Use `details("anime name")` function to search and get full details of tht anime.

```JS
const anime = require("z-anime");

(async () => {
  
  const anime_details = await anime.details("tonikawa"); // It will return full anime details from Zoro.to
  
  console.log(anime_details);
})();
```

### Get Movies list:

* Use `movies()` function to get Movies list of page 1 of Zoro.to.
* You can get a particular page number of Movies by using `movies(3)` ( To get Movies page 3 ).

```JS
const anime = require("z-anime");

(async () => {
  
  const data1 = await anime.movies(); // It will return Top Airing anime page 1
  
  const data2 = await anime.movies(3); // It will return Top Airing anime page 3
  
  console.log(data1);
  console.log(data2);
})();
```

### Get ONA list:

* Use `ona()` function to get ONA list of page 1 of Zoro.to.
* You can get a particular page number of ONA by using `ona(3)` ( To get ONA page 3 ).

```JS
const anime = require("z-anime");

(async () => {
  
  const data1 = await anime.ona(); // It will return ONA anime page 1
  
  const data2 = await anime.ona(3); // It will return ONA anime page 3
  
  console.log(data1);
  console.log(data2);
})();
```

### Get OVA list:

* Use `ova()` function to get ONA list of page 1 of Zoro.to.
* You can get a particular page number of OVA by using `ona(3)` ( To get OVA page 3 ).

```JS
const anime = require("z-anime");

(async () => {
  
  const data1 = await anime.ova(); // It will return OVA anime page 1
  
  const data2 = await anime.ova(3); // It will return OVA anime page 3
  
  console.log(data1);
  console.log(data2);
})();
```

### Get TV list:

* Use `tv()` function to get ONA list of page 1 of Zoro.to.
* You can get a particular page number of TV animes by using `tv(3)` ( To get Movies page 3 ).

```JS
const anime = require("z-anime");

(async () => {
  
  const data1 = await anime.tv(); // It will return tv anime page 1
  
  const data2 = await anime.tv(3); // It will return tv anime page 3
  
  console.log(data1);
  console.log(data2);
})()
```

### Get Specials list:

* Use `specials()` function to get Specials list of page 1 of Zoro.to.
* You can get a particular page number of Specials by using `specials(3)` ( To get Movies page 3 ).

```JS
const anime = require("z-anime");

(async () => {
  
  const data1 = await anime.specials(); // It will return Specials anime page 1
  
  const data2 = await anime.specials(3); // It will return Specials anime page 3
  
  console.log(data1);
  console.log(data2);
})();
```

### Get Dubbed Anime list:

* Use `dubbed()` function to get Dubbed Anime list of page 1 of Zoro.to.
* You can get a particular page number of Dubbed Anime by using `specials(3)` ( To get Dubbed Anime page 3 ).

```JS
const anime = require("z-anime");

(async () => {
  
  const data1 = await anime.dubbed(); // It will return Dubbed Anime page 1
  
  const data2 = await anime.dubbed(3); // It will return Dubbed Anime page 3
  
  console.log(data1);
  console.log(data2);
})();
```

### Get Subbed Anime list:

* Use `subbed()` function to get Dubbed Anime list of page 1 of Zoro.to.
* You can get a particular page number of Dubbed Anime by using `specials(3)` ( To get Subbed Anime page 3 ).

```JS
const anime = require("z-anime");

(async () => {
  
  const data1 = await anime.subbed(); // It will return Subbed Anime page 1
  
  const data2 = await anime.subbed(3); // It will return Subbed Anime page 3
  
  console.log(data1);
  console.log(data2);
})();
```
