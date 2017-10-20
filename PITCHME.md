@title[Rails loving Javascript]
# Rails <span style="color: #e49436">loving</span> Javascript

#### Eine Reise hin und wieder zurück
<br>
<br>
<span style="color: #bbb; font-size: 80%">[Rails, Ruby, jQuery, ES6, NPM, Yarn, Webpack]</span>

---
@title[Rails]
### Es war einmal...
<br>
<ul>
  <li class="fragment"><span style="font-size: 80%">Rails Version 1.0 wurde im Dezember 2005 released</span></li>
  <li class="fragment"><span style="font-size: 80%">2007 Version 2.0 mit REST als Plattform für Web Services</span></li>
  <li class="fragment"><span style="font-size: 80%">Rails 5.1 im April 2017 mit Webpacker und System tests</span></li>
</ul>

Note: 
Representational State Transfer (GET POST PUT DELETE in der HTTP Schicht, zustandslos)

---

## Rails fühlt sich einfach richtig an.

---

### MVC (<span style="color: #e49436">Model View Controller</span>)
<br>
<ul>
  <li class="fragment"><span style="color: #e49436">M</span><span style="font-size: 80%">   ActiveRecord, die ORM-Schicht</span></li>
  <li class="fragment"><span style="color: #e49436">C</span><span style="font-size: 80%">   ActionController, die Steuerungsschicht (auch REST)</span></li>
  <li class="fragment"><span style="color: #e49436">V</span><span style="font-size: 80%">   ActionView, die Präsentationsschicht</span></li>
</ul>

Note:
Datenbanken wie z.B. SQLite, DB2, Informix, MySQL, Oracle, PostgreSQL und Microsoft SQL Server
HTML, XML – z. B. für XHTML und Web Services, JavaScript – RJS-Templates, Binärdaten
Templatesysteme: ERB für (X)HTML und Javascript, Builder für XML, Haml, Sass, CoffeeScript
HTTP-Header manipulieren

---

# Philosophie
<br>
### <span style="color: #e49436">Don’t repeat yourself.</span>
### <span style="color: #e49436">Convention over Configuration.</span>

---
@title[Ruby]

### Ruby
- Entworfen von Yukihiro Matsumoto
- Ziel: Flexibilität, Ausdrucksstärke und Einfachheit |
- Synthese aus Perl, Smalltalk, Eiffel, Ada und Lisp |
- sollte objektorientierter als Python und zugleich mächtiger als Perl sein |

Note:
Wenn du Java, JavaScript, PHP, Perl, oder Python kennst, wird Ruby für dich leicht zu erlernen sein

---
@title[Rails Sample Code]

### <span style="color: #e49436">Lesbarkeit</span>
<br>

```ruby
class Project < ApplicationRecord 
  belongs_to :portfolio

  has_one :project_manager
  has_many :milestones
  has_many :deliverables, through: milestones

  validates :name, :description, presence: true 
  validates :non_disclosure_agreement, acceptance: true 
  validates :short_name, uniqueness: true
end
```

---
@title[Rails Live Code]

### <span style="color: #e49436">Live Code</span>
<br>

```shell
$ rails _5.1.4_ new serom-demo
$ cd serom-demo
$ bin/rails about
$ bin/rails server

open browser http://localhost:3000/
```

+++

```shell
$ bin/rails generate scaffold Product \
            title:string description:text \
            image_url:string price:decimal
```

---
@title[Step 3. Done!]

### <span style="color: #e49436">STEP 3. GET THE WORD OUT!</span>

<br>

<span style="font-size: 1.3em;"><span style="color:white">htt</span><span style="color:white">ps://git</span><span style="color: #e49436">pitch</span><span style="color: white">.com/<span style="color: #e49436">user</span>/<span style="color: #e49436">repo</span>/<span style="color: #e49436">branch</span></span>

<br>

#### Instantly use your GitPitch slideshow URL to promote, pitch or present absolutely anything.

---
@title[Slide Rich]

### <span style="color: #e49436">Slide Rich</span>

#### Code Presenting for Blocks, Files, and GISTs
#### Image, Video, Chart, and Math Slides
#### Multiple Themes With Easy Customization
<br>
#### <span style="color: #e49436">Plus collaboration is built-in...</span>
#### Your Slideshow Is Part Of Your Project
#### Under Git Version Control Within Your Git Repo

---

@title[Feature Rich]

### <span style="color: #e49436">Feature Rich</span>

#### Present Online or Offline
#### With Speaker Notes Support
#### Print Presentation as PDF
#### Auto-Generated Table-of-Contents
#### Share Presentation on Twitter or LinkedIn

---

### Go for it.
### Just add <span style="color: #e49436; text-transform: none">PITCHME.md</span> ;)
<br>
<a style="font-size:0.6em;" href="https://github.com/gitpitch/gitpitch/wiki">[ Click To Learn More On Wiki ]</a>
