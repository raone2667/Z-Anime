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
    <li><a href="#anime-pages-output">Anime List Output</a></li>
    <li><a href="#search-output">Search Output</a></li>
    <li><a href="#anime-details">Anime Details</a></li> <br />
    
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

### Output:

<details>
  <summary>View Output</summary>

<br />

  ```js
  [
  {
    index: '1',
    title: 'One Piece',
    image: 'https://img.zorores.com/_r/300x400/100/54/90/5490cb32786d4f7fef0f40d7266df532/5490cb32786d4f7fef0f40d7266df532.jpg',
    url: 'https://sanji.to/one-piece-100'
  },
  {
    index: '2',
    title: 'Demon Slayer: Kimetsu no Yaiba Swordsmith Village Arc',
    image: 'https://img.zorores.com/_r/300x400/100/db/2f/db2f3ce7b9cab7fdc160b005bffb899a/db2f3ce7b9cab7fdc160b005bffb899a.png',
    url: 'https://sanji.to/demon-slayer-kimetsu-no-yaiba-swordsmith-village-arc-18056'
  },
  {
    index: '3',
    title: 'My Star',
    image: 'https://img.zorores.com/_r/300x400/100/99/59/995928d6858977d66f7da57e0e0af08a/995928d6858977d66f7da57e0e0af08a.jpg',
    url: 'https://sanji.to/my-star-18330'
  },
  {
    index: '4',
    title: 'I Got a Cheat Skill in Another World and Became Unrivaled in The Real World, Too',
    image: 'https://img.zorores.com/_r/300x400/100/0a/d5/0ad5356f28ee75bccfde8b69ea6a5e54/0ad5356f28ee75bccfde8b69ea6a5e54.jpg',
    url: 'https://sanji.to/i-got-a-cheat-skill-in-another-world-and-became-unrivaled-in-the-real-world-too-18343'
  },
  {
    index: '5',
    title: 'Mashle: Magic and Muscles',
    image: 'https://img.zorores.com/_r/300x400/100/9f/af/9faf29fb396c436d19ed83fa82a31e2f/9faf29fb396c436d19ed83fa82a31e2f.jpg',
    url: 'https://sanji.to/mashle-magic-and-muscles-18339'
  },
  {
    index: '6',
    title: "Hell's Paradise",
    image: 'https://img.zorores.com/_r/300x400/100/5f/d0/5fd0a7d4f0e1a9088c85bc0dcb2f176a/5fd0a7d4f0e1a9088c85bc0dcb2f176a.png',
    url: 'https://sanji.to/hells-paradise-18332'
  },
  {
    index: '7',
    title: 'Dr. Stone: New World',
    image: 'https://img.zorores.com/_r/300x400/100/0c/ab/0cab1ee2bbe1a4def0790121df2c1fc7/0cab1ee2bbe1a4def0790121df2c1fc7.jpg',
    url: 'https://sanji.to/dr-stone-new-world-17725'
  },
  {
    index: '8',
    title: 'Blue Lock',
    image: 'https://img.zorores.com/_r/300x400/100/fc/ed/fced51e392ffd80041b3a1581ba7de2f/fced51e392ffd80041b3a1581ba7de2f.jpg',
    url: 'https://sanji.to/blue-lock-17889'
  },
  {
    index: '9',
    title: 'My Hero Academia Season 6',
    image: 'https://img.zorores.com/_r/300x400/100/20/b7/20b7580c1abdf45a6eaf4826fc9fdf33/20b7580c1abdf45a6eaf4826fc9fdf33.jpg',
    url: 'https://sanji.to/my-hero-academia-season-6-18154'
  },
  {
    index: '10',
    title: 'Tokyo Revengers: Christmas Showdown',
    image: 'https://img.zorores.com/_r/300x400/100/fb/66/fb663be9a427cc4c9556a5a124b060e8/fb663be9a427cc4c9556a5a124b060e8.jpg',
    url: 'https://sanji.to/tokyo-revengers-christmas-showdown-18244'
  }
]
  ```

<br />
  
</details>

<br />

### Get Spotlight anime list:

* Use `spotlight()` function to get top 12 spotlight anime list of Zoro.to.

```JS
const anime = require("z-anime");

(async () => {
  
  const spotlight = await anime.spotlight();  // It will return top 12 spotlight anime.
  
  console.log(spotlight);
})();
```

### Output:

<details>
  <summary>View Output</summary>

  <br />

  ```js
  [
  {
    index: '1',
    image: 'https://img.zorores.com/_r/1366x768/100/69/dd/69dd49d8ad5033c8f649b67e9c3bfef9/69dd49d8ad5033c8f649b67e9c3bfef9.jpg',
    title: 'Skip and Loafer',
    release: 'Apr 4, 2023',
    duration: '23m',
    quality: 'HD',
    cc: '12',
    episodes: '12',
    description: 'In order to pursue her dream of bringing positive changes to Japan, Mitsumi Iwakura leaves her countryside town to attend a prestigious high school in the hustle and bustle of Tokyo. As she has already mapped a clear life plan, she has absolute confidence that there will be zero mishaps from then onwards.Despite her ambitious promise, the country girl ends up running late on the first day when she gets lost on her way to school. Fortunately, she meets a fellow first-year student, Sousuke Shima, who is in the same situation and offers to go with her. They eventually make it to school, but the misfortunes do not end there, as Mitsumi leaves an unfavorable first impression in front of her classmates.',
    url: 'https://sanji.to/watch/skip-and-loafer-18351'
  },
  {
    index: '2',
    image: 'https://img.zorores.com/_r/1366x768/100/ff/b6/ffb6981af9cacd38b190c2d878a4405a/ffb6981af9cacd38b190c2d878a4405a.jpg',
    title: 'I Got a Cheat Skill in Another World and Became Unrivaled in The Real World, Too',
    release: 'Apr 7, 2023',
    duration: '24m',
    quality: 'HD',
    cc: '12',
    episodes: '13',
    description: 'All his life, Yuuya Tenjou has been the subject of resentment and contempt from everyone around him, even from his parents. To make matters worse, his grandfather—the only person who ever showed him affection—suddenly dies, leaving Yuuya truly alone.Despite facing many adversities, Yuuya does what he can to offer kindness to those who need it—but even the most good-natured people can only tolerate so much abuse. Just when he reaches his breaking point, a flicker of hope appears in the form of a hidden door in his bathroom.',
    url: 'https://sanji.to/watch/i-got-a-cheat-skill-in-another-world-and-became-unrivaled-in-the-real-world-too-18343'
  },
  {
    index: '3',
    image: 'https://img.zorores.com/_r/1366x768/100/e4/05/e4055651560b12f4f735657be1dc001f/e4055651560b12f4f735657be1dc001f.jpg',
    title: "Hell's Paradise",
    release: 'Apr 1, 2023',
    duration: '22m',
    quality: 'HD',
    cc: '11',
    episodes: '13',
    description: "Gabimaru the Hollow, a ninja of Iwagakure Village known for being cold and emotionless, was set up by his fellow ninja and is now on death row. Tired of killing and betrayal, he wants to die. However, no method of execution works on him because as much as the seemingly apathetic Gabimaru refuses to admit it, he does have a reason to live. He wants to return to his wife, who was the reason why he softened up and failed to be an effective assassin. Thus, he refuses to die.Asaemon the Decapitator, a famous executioner, sees this and has a proposal for the ninja. He wants Gabimaru to join an expedition to an island south of Japan in search of the elixir of life in exchange for a full pardon by the Shogunate. However, this island isn't a normal island: it's believed to be Paradise.",
    url: 'https://sanji.to/watch/hells-paradise-18332'
  },
  {
    index: '4',
    image: 'https://img.zorores.com/_r/1366x768/100/76/9a/769aa036cdb4a575b43b44ef2ad625bf/769aa036cdb4a575b43b44ef2ad625bf.jpg',
    title: 'Edens Zero 2nd Season',
    release: 'Mar 11, 2023',
    duration: '23m',
    quality: 'HD',
    cc: '12',
    episodes: 'Not declared yet',
    description: "Now in possession of the Edens Zero, Shiki Granbell has gathered the Four Shining Stars. With the help of his new friends, Shiki will be able to breach Dragonfall—the border of the Sakura Cosmos swarming with mechanical dragons. Once that is achieved, he can continue his quest to find the goddess Mother.Before the Edens Zero crew can advance their journey, they notice a mysterious warship following them. Upon learning that the ship—the Belial Gore—belongs to Drakken Joe, Shiki and his crew attempt to infiltrate it, intent on figuring out why the Dark Alchemist is after them. In the process, the Edens Zero is taken hostage by Drakken's subordinates.",
    url: 'https://sanji.to/watch/edens-zero-2nd-season-18331'
  },
  {
    index: '5',
    image: 'https://img.zorores.com/_r/1366x768/100/b7/da/b7da3cbb4e82c692f724b73848326dca/b7da3cbb4e82c692f724b73848326dca.jpg',
    title: 'Loving Yamada at Lv999',
    release: 'Apr 2, 2023',
    duration: '23m',
    quality: 'HD',
    cc: '12',
    episodes: '13',
    description: "After her boyfriend breaks up with her for another girl, college student Akane Kinoshita wrestles with a broken heart and the memories he left behind. Loading up Forest of Savior, the MMO they used to play together, she forms a plan to get back at her ex-boyfriend through an in-person event for the game. In the process, she runs into someone unexpected: Akito Yamada, a gaming legend who just happens to be her guildmate.Desperate for support, Akane ropes the asocial Yamada into helping with her scheme and lending her a shoulder to cry on. The differences between Akane and Yamada soon become apparent as they spend time together, yet they cannot help but notice each other's inner qualities. As the two gain more experience with one another in and out of the game, their tentative acquaintance may level up in a way neither expects.",
    url: 'https://sanji.to/watch/loving-yamada-at-lv999-18341'
  },
  {
    index: '6',
    image: 'https://img.zorores.com/_r/1366x768/100/be/85/be855285814752aa2def6fcaba6f3269/be855285814752aa2def6fcaba6f3269.jpg',
    title: 'Tonikawa: Over The Moon For You: 2nd Season',
    release: 'Apr 8, 2023',
    duration: '23m',
    quality: 'HD',
    cc: '11',
    episodes: 'Not declared yet',
    description: "In the wake of their first home burning down, Nasa and Tsukasa Yuzaki are seeking temporary shelter at the Arisugawas' bathhouse. Though they have only been married for a short time, their relationship has only become sweeter by the day. Nasa is determined to spend as much time with his wife as possible, basking in the happiness of their marriage.The newlyweds find new ways to explore their relationship. From adopting a cat, going to an amusement park, and even watching an impromptu romantic comedy featuring Nasa's former teacher, every day is a new experience. But while Tsukasa continues to meet the people in Nasa's life, Nasa has yet to meet more of Tsukasa's family. Though they appear to be the picture-perfect couple to everyone around them, Nasa begins to wonder if he will ever learn more about his wife's mysterious past.",
    url: 'https://sanji.to/watch/tonikawa-over-the-moon-for-you-2nd-season-18226'
  },
  {
    index: '7',
    image: 'https://img.zorores.com/_r/1366x768/100/7c/d5/7cd514ee5521d04d45acfcdd0721f2f2/7cd514ee5521d04d45acfcdd0721f2f2.jpg',
    title: 'Black Clover: Sword of the Wizard King',
    release: 'Jun 16, 2023',
    duration: '1h 50m',
    quality: 'HD',
    cc: '1',
    episodes: 'Not declared yet',
    description: 'As a lionhearted boy who can’t wield magic strives for the title of Wizard King, four banished Wizard Kings of yore return to crush the Clover Kingdom.',
    url: 'https://sanji.to/watch/black-clover-sword-of-the-wizard-king-17752'
  },
  {
    index: '8',
    image: 'https://img.zorores.com/_r/1366x768/100/57/f8/57f8283354fe92f23fc216a53e7368d0/57f8283354fe92f23fc216a53e7368d0.jpg',
    title: 'The Legendary Hero Is Dead!',
    release: 'Apr 7, 2023',
    duration: '23m',
    quality: 'HD',
    cc: '11',
    episodes: '12',
    description: "Far to the north of the world lies Hell's Gate, a portal formerly used by the Demon Lord to invade the human realm. Thanks to the legendary hero Shion Bladearts, wielder of Excalibur, and his loyal band of companions, the Gate was sealed off and the demonic threat was vanquished.  Unfortunately, the seal was incomplete and has begun to weaken, allowing the demons to once again begin their attack. Worried about the safety of his village, selfish and perverted farmer Touka Scott dig pitfalls to defend against the demons. But fear not, for Shion is on his way to reseal Hell's Gate and save humanity!  Or at least he was, because the legendary hero is dead, having fallen into one of the pitfalls Touka dug. Luckily, dealing with the dead is the specialty of necromancer Anri Haynesworth. While she can't revive him, Anri can at least salvage their quest by forcing Touka's soul into Shion's rotting body and dragging him along to Hell's Gate in Shion's place. Not wanting to be left behind, Touka's childhood friend Yuna Yunis tags along. Together, the three of them set out as what just might be the most unsuitable party to ever try to save the world!",
    url: 'https://sanji.to/watch/the-legendary-hero-is-dead-18354'
  },
  {
    index: '9',
    image: 'https://img.zorores.com/_r/1366x768/100/ba/a2/baa2cf51574e886b03140a0c023dc849/baa2cf51574e886b03140a0c023dc849.jpg',
    title: "The Ancient Magus' Bride Season 2",
    release: 'Apr 6, 2023',
    duration: '23m',
    quality: 'HD',
    cc: '11',
    episodes: '12',
    description: "Apprentice mage Chise Hatori is invited to enroll at the College, a prestigious learning institution for sorcerers, to examine and look for a way to remove the curses she bears. Despite her groom Elias Ainsworth's reluctance, Chise accepts the proposal, as she believes attending the school might help her minimize her self-sacrificing tendencies.From the get-go, Chise grabs the attention of her classmates and professors alike, who have never seen a mage in action before. However, there is a sinister plot brewing behind the College's back, and the young mage will have to determine who is friend or foe in order to put a stop to it.",
    url: 'https://sanji.to/watch/the-ancient-magus-bride-season-2-18338'
  },
  {
    index: '10',
    image: 'https://img.zorores.com/_r/1366x768/100/56/cc/56cca40be898cbecc462ea9987870942/56cca40be898cbecc462ea9987870942.jpg',
    title: 'Dr. Stone: New World',
    release: 'Apr 6, 2023',
    duration: '23m',
    quality: 'HD',
    cc: '11',
    episodes: '11',
    description: 'With the ambitious Ryuusui Nanami on board, Senkuu Ishigami and his team are almost ready to sail the seas and reach the other side of the world—where the bizarre green light that petrified humanity originated. Thanks to the revival of a skillful chef, enough food is being prepared for the entire crew, and the incredible reinvention of the GPS promises to ensure safety on the open sea.Preparations for the upcoming journey progress swimmingly until Senkuu receives an eerie message from a mysterious source. More driven than ever, the scientist sets out to explore the new world and discover what it can offer for his scientific cause. Though the uncharted territories may hide unkind surprises, Senkuu, with a little help from science, is ready to take on any challenge.',
    url: 'https://sanji.to/watch/dr-stone-new-world-17725'
  },
  {
    index: '11',
    image: 'https://img.zorores.com/_r/1366x768/100/40/22/402294e6873d87b6c81d42902a13d07c/402294e6873d87b6c81d42902a13d07c.jpg',
    title: 'The Tunnel to Summer, the Exit of Goodbye',
    release: 'Sep 9, 2022',
    duration: '1h 23m',
    quality: 'HD',
    cc: '1',
    episodes: 'Not declared yet',
    description: "Kaoru Tono heard a rumor: The laws of space and time mean nothing to the Urashima Tunnel. If you find it, walk through and you'll find your heart's desire on the other side...in exchange for years of your own life. One night, Kaoru just so happens to find himself standing in front of a tunnel that looks suspiciously like the one the rumor describes. He finds himself thinking of Karen, the sister he lost in an accident five years ago.  To Kaoru's surprise, he's been followed by the new transfer student Anzu Hanashiro, who promises to help him experiment with the mysterious tunnel—but what does she want from Kaoru in exchange? And what will he have left to give, after the tunnel's done with him?",
    url: 'https://sanji.to/watch/the-tunnel-to-summer-the-exit-of-goodbye-18393'
  },
  {
    index: '12',
    image: 'https://img.zorores.com/_r/1366x768/100/58/d0/58d0b99666b285d2c484fec5dfaa23f0/58d0b99666b285d2c484fec5dfaa23f0.jpg',
    title: 'Bleach',
    release: 'Oct 5, 2004',
    duration: '24m',
    quality: 'HD',
    cc: '366',
    episodes: '366',
    description: "Ichigo Kurosaki is an ordinary high schooler—until his family is attacked by a Hollow, a corrupt spirit that seeks to devour human souls. It is then that he meets a Soul Reaper named Rukia Kuchiki, who gets injured while protecting Ichigo's family from the assailant. To save his family, Ichigo accepts Rukia's offer of taking her powers and becomes a Soul Reaper as a result.However, as Rukia is unable to regain her powers, Ichigo is given the daunting task of hunting down the Hollows that plague their town. However, he is not alone in his fight, as he is later joined by his friends—classmates Orihime Inoue, Yasutora Sado, and Uryuu Ishida—who each have their own unique abilities. As Ichigo and his comrades get used to their new duties and support each other on and off the battlefield, the young Soul Reaper soon learns that the Hollows are not the only real threat to the human world.",
    url: 'https://sanji.to/watch/bleach-806'
  }
]
  ```

  <br />
  
</details>

<br />

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
