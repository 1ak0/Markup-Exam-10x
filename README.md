# Georgian Spotify 🎧

Spotify-ს ინტერფეისის მარკაპი (HTML + SCSS + JavaScript), შექმნილი საგამოცდო პროექტად.
პროექტი მოიცავს მთავარ გვერდს და 13 შიდა გვერდს, მუქ/ნათელ თემას და ადაპტირებულ დიზაინს მობილურისთვის, ტაბლეტისთვის და დესკტოპისთვის.

![Desktop view](docs/screenshot-desktop.png)

<p align="center">
  <img src="docs/screenshot-mobile.png" alt="Mobile view" width="260" />
</p>

## გვერდები

| გვერდი | ფაილი |
| --- | --- |
| მთავარი (Home) | `index.html` |
| Discover | `pages/discover.html` |
| ძებნა (Search) | `pages/search.html` |
| ბიბლიოთეკა (Library) | `pages/library.html` |
| ალბომი | `pages/album.html` |
| პლეილისტი | `pages/playlist.html` |
| არტისტი | `pages/artist.html` |
| სიმღერა | `pages/song.html` |
| პოდკასტი | `pages/podcast.html` |
| ეპიზოდი | `pages/episode.html` |
| პროფილი | `pages/profile.html` |
| Now Playing | `pages/now-playing.html`, `pages/now-playing-text.html`, `pages/now-playing-music-section.html` |

## ფუნქციონალი

- **ადაპტირებული დიზაინი:** mobile-first მიდგომა, ძირითადი breakpoint-ები `768px`, `992px`, `1024px`, `1280px`.
- **მუქი / ნათელი თემა:** გადამრთველი ზედა მენიუში, არჩევანი ინახება `localStorage`-ში და გვერდის განახლების შემდეგაც რჩება.
- **Friends Activity პანელი:** იხსნება და იხურება მომხმარებლების ხატულით.
- **ქარდების "დასტის" ეფექტი:** JavaScript ქარდის სურათს CSS ცვლადად (`--img-stack`) გადასცემს.
- **ფერის ავტომატური შერჩევა:** Search გვერდზე ქარდის ფონი სურათის საშუალო ფერით იღებება (`canvas`-ით).
- **ანიმაციები Discover გვერდზე:** `IntersectionObserver` ანიმაციას იწყებს მხოლოდ მაშინ, როცა სექცია ეკრანზე ჩანს.
- **მობილური ნავიგაცია:** ქვედა მენიუ Home / Discover / Search / Library / Me.
- **ნავიგაცია `<details>`-ით:** Pins და Playlists ჩამოსაშლელი მენიუები JavaScript-ის გარეშე.

## ტექნოლოგიები

- HTML5
- SCSS (Sass modules, `@use`)
- Vanilla JavaScript
- შრიფტი: [Satoshi](https://www.fontshare.com/fonts/satoshi)

## პროექტის სტრუქტურა

```
Markup-Exam-10x/
├── index.html
├── pages/                  # შიდა გვერდები
├── assets/
│   ├── fonts/Satoshi/
│   ├── img/                # სურათები და ხატულები
│   ├── js/main.js
│   └── styles/
│       ├── style.scss      # მთავარი SCSS ფაილი
│       ├── style.css       # დაკომპილირებული CSS
│       ├── abstracts/      # ცვლადები და mixin-ები
│       ├── base/           # reset და შრიფტები
│       ├── components/     # ღილაკები, ქარდები, ხატულები
│       ├── layouts/        # header, aside, player და გვერდების განლაგება
│       ├── sections/       # ცალკეული სექციები
│       └── animations/
└── favicon.ico
```

## გაშვება

1. დააკლონე რეპოზიტორია:
   ```bash
   git clone https://github.com/1ak0/Markup-Exam-10x.git
   ```
2. გახსენი საქაღალდე VS Code-ში.
3. გაუშვი **Live Server** გაფართოებით (`index.html` → მარჯვენა კლიკი → *Open with Live Server*).

> ფაილის პირდაპირ გახსნისას (`file://`) Search გვერდზე ფერის ავტომატური შერჩევა არ მუშაობს ბრაუზერის უსაფრთხოების წესების გამო, ამიტომ გამოიყენე Live Server.

### SCSS-ის დაკომპილირება

სტილების შეცვლისას `style.scss` უნდა დაკომპილირდეს `style.css`-ში. მაგალითად, **Live Sass Compiler** გაფართოებით, ან ტერმინალით:

```bash
sass --watch assets/styles/style.scss assets/styles/style.css
```

## ავტორი

**Iako** · [GitHub](https://github.com/1ak0)

---

პროექტი შექმნილია სასწავლო მიზნით. Spotify-ის სახელი, დიზაინი და გამოყენებული ალბომების/არტისტების სურათები ეკუთვნის მათ მფლობელებს.