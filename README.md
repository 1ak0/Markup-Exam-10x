<div align="center">

# 🎧 Georgian Spotify

**Spotify-ის ინტერფეისის რესპონსიული მარკაპი, შექმნილი HTML-ით, SCSS-ით და JavaScript-ით**

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![Sass](https://img.shields.io/badge/Sass-CC6699?style=for-the-badge&logo=sass&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)

[**🔗 Live Demo**](https://1ak0.github.io/Markup-Exam-10x/) · [**📂 კოდი**](https://github.com/1ak0/Markup-Exam-10x)

</div>

---

## 📑 სარჩევი

- [პროექტის შესახებ](#-პროექტის-შესახებ)
- [ფუნქციონალი](#-ფუნქციონალი)
- [გვერდები](#-გვერდები)
- [ტექნოლოგიები](#-ტექნოლოგიები)
- [პროექტის სტრუქტურა](#-პროექტის-სტრუქტურა)
- [გაშვება](#-გაშვება)
- [ავტორი](#-ავტორი)

---

## 📌 პროექტის შესახებ

**Georgian Spotify** არის Spotify-ის ვებ-აპლიკაციის ინტერფეისის მარკაპი, შექმნილი საგამოცდო პროექტად.
პროექტი მოიცავს **14 გვერდს** და სამივე ზომაზე მუშაობს: მობილური, ტაბლეტი და დესკტოპი.

მთავარი მიზანი იყო:

- სუფთა, სემანტიკური HTML სტრუქტურა
- მოდულური SCSS არქიტექტურა
- mobile-first რესპონსიული დიზაინი
- ინტერაქტიული ელემენტები ბიბლიოთეკების გარეშე, სუფთა JavaScript-ით

---

## ✨ ფუნქციონალი

| | ფუნქცია | აღწერა |
| :---: | --- | --- |
| 🌗 | **მუქი / ნათელი თემა** | გადამრთველი ზედა მენიუში. არჩევანი ინახება `localStorage`-ში და გვერდის განახლების შემდეგაც რჩება |
| 📱 | **რესპონსიული დიზაინი** | mobile-first მიდგომა, ცალკე ნავიგაცია მობილურისთვის და დესკტოპისთვის |
| 👥 | **Friends Activity** | მეგობრების აქტივობის პანელი, რომელიც იხსნება და იხურება ღილაკით |
| 🃏 | **ქარდების "დასტის" ეფექტი** | JavaScript ქარდის სურათს CSS ცვლადად (`--img-stack`) გადასცემს |
| 🎨 | **ფერის ავტომატური შერჩევა** | Search გვერდზე ქარდის ფონი სურათის საშუალო ფერით იღებება (`canvas` API) |
| 🎞️ | **ანიმაციები scroll-ზე** | Discover გვერდზე `IntersectionObserver` ანიმაციას იწყებს, როცა სექცია ეკრანზე გამოჩნდება |
| 📂 | **ჩამოსაშლელი მენიუ** | Pins და Playlists მენიუები `<details>` ელემენტით, JavaScript-ის გარეშე |
| 🎵 | **Player** | ქვედა პლეერი მობილურისთვის და გაფართოებული ვერსია დესკტოპისთვის |

### 📐 Breakpoint-ები

| მოწყობილობა | სიგანე |
| --- | --- |
| 📱 მობილური | `< 768px` |
| 📟 ტაბლეტი | `≥ 768px` |
| 💻 ლეპტოპი | `≥ 992px` / `≥ 1024px` |
| 🖥️ დესკტოპი | `≥ 1280px` |

---

## 🗂 გვერდები

| გვერდი | ფაილი | აღწერა |
| --- | --- | --- |
| 🏠 Home | `index.html` | მთავარი გვერდი: პლეილისტები, მიქსები, არტისტები, ალბომები, პოდკასტები |
| 🧭 Discover | `pages/discover.html` | ახალი მუსიკის აღმოჩენა ანიმაციებით |
| 🔍 Search | `pages/search.html` | ძებნა და კატეგორიები |
| 📚 Library | `pages/library.html` | მომხმარებლის ბიბლიოთეკა |
| 💿 Album | `pages/album.html` | ალბომის გვერდი სიმღერების სიით |
| 🎶 Playlist | `pages/playlist.html` | პლეილისტის გვერდი |
| 🎤 Artist | `pages/artist.html` | არტისტის პროფილი |
| 🎵 Song | `pages/song.html` | სიმღერის დეტალები და ტექსტი |
| 🎙️ Podcast | `pages/podcast.html` | პოდკასტის გვერდი |
| 📻 Episode | `pages/episode.html` | პოდკასტის ეპიზოდი |
| 👤 Profile | `pages/profile.html` | მომხმარებლის პროფილი |
| ▶️ Now Playing | `pages/now-playing*.html` | მიმდინარე სიმღერის 3 ხედი: პლეერი, ტექსტი, რიგი |

---

## 🛠 ტექნოლოგიები

- **HTML5:** სემანტიკური ელემენტები (`header`, `nav`, `main`, `aside`, `section`, `article`, `footer`)
- **SCSS:** Sass მოდულები (`@use`), ცვლადები, mixin-ები
- **JavaScript (ES6+):** `localStorage`, `IntersectionObserver`, `Canvas API`
- **შრიფტი:** [Satoshi](https://www.fontshare.com/fonts/satoshi)

---

## 📁 პროექტის სტრუქტურა

<details>
<summary><b>დააჭირე სტრუქტურის სანახავად</b></summary>

<br />

```
Markup-Exam-10x/
├── index.html
├── pages/                     # შიდა გვერდები (13 ფაილი)
└── assets/
    ├── fonts/Satoshi/         # შრიფტები
    ├── img/                   # სურათები და ხატულები
    ├── js/
    │   └── main.js            # მთელი ინტერაქტივი
    └── styles/
        ├── style.scss         # მთავარი SCSS ფაილი
        ├── style.css          # დაკომპილირებული CSS
        ├── abstracts/         # ცვლადები და mixin-ები
        ├── base/              # reset და შრიფტები
        ├── components/        # ღილაკები, ქარდები, ხატულები
        ├── layouts/           # header, sidebar, player, გვერდების განლაგება
        ├── sections/          # ცალკეული სექციები
        └── animations/        # ანიმაციები და hover ეფექტები
```

</details>

---

## 🚀 გაშვება

**1. დააკლონე რეპოზიტორია**

```bash
git clone https://github.com/1ak0/Markup-Exam-10x.git
cd Markup-Exam-10x
```

**2. გაუშვი Live Server-ით**

გახსენი საქაღალდე VS Code-ში → `index.html` → მარჯვენა კლიკი → **Open with Live Server**

> [!NOTE]
> ფაილის პირდაპირ გახსნისას (`file://`) Search გვერდზე ფერის ავტომატური შერჩევა არ მუშაობს ბრაუზერის უსაფრთხოების წესების გამო. ამიტომ გამოიყენე Live Server.

**3. SCSS-ის დაკომპილირება** (თუ სტილებს ცვლი)

```bash
sass --watch assets/styles/style.scss assets/styles/style.css
```

ან გამოიყენე VS Code-ის გაფართოება **Live Sass Compiler**.

---

## 👤 ავტორი

**Ia Gigolashvili**

[![GitHub](https://img.shields.io/badge/GitHub-1ak0-181717?style=flat&logo=github)](https://github.com/1ak0)

---

<div align="center">

<sub>პროექტი შექმნილია სასწავლო მიზნით. Spotify-ის სახელი, დიზაინი და ალბომების/არტისტების სურათები ეკუთვნის მათ მფლობელებს.</sub>

<br />


</div>
