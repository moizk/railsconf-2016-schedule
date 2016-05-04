#2016

## First Day

### Stuck in the Middle: Leverage the power of Rack Middleware (3501 EF)

Before a request ever hits your Rails application, it winds its way through a series of pieces of Rack middleware. Middleware sets session cookies, writes your logs, and enables the functionality in many gems such as Warden.

With Rails or any Rack app, you can easily insert your own custom middleware, allowing you to log, track, redirect, and alter the incoming request before it hits your application.

You will leave this talk confident in writing your own custom middleware, better able to troubleshoot gems that rely on middleware and with an understanding of how your Rails app functions.

AMY UNGER
The granddaughter of a former MIT computer (yup, that was a job title), Amy was clearly supposed to be a programmer, but just did not get the message. Her wanderings have taken her through the land of libraries and archives and into software consulting. Now a software engineer at Heroku, she is deeply grateful for every scarce day she does not use vim commands in Google Docs.

### Multi-table Full Text Search with Postgres (3501 EF)

Searching content across multiple database tables and columns doesn't have to suck. Thanks to Postgres, rolling your own search isn't difficult.

Following an actual feature evolution I worked on for a client, we will start with a search feature that queries a single column with LIKE and build up to a SQL-heavy solution for finding results across multiple columns and tables using database views.

We will look at optimizing the query time and why this could be a better solution over introducing extra dependencies which clutter your code and need to be stubbed in tests.

CALEB THOMPSON
Speaker, developer, painter, gamer: an eccentric eclectic. Caleb is currently coding mostly in Ruby and Go. He has braved the wintry tundra of Alaska and the harsh deserts of Arizona. He has fired a Mosin-Nagant without blinking, fought the Red Menace, built Battleship Couch, and killed a bear and wore its pelt. He enjoys fine wines, craft beers, and punching comets.

### Foreign API Simulation with Sinatra (3501 EF)

Nowadays, we often rely on third party services that we integrate into our product, instead of building every aspect of an application. In many cases, well written API clients exist, but on occasion you run into the issue that there isn't a ready to use client or it simply doesn't fit your needs. How do you write a good API client and more importantly how do you test it without hitting the remote API. So far, the standard approach has been replaying requests with VCR or stubbing them with Webmock. There is a third option: simulating foreign APIs with Sinatra from within your test suite!

KONSTANTIN TENNHARD
Hi, I'm Konstantin, a computer scientist who specializes in developing large scale internet applications. Not too long ago I moved from Germany to Canada to work at Shopify.

Software design is what I live and breathe. I use it as a tool to empower other developers to move faster and with more confidence. My scientific interests on the other hand are natural language processing and statistical learning methods.

### 3x Rails: Tuning the Framework Internals (3501 EF)

Matz declared that the next major version of Ruby is going to be 3x faster than Ruby 2. But how can we make a software 3x faster? Can we do that for Rails?

In this session, we will discuss the ways to survey performance hotspots in each layer of the framework, tuning techniques on the performance issues, and some actual works that you can apply to your apps.

Topics to be covered:

Speeding up DB queries and model initialization
View rendering and template lookup
Routes and URLs
Object allocations and GC pressure
Faster Rails boot and testing
Asset Pipeline tweaks
AKIRA MATSUDA
Rails committer, Ruby committer, Haml committer, creator of widely used Rails plugins such as Kaminari, activedecorator, actionargs, i18ngenerators, html5validators, motorhead, erd, database_rewinder, etc. Founder of "Asakusa.rb", the most active Ruby community in Japan.


### Zen and the Art of the Controller (3501 DC)

JUNIOR-DEVELOPER
So you’re fresh out of boot camp or just off a month long binge on RoR tutorials/examples and you’re feeling pretty good about MVC and how controllers fit into the whole framework. But projects in the wild are often far more complicated than you’ve been exposed to. In this talk, we’re going to discuss several techniques used by seasoned engineers to build and refactor controllers for features you’ll actually be working on.

MICHAEL KELLY
Michael Kelly, Senior Engineer with Assembled Brands, is passionate about two things, building MVPs and teaching cool technologies to younger developers. He’s been building Rails applications for over three years now and has over seven years of experience as a software engineer. He tweets a little and is generally just a bad monkey.

### Facepalm to Foolproof: Avoiding Common Production Pitfalls (3501 DC)

JUNIOR-DEVELOPER
"WTF asset pipeline?" 
"What are all these errors?" 
"Why is my app running so slow?"

If you're new to Rails development, or just want some tips on deploying and running in production, this is the talk for you. Relying on real-world experience as part of the Heroku support team, we'll talk through common issues (and a few funny ones) we see when people take their "but it works in development!" app to a production environment.

JON MCCARTIE
Jon sold all his stuff, bought an RV, and lives full-time on the road with his wife and 3 kids. Jon works at Heroku.

## 2nd day

### ActionCable for Not-Another-Chat-App-Please (3501 DC)

RealTime updates using WebSockets are so-hot-right-now, and Rails 5 introduces ActionCable to let the server talk to the browser. Usually, this is shown as a Chat application -- but very few services actually use chats.

Instead, Rails Apps want to be able to update pages with new inventory information, additional products, progress bars, and the rare notification. How can we make this happen in the real world? How can we handle this for unauthenticated users? How can we deploy this?

JESSE WOLGAMOTT
Jesse is the Back-end Curriculum Lead Instructor at The Iron Yard, has taught Ruby courses since 2012, authored a book on AngularJS+Rails, and has loved Rails since 2007. Jesse has trained and spoke at conferences internationally, and has determined that Tacos rule and salads drool.


### Rails 5 Features You Haven't Heard About (3501 DC)

We've all heard about Action Cable, Turbolinks 5, and Rails::API. But Rails 5 was almost a thousand commits! They included dozens of minor features, many of which will be huge quality of life improvements even if you aren't using WebSockets or Turbolinks.

This will be a deep look at several of the "minor" features of Rails 5. You won't just learn about the features, but you'll learn about why they were added, the reasoning behind them, and the difficulties of adding them from someone directly involved in many of them.

SEAN GRIFFIN
Sean is a committer on Ruby on Rails, the maintainer of Active Record, cohost of The Bike Shed podcast, and the creator of Diesel, an ORM and query builder for Rust. Having spent over a decade in the industry, he now focuses entirely on open source software. In recent months he primarily focuses on Rust and improving the web development landscape.

### Turbolinks 5: I Can’t Believe It’s Not Native! (3501 DC)

Learn how Turbolinks 5 enables small teams to deliver lightning-fast Rails applications in the browser, plus high-fidelity hybrid apps for iOS and Android, all using a shared set of web views.

SAM STEPHENSON
Sam lives in Chicago and has been building web applications at Basecamp since 2005.


### Small Details, Big Impact (3501 G)

Most people are on the lookout for the Next Big Thing™, but at Skylight we know it’s #allthelittlethings that make for the best possible user experience. From the many not-so-happy paths of authentication to the challenge of guessing a user’s preferred name, we’ll dig deep into all those tiny details that will surprise and delight your customers. If you were hoping to hear more about how we use Rust, don't worry—we've got you covered! We’ll be sharing many of our finer implementation details as well as the thought processes behind them.

YEHUDA KATZ, LIZ BAILLIE
Yehuda Katz is one of the creators of Ember.js, a member of the Rust Core Team, and a retired Ruby on Rails and jQuery Core Team member. His 9-to-5 home is at the startup he founded, Tilde Inc.. There he works on Skylight, the smart profiler for Rails, and does Ember.js consulting. He's best known for his open source work, which also includes having created projects like Thor, Handlebars and Bundler. He blogs at http://yehudakatz.com and can be found on Twitter as @wycats.

Liz is a former cartoonist, current developer at Tilde, future sassy old woman with too many dogs.

This is a sponsored talk by Skylight.

