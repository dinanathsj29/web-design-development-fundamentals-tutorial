Web Design Development Foundations-Web Technology Fundamentals
=====================
We use the Internet for Banking, Shopping, Ticket Bookings, Music/Entertainment, and Social Media, but do you really know how the web works? Here I introduce the technology that makes the web run, the terminology involved, and how it all comes together to power the websites we know and love. Will cover various term/technologies involved like (HTML, CSS, JavaScript, URL, DNS, HTTP), and explains what separates the front end (what we see), from the back end (what we don't) on the web, databases, servers and the technology that makes the web work.

Topics include
===================== 
1. [Course Introduction](#section-1-course-introduction)
2. [Introduction to Web World](#section-2-introduction-to-web-world)
3. [Introduction to Front-End Technology](#section-3-introduction-to-front-end-technology)
4. [Introduction to Back-End Technology](#section-4-introduction-to-back-end-technology)
5. [Other Supporting Technology](#section-5-other-supporting-technology)
6. [Whats Next Step?](#section-6-whats-next-step)

Section 1. Course Introduction
=====================
### 1.1. Welcome
Hi All, I'm **`Dinanath Jayaswal, Senior UI/Web Developer and Adobe Certified Expert Professional`**, I wanna welcome you to Web Design Development Foundations-Web Technology Fundamentals. This content is designed to introduce the fundamental concepts, surrounding terminology, technology, techniques, terms that are used to create and run the web. For anyone new to the web the vast number of terms, abbreviations, and processes involved can be a little bit overwhelming, disturbing. It's my goal to explain in the core, basic terms how the web works, Client, Servers, Browsers, Front End, Back End and various terminology involved, also how the technology all fits together.

This course contents roadmap to becoming a Web Designer/Developer.

### 1.2. Who is this for?
This course is for every Web/Internet User, fresher as well as an experienced Web Designer/Developer who wants to learn-brush up-cover up various terms/techniques/acronyms/abbreviations used in Web/Internet Design/Development world.

Section 2. Introduction to Web World
=====================
### 2.1. How does the web work?
#### The Internet
  Massive networks of millions of computers all over the world that use to share and transmit information trough following protocols/mediums
- Email
- Sms messaging
- Application data
- World Wide Web

#### World Wide Web (WWW)
- Runs over the Internet
- Transfer data using HTTP (Hyper Text Transfer Protocol)

#### The Web 
Communication/series of interaction between Clients & Servers

#### Clients
Devices which requests and renders web contents. Some of the popular clients are Browsers, Mobile Apps, Screen Reader Devices etc

#### Servers
Applications which deliver Web Contents, Services to Clients

### 2.2. Client-Server Interaction Model
#### Browser 
- The browser is Software/application helps to visit, view, accessing information and take the best use of websites/web pages
- Popular browsers are `Google Chrome, Mozilla Firefox, Internet Explorer, Safari` etc.

<p>
  <figure>
    &nbsp;&nbsp;&nbsp; <img src="./images/browers_all_2.png" alt="all browsers" title="widely used browsers" width="400" border="2" />
    <figcaption>&nbsp;&nbsp;&nbsp; Image - Widely used modern browsers</figcaption>
  </figure>
</p>

#### Request <--> Response Mechanism 
```
1. User Type in `URL (Uniform Resource Locator)` like `http://www.yahoo.com` -> 
2. URL passed to `DNS (Domain Name Server)` -> 
3. DNS translates URL into `IP (Internet Protocol)` address (`172.16.0.0`) -> 
4. Browser use DNS to locate host server and send request of content (in the form of HTML page, Images, CSS, JavaScript).
```

<p>
  <figure>
    &nbsp;&nbsp;&nbsp; <img src="./images/client_server_request_response.png" title="Request Response Mechanism Image" alt="Client Server, Request Response Mechanism" border="2" />
    <figcaption>&nbsp;&nbsp;&nbsp; Image - Client Server, Request Response Mechanism</figcaption>
  </figure>
</p>

#### Static Sites
Simply shows content (which is `not change frequently`) requested by the client without any additional processing (Static sites pages usually consists of Front end technologies like HTML, CSS, JavaScript)
  
#### Dynamic Sites
First Business Logic execute by Web Applications like ASP, PHP, Ruby on Rails etc. than browser shows content (`latest/updated`) requested by the client (Dynamic sites pages usually consists of Front end technologies like HTML, CSS, JavaScript, in combination with some Back end technology like ASP, PHP, Ruby on Rails etc.)

### 2.3. DNS (Domain Name Server)
- Every site have unique `IP (Internet Protocol)` address used to identify location `(http://www.google.com = 169.20.127.243)`
- DNS (Domain Name Server) is like `Internets phone book` which stores unique website and its IP (Internet Protocol) address for each and every website
- IP Address == Domain Name Server (172.16.0.0 == domain name http://www.yahoo.com or so)

### 2.4. Internet Protocol
- Protocols are simple languages/standards/set of rules through which computers share information which each other
- Internet wouldn't work at all without Protocols

- Different/multiple layers of protocols
  - **Application Layer (creation & sharing of data over the web)**
    - HTTP (Hyper Text Transfer Protocol)
    - FTP (File Transfer Protocol)
    - SMTP (Simple Mail Transfer Protocol)
    - DNS (Domain Name Server)
    - RIP (Routing Information Protocol)
    - SNMP (Simple Network Management Protocol)
  - **Transport Layer (communication)**
    - TCP (Transmission Control Protocol and Internet Protocol created in 1973)
    - UDP (User Datagram Protocol)
  - **Internet Layer (address and routing structure of data)**
    - IPv4 (Internet Protocol Version 4)
    - IPv6 (Internet Protocol Version 6)

### 2.5. HTTP (Hyper Text Transfer Protocol)
- Standard protocol for `transferring data/resources over the Web`
- In case of HTTP, Browsers are HTTP Clients, send HTTP request and Servers are HTTP Servers, send the HTTP response to transfer data with a standardized format
- HTTP is one-way `stateless protocols`, it simply means that once the REQUEST sent & RECEIVED than that state is forgotten ie discarded by the browser and web server, which makes HTTP very much simple and efficient
- Due to one way stateless nature its difficult to send and receive OR upload and download large files with HTTP.

#### Some Common web protocols
- **FTP (File Transfer Protocol)**
Typically used to `transfer large files` and its ideal for uploading or downloading files to your site
- **SMTP (Simple Mail Transfer Protocol)**
The Standard web protocol for `sending email` across the web. Most email clients use SMTP for sending and receiving emails
- **POP (Post Office Protocol)**
POP typically used to `receive emails`.
- **RTP (Real-Time Transfer Protocol)**
Standard protocol for `delivering/serving audio or video` over the web. Its commonly used in voice over and chat applications.
- **RTMP (Real Time Messaging Protocol)**
Developed by Macromedia (Adobe Corp.) for `streaming audio video and data` over the Internet, between a Flash player and a server.
- **HTTPS (Hypertext Transfer Protocol Secure)**
HTTP layered with a security protocol. Usually used for e-commerce or other secure transactions, payment gateways.

### 2.6. URL (Uniform Resource Locator)
URL Uniform Resource Locator OR (Universal Resource Locator) specifies its location on a computer network (web address, web path, web site name).

#### Anatomy/contains of URL
`URL = http://www.yahoo.com` <br/>

| URL Parts             | Meaning/Description       |
| -------------         |:-------------------------:|
| http                  | protocol                  |
| //www.yahoo.com:8080  | resource name             | 
| www                   | sub-domain (Most of cases sub-domain is not required ie you can type http://yahoo.com) |
| yahoo                 | domain name               |
| com                   | top-level domain          |

#### URL path/port

http://www.yahoo.com/products/product1.html

http://www.yahoo.com:80 (`80 = port number (80 is default port`))

#### Top level domain 
- .com
- .net
- .org
- .info

### 2.7. How browser works
The browser uses HTTP to communicate with Web Server and request pages, content. Browsers rendering engine translates/renders pages and displays the contents as per support.

#### Why browsers behave differently
- Browsers developed independently of each other
- Multiple rendering engines drive page layout
- DOM (Document Object Model) support varies
- Browsers use independent JavaScript engines

#### Common Rendering Engines

| Engine        | Browser       |
| ------------- |:-------------:|
| Trident       | Internet Explorer, (AOL - America Online), Windows Mobile |
| Presto        | Opera |
| Gecko         | Mozilla FF, Camino  |
| Webkit        | Safari, Google Chrome, WebOS |
| Blink         | Google Chrome, Opera 14+ |

### 2.8. W3C and Web standards (World Wide Web Consortium)
- `W3C (World Wide Web Consortium) is main International Standards Organization for the World Wide Web help in `developing protocols and guidelines` that ensure long-term growth for the Web
- W3C (World Wide Web Consortium) started in the year 1994 to issue recommendations for web technologies
- Check web standards for consistent design (The Web Standard Project): www.webstandards.org
- W3C website: https://www.w3.org/

### 2.9. Web Server
Websites are hosted/uploaded on Web Server. Web Server is nothing more than normal computer installed with specialized software and components for a specific use.
Web stacks are groups of software that work with each other to build and process websites (static & Dynamic websites).

#### Web stacks consists of
- OS (Operating System)
- Web Server
- Database Server
- Programming Language

#### Common web stacks
| Web Stack        | Full Form (Technologies)       |
| ------------- |:-------------:|
| LAMP          | Linux Apache MySql Php / Linux Apache MySql Perl/Python |
| MAMP          | Macintosh Apache MySql Php |
| WAMP          | Windows Apache MySql Php |
| WISA          | Windows IIS MS SQL .NET |
| MARS          | MySql Apache Ruby Solaris |

Section 3. Introduction to Front-End Technology
=====================
### 3.1. Front End Design (Client Side)
#### Front End (Client Side) Design refers to:
- The `visual part/User Interface layer (what we see)` of websites/applications
- Front End Design is typically the `UI, Layout, typography/fonts, images` and many other visual elements/aspects shown on the web page and their styling.
- One can also refer it as usability and user experience design as well

#### 3 pillars / core Languages/technologies used for Frond End Web Design/Development
1. **HTML (HyperText Markup Language)** - Essential Structure / Content, Redable and convey structure to user
2. **CSS (Cascading Style Sheet)** - Page Design / Layouts / Styling / Formattings, look and feel
3. **JavaScript (JS)** - Page Behavior, Logic, Conditions and Validations

#### Front End Design/Web Design
Web Design is creating and designing web pages, designing for all user interfaces/experiences like browsers, screen readers, mobiles, printers

#### Front-End Design/Development includes
- The visual part of web design
- Planning
- Structuring content/data/pages
- User Interface designing / Client Side designing
- Interactivity 

#### Front End Designer Role
- Includes visual part of web designing
- Creating mockups and developing visual standards
- UI designing, typography, page layout
- Structuring semantic content/data/pages
- Mainly works with HTML, CSS, Photoshop
  
#### Front-End Developer Role
- Can act and do the part of Front End Designer
- Planning for Dynamic Content
- Logical/Conditional Interactivity
- Fetch Data from Servers with APIs
- Mainly works with JavaScript and other JS frameworks, HTML, CSS

#### Web Designing workflow
- Determine web site/clients/Audience goals 
- Clearly Define contest - navigation / content organization
- WireFraming / Architecting the site - proper navigation / content organization
- Generate Mockups - post-it, illustrator / Photoshop / Fireworks
- Build it - HTML CSS JS Flash
- Test it - Multiple Browsers / Devices, consistent output

#### Interactive Design
- The creation and integration of feature-rich interfaces
- Organize content and flow properly
- Plan navigation
- Use Video and blended media

#### Client Side Scripting
Script executed in the browser environment (JavaScript)

<p>
  <figure>
    <img src="./images/html5.png" alt="HTML5 Logo" title="HTML5" border="2" align="right"/>
  </figure>
</p>

### 3.2. HTML (HyperText Markup Language)
#### HTML
- HyperText Markup Language
- The Standard/foundation/gateway language used for creating/structuring content on the web
- We can create a static website by HTML only
- NO HTML = NO WEB PAGE :)

#### History of HTML
| Year          | History       |
| ------------- |:-------------:|
| 1990          | Specification Drafted in Mid 90s by Tim Berners Lee |
| 1991          | Tim Berners Lee published document called "HTML Tags" |
| 1995          | HTML 2.0 ('standard' HTML) |
| 1997          | HTML 3.2 (proprietary browser companies developed many features) |
| 1999          | HTML 4.0 W3C Web standards support |
| 2000          | XHTML 1.0 (HTML move towards XML)-Extensible Markup Language |
| 2001          | 2009 - XHTML 2.0 |
| 2004          | WHATWG formed (Web HyperText Application Technology Working Group, they continued with development of HTML 5.0) |
| 2007          | 2008 - W3C adopts WHATWG's HTML5 Web Application 1.0 specification and drafts |
| 2009          | XHTML 2.0 drops/stops |
| 2014          | W3C Recommendation: HTML5 |

### 3.3. HTML page structuring
- HTML Syntax is very simple easy to learn
- HTML page consists of `DTD & TAGS` for different visual aspects

#### Basic HTML page structure
```
  <!DOCTYPE html>

  <html lang="en">

    <head>
      <meta charset="UTF-8">
      <meta name="viewport" content="width=device-width, initial-scale=1.0">
      <meta http-equiv="X-UA-Compatible" content="ie=edge">
      <title>Basic HTML</title>
    </head>

    <body>
      <p>This is Basic HTML page </p>
    </body>

  </html>
```

#### DTD (Document Type Declaration OR Document Type Definition)
- Usually the first line of an HTML page, its an instruction to the web browser about what version of HTML the page is written and rules to parse/render.

| HTML Version    | DTD           |
| -------------   |:-------------:|
| HTML5           |  Document Type Declaration (&lt;!DOCTYPE html&gt; |
| XHTML           |  Document Type Definition (.DTD file) &lt;!DOC TYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Strict//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd"&gt; | 
| HTML4           |  Document Type Definition (.DTD file) &lt;!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01 Transitional//EN" "http://www.w3.org/TR/html4/loose.dtd"&gt; |

#### Tags
- Tags are html commands/set of instructions to create web page with specific UI element
- Tags are used to identify content like `<h1> = heading 1`, `<p> = paragraph` etc.
- HTML contains tags which are used to identify elements and structure pages example `<header>,<table>,<li>,<img>`
- `<head>` tag consists of non visual elements, meta tags, links to  external .css, .js files and libraries
- `<body>` tag contents all visual elements which appears on web page

#### Tools for building web sites-web pages/writing HTML
- Text Editor/HTML Editor like `NotePad, NotePad++, SublimeText, Atom, Brackets, Coda, Visual Studio Code, DreamWeaver` etc.
- To view output of .html pages we need Browsers like - `Google Chrome, Mozilla Firefox, Internet Explorer, Safari` etc.

<p>
  <figure>
    <img src="./images/css3.png" alt="CSS3 Logo" title="CSS3" border="2" align="right"/>
  </figure>
</p>

### 3.4. CSS (Cascading Style Sheets)
- CSS is presentational, styling, formatting language developed to control look and feel of HTML files
- Presentational markup tags like `<font> <b> <i> <u>` etc discouraged or deprecated as style-sheet language like CSS developed to control the presentation of HTML documents
- Styles can be written in different ways:
  1. **external style**: `style.css` (separation of concern)
  2. **embedded/internal styles**: `<style> </style>`
  3. **inline styles**: `<p styles="color:red; font-size: 18px;">`This is an inline style </p>

#### CSS selector (selector { declaration - property: value; })
```
  p {
    color: red;
    font-size: 18px;
  }
```

#### 1. external style**: `style.css` (separation of concern)
##### `index.html`

```
  <!DOCTYPE html>

  <html lang="en">

    <head>
      <meta charset="UTF-8">
      <meta name="viewport" content="width=device-width, initial-scale=1.0">
      <meta http-equiv="X-UA-Compatible" content="ie=edge">
      <title>external style</title>
      <link href="style.css" rel="stylesheet" type="text/css" /> 
    </head>

    <body>
      <p>This is an external style </p>
    </body>

  </html>
```

##### `style.css`

```
  p {
    color: red;
    font-size: 18px;
  }
```

#### 2. embedded/internal styles
##### `index.html`

```
  <!DOCTYPE html>

  <html lang="en">

    <head>
      <meta charset="UTF-8">
      <meta name="viewport" content="width=device-width, initial-scale=1.0">
      <meta http-equiv="X-UA-Compatible" content="ie=edge">
      <title>embedded/internal styles</title>
      <style>
         p {
           color: red;
           font-size: 18px;
         }
      </style>
    </head>

    <body>
      <p>This is an embedded/internal styles </p>
    </body>

  </html>
```

#### 3. inline styles
##### `index.html`

```
  <!DOCTYPE html>

  <html lang="en">

    <head>
      <meta charset="UTF-8">
      <meta name="viewport" content="width=device-width, initial-scale=1.0">
      <meta http-equiv="X-UA-Compatible" content="ie=edge">
      <title>inline style</title>
    </head>

    <body>
      <p styles="color:red; font-size: 18px;">This is an inline style </p>
    </body>

  </html>
```

<p>
  <figure>
    <img src="./images/javascript_logo_1.png" alt="JavaScript Logo" title="JavaScript" border="2" width="200" align="right"/>
  </figure>
</p>

### 3.5. JavaScript
- Created and introduced by `Brendan Eich (Netscape) in 1995` to increase and expand the capabilities of the native browser.
- A client-side scripting language used to add interactivity and functionality to websites 
- JavaScript it has nothing to do with Java ...!!! NOT AT ALL RELATED to JAVA)

#### Common usage of JavaScript
- Build interactive elements, Rollover, Button clicks, Menus
- Create Dynamic Menus-Logics
- Open new browser windows
- Update data within the page/browser
- Client-side form validation
- Manipulate page elements

#### Basic JavaScript page structure
```
  <!DOCTYPE html>

  <html lang="en">

    <head>
      <meta charset="UTF-8">
      <meta name="viewport" content="width=device-width, initial-scale=1.0">
      <meta http-equiv="X-UA-Compatible" content="ie=edge">
      <title>Basic HTML JavaScript</title>
      <script>
        // write javascript code here
      </script>
    </head>

    <body>
      <p>This is Basic HTML JavaScript page </p>
    </body>

  </html>
```

- Scripts can be written at different places:
1. **external script**: `script.js` (separation of concern)
2. **embedded/internal script (under HEAD or BODY tag)**: `<script> </script>`

#### 1. external script: `script.js` (separation of concern)
##### `index.html`
```
  <!DOCTYPE html>

  <html lang="en">

    <head>
      <meta charset="UTF-8">
      <meta name="viewport" content="width=device-width, initial-scale=1.0">
      <meta http-equiv="X-UA-Compatible" content="ie=edge">
      <title>Basic HTML JavaScript</title>
      <script src="script.js"></script>
    </head>

    <body>
      <p>This is Basic HTML JavaScript page </p>
    </body>

  </html>
```

##### `script.js`

```
  // write javascript code here
  alert('external javascript code executed.');
```

#### 2. embedded/internal script (under HEAD or BODY tag)
##### `index.html`
```
  <!DOCTYPE html>

  <html lang="en">

    <head>
      <meta charset="UTF-8">
      <meta name="viewport" content="width=device-width, initial-scale=1.0">
      <meta http-equiv="X-UA-Compatible" content="ie=edge">
      <title>Basic HTML JavaScript</title>
      <script>
          // write javascript code here
          alert('embedded/internal javascript code executed.');
      </script>
    </head>

    <body>
      <p>This is Basic HTML JavaScript page </p>


      <script>
          // write javascript code here
          alert('embedded/internal javascript code executed.');
      </script>
    </body>

  </html>
```

#### JavaScript Frameworks/libraries 
- already have the various codes and common utilities ready
- collection of javascript methods and functions that make it easier to perform targeted tasks

#### Popular JavaScript frameworks/libraries
- jQuery
- Angular
- React
- Vue
- Prototype
- Ember
- D3

### 3.6. Images
There are many formats of photos/pictures/images/Web Graphics used on the web
- BMP
- GIF
- JPEG / JPG
- PNG 
- SVG

Creating images for the web often requires the designer to find a balance between keeping the file sizes small while maintaining acceptable image quality with resolution.

JPEG / JPG, GIF and PNG files type are the standard image formats for the web graphics.

#### GIF (Graphics Interchange Format)
- Introduced in 1987 by CompuServe 
- It is the most popular image format type on the web

##### GIF characteristics
- Limited to 256 colors support only
- Typically used for logos or icons
- GIFs support transparency and limited animation

#### JPEG / JPG (Joint Photographic Experts Group)
Image compression standard established in 1992 and widely used for areas such as the web and digital photography, often shortened to the file extension "JPG"

##### JPEG / JPG characteristics
- Supports millions of colors
- Used in all types of image High Resolutions Scenery
- Uses "lossy" compression to reduce file size
- JPGs are compressed each time they saved

#### PNG (Portable Network Graphic)
Created in 1995 to improve over JPEG and replace the GIF by open source community over copyright disputes/license issues with GIF

##### PNG characteristics
- Like GIFs Support transparency
- Uses lossless compression
- Like JPEG supports millions of colors
- Older browser support is lacking

#### SVG (Scalable Vector Graphics)
- SVG is a vector graphics format
- Can be scaled independently of resolution
- Graphics are written in SVG markup which makes them editable through the code
- Since they are markup they can be further styled through CSS
- SVG is now widely supported among latest devices and browsers

#### Tools for creating graphics/images
- Adobe Photoshop
- Adobe illustrator
- Adobe Fireworks
- CorelDraw
- GIMP

### 3.7. API (Application Programming Interfaces)
An exposed set of functions that allow other applications to access features and functionality without giving direct access to source code.

#### Widely used API Examples
- Using Google Maps
- Weather reports
- Youtube videos
- Facebook feeds
- Amazons latest offers
- Latest sports scores
- Latest Newsfeeds

### 3.8. HTML5 APIs
- HTML is used to create web pages/websites with simple standard elements
- HTML5 introduced following advanced APIs to avoid third-party plug-in support/dependency

#### HTML5 APIs Examples
- Media API - Audio/Video control
- Geo-Location API - Access current location of users
- Drag and Drop API - Drag and Drop functionality
- App Cache API - Storing data offline/caching for future use
- Canvas API - Draw directly in the browser

### 3.9. Web Fonts
- Earlier we use to use fonts available and installed on user machine like Arial, Verdana, Times, Sherif etc.
- Web Fonts technology allows the downloading and temporary installation of fonts within the browser
- @font-face CSS technique is used to request any engaging and latest fonts/typography from the web server
- **New font formats developed**
  - EOT  - Embedded OpenType
  - WOFF - Web Open Font Format 
- **Famous third-party font hosting server**
  - Google Fonts
  - Adobe Typekit

Section 4. Introduction to Back-End Technology
=====================
### 4.1. Server Side scripting
Any programming/scripting that runs on the web server is referred to as Server Side scripting. It may be:
- Processing Form data
- Managing users
- Booking a Movie Tickets, Travel, Hotel
- Online purchase

#### Server Side Scripting languages
- CGI (Common Gateway Interface)
- Perl
- ASP (Active Server Pages)
- Java 
- JSP (Java Server Pages)
- PHP (HyperText PreProcessor / Personal Home Page)
- .NET
- Cold Fusion CFML
- NodeJS

### 4.2. PHP
- In year `1994 Rasmus Lerdorf` has written a set of CGI scripts to track a visitor to his online resume. He opens sources the scripts and named it Personal Home Page (PHP).
- In 1997 developers named `Andi Gutmans and Zeev Suraski` rewrote the existing parser and released PHP 3.0, renaming it HyperText PreProcessor.
- As PHP was free and open source it attracted a wide community of developers
- PHP paired with other open source tools like Linux, Apache, and MySQL
- PHP was very easy to learn so it became one of the most important and widely used back end/server side scripting language to build robust/dynamic sites
- PHP is embedded within HTML but .php, .asp, .cfm pages must process/render on the server before it displays in browser
- Note - .php, .asp, .cfm or any other server-side scripting files will not run locally, you just need some software like MAMP, WAMP, XAMPP to set/create server environment on local

### 4.3. Popular Server Side Languages
- **JSP (Java Server Pages)**
  - Part of the larger Java framework and used by Java programmers
  - Scripts are combinations of XML and Java scriptlets
  - Used in enterprise level sites but can be used for any sized sites or applications
- **.NET**
  - VB .NET is referred as .NET but its part of the larger .NET framework
  - Used in enterprise level sites or applications
- **ColdFusion (Adobe ColdFusion)**
  - ColdFusion is added to the page through its own markup language called as CFML much like HTML
- **Python**
  - Powerful open source multi-purpose development language
- **Ruby**
  - General purpose development language
  - Its popular due to Ruby-on-Rails web framework

### 4.4. Dealing with Data
- Data used in websites/applications must stored in Database for future uses and retrievals like User Name, Password, Authentication details, Profile, Product list, Pricing and so on
- At client side ie in the browser due to security purpose, we can store a very less and limited amount of data
- DBMS (Database Management System) 
  - Store data in tables
- RDBMS (Relational Database Management System) 
  - Store data in tables that relate to each other
  - Allows complex sorting and filtering of data
  - MySQL, Sybase, Oracle, SQLite
- Non-Relational Database (No SQL database)
  - NoSQL database store data in object driven datasets
  - Faster to index and scale easier than relational databases
  - MongoDB, Cassandra, CouchDB, SimpleDB, HBase

### 4.5. SQL database (Structured Query Language)
- The Standard Query Language for managing and retrieving information from databases.
- SQL syntax is simple and logical, easy to learn
- select, insert, update, delete such simple keyword-based syntax statement used to manipulate data

### 4.6. CMS (CMS Content Management System)
- An application to control creation, management, publishing and archiving sites content
- A good CMS can speed up creation, updating of content faster, manage user groups, controls content as per roles
- Web-based CMS assist in the creation, publishing and archiving of site content, also provides advanced control over site functionality such as blogging, community boards, and e-commerce.

#### How to choose a CMS?
- Understand site goals and future needs
- Match site focus to CMS focus
- Look for quality plug-ins
- Look for robust support
- Compare budget to CMS needs
- Make sure site admin is simple
- Does the CMS allow custom layouts

#### Popular CMS
- `WordPress, Jhoomla, Drupal, Expression Engine, Radiant`
- www.expressionengine.com
- www.madebyfrog.com
- www.drupal.org
- www.joomla.org
- www.movabletype.org
- www.radiantcms.org
- www.wordpress.org

### 4.7. CDN (Content Delivery Network / Content Distribution Network)
- A system for delivering content over a distributed network of servers
- As a developer no need to download all libraries on local and do development, use CDN path to include required libraries, it will be cached and downloaded faster
- CDNs are largely used to serve static resources such as JavaScript/CSS libraries, videos or other site dependencies

#### Popular CDNs
- Google CDN
- Microsoft CDN

### 4.8. Cloud services (Cloud Computing)
Usually refers to distributed processes over the internet
- dropbox (store and share files, projects)
- youtube
- google cloud storage
- amazon web services
- microsoft cloud services
- rackspace
- heroku

### 4.9. GitHub
- Github is built around Git an open source version control system
- GitHub is an online distribution service that allows users to store repositories online that can be version controlled and shared with other users
- Allows to manage the project, publish files and store revisions, sharing and collaborating

Section 5. Other Supporting Technology
=====================
### 5.1. JavaScript libraries
- Collection of pre-written methods/functions features that make development faster and easier
- Extends the functionality of native JavaScript, may be focused sets like date.js, moment.js to jQuery a broader task oriented library

#### Popular JavaScript frameworks/libraries
- jQuery
- Angular
- React
- Vue
- Prototype
- Ember
- D3

### 5.2. Frameworks and Boilerplates
Collection of prebuilt HTML, CSS and JavaScript files designed to speed up, make the development of sites easier. 
- **HTML** - (readymade templates, semantic structure)
- **CSS** - (ready typography, layouts, Browser resets)
- **JavaScript** - (enhanced features modal windows, tooltips, menus)
- **`Examples** - Bootstrap, Angular, HTML Shiv Shim`

#### Boilerplate
- A set of templates build around a specific starting point or goal
- Provide a starting point for building sites or apps (latest features need to work/support in older browsers)

#### Framework
- A collection of assets designed to help build sites or applications faster, easier
- Includes CSS grids, javascript libraries or helpful scripts and HTML templates

### 5.3. CSS PreProcessors
- CSS is static stylesheet language, CSS PreProcessors help to write CSS more efficiently, semantically with programming features like variables, functions, maths operations, conditionals etc.
- The scripting language that extends the functionality of CSS and must be compiled into native CSS code before publishing

#### Popular CSS PreProcessors
| CSS PreProcessors  | Source created in        | File conversion           |
| ------------------ |:------------------------:| ------------------------- |
| SASS               | (Written in Ruby)        | .scss / .sass -> .css     |
| Less               | (Written in JavaScript)  | .less -> .css             |
| Stylus             | (Written in JavaScript)  | .styl -> .css             |

### 5.4. XML - eXtensible Markup Language
A semantic markup language containing rules for defining document structure and data and transfer globally (customized tags) and widely used to share data between multiple applications.

```
<?xml version="1.0" ?>

    <studentDetails>

        <name>Test</name>
        <rollNumber>001</rollNumber>

    <studentDetails>
```

### Common uses of AML
- RSS feeds - online contents
- AJAX Applications - store or write data
- Flash/XML
- External APIs

### Associate technologies with XML
- XSL & XSLT
- XPath

### 5.5. AJAX (Asynchronous JavaScript and XML)
- Not a new technology 
- Not a scripting or programming language
- It isn't any one thing at all...!!!
- AJAX is a new technique for creating better, faster, and more Interactive interfaces or web applications with the help of XML, HTML, CSS, and JavaScript Document Object Model (DOM)
- Think AJAX as a new specific approach to web development which focuses on building interactive and engaging web experiences

### 5.6. RSS Feed (Rich Site Summary / Real Simple Syndication / Really Simple Syndication)
- RSS uses a family of standard web feed formats to publish frequently updated information like blog entries, news headlines, audio, video. 
- An RSS document (called "feed", "web feed", or "channel") includes full or summarised text, and metadata, like publishing date and author's name.
- RSS is a standardized XML base format

Section 6. What's Next Step?
=====================
Congratulations! You have completed Web Design Development Foundations-Web Technology Fundamentals lessons. Thank You for looking into Web Fundametals. Now you have a good idea of how web works and technologies behind web. Your next step could be Mastering HTML, lets begin your web design-development journey with [Learning HTML5 Essentials](https://github.com/dinanathsj29/html5-essentials). Best of Luck! Happy Learning!
