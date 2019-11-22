<template>
  <div class="main-wrapper">
    <nav class="navbar navbar-expand-lg navbar-dark bg-primary fixed-top" id="sideNav">
      <a class="navbar-brand js-scroll-trigger" href="#about">
        <span class="d-block d-lg-none">MIKA LEHTINEN</span>
        <span class="d-none d-lg-block">
          <img class="img-fluid img-profile rounded-circle mx-auto mb-2" src="./assets/mika.jpg" alt="">
        </span>
      </a>
      <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarSupportedContent">
        <ul class="navbar-nav">
          <li class="nav-item">
            <a class="nav-link js-scroll-trigger" href="#about">About</a>
          </li>
          <li class="nav-item">
            <a class="nav-link js-scroll-trigger" href="#experience">Experience</a>
          </li>
          <li class="nav-item">
            <a class="nav-link js-scroll-trigger" href="#education">Education</a>
          </li>
          <li class="nav-item">
            <a class="nav-link js-scroll-trigger" href="#skills">Skills</a>
          </li>
          <li class="nav-item">
            <a class="nav-link js-scroll-trigger" href="#Work">Work</a>
          </li>
          <li class="nav-item">
            <a class="nav-link js-scroll-trigger" href="#interests">Interests</a>
          </li>
        </ul>
      </div>
    </nav>

    <div class="container-fluid p-0">

      <section class="resume-section p-3 p-lg-5 d-flex d-column" id="about">
        <div class="my-auto">
          <h1 class="mb-0">{{ name }}
            <span class="text-primary">{{ surname }}</span>
          </h1>
          <div class="subheading mb-5">{{ address }}
            <a href="mailto:name@email.com">{{ email }}</a>
          </div>
          <p class="mb-5">{{ aboutMe }}</p>
          <ul class="list-inline list-social-icons mb-0">
            <li class="list-inline-item">
              <a href="mailto:mika@lehtidigital.se">
                <span class="fa-stack fa-lg">
                  <i class="fa fa-circle fa-stack-2x"></i>
                  <i class="fa fa-envelope fa-stack-1x fa-inverse"></i>
                </span>
              </a>
            </li>
            <li class="list-inline-item">
              <a href="https://www.linkedin.com/in/mika-lehtinen-48a33488/" target="_blank">
                <span class="fa-stack fa-lg">
                  <i class="fa fa-circle fa-stack-2x"></i>
                  <i class="fa fa-linkedin fa-stack-1x fa-inverse"></i>
                </span>
              </a>
            </li>
            <li class="list-inline-item">
              <a href="http://github.com/mikalehti" target="_blank">
                <span class="fa-stack fa-lg">
                  <i class="fa fa-circle fa-stack-2x"></i>
                  <i class="fa fa-github fa-stack-1x fa-inverse"></i>
                </span>
              </a>
            </li>
          </ul>
        </div>
      </section>

      <section class="resume-section p-3 p-lg-5 d-flex flex-column" id="experience">
        <div class="my-auto">
          <h2 class="mb-5">Experience</h2>

          <div class="resume-item d-flex flex-column flex-md-row mb-5" v-for="job in experience" :key="job.description">
            <div class="resume-content mr-auto">
              <h3 class="mb-0">{{ job.position }}</h3>
              <div class="subheading mb-3">{{ job.company }}</div>
              <p>{{ job.description }}</p>
            </div>
            <div class="resume-date text-md-right">
              <span class="text-primary">{{ job.startDate }} - {{ job.endDate }}</span>
            </div>
          </div>

        </div>

      </section>

      <section class="resume-section p-3 p-lg-5 d-flex flex-column" id="education">
        <div class="my-auto">
          <h2 class="mb-5">Education</h2>

          <div class="resume-item d-flex flex-column flex-md-row mb-5">
            <div class="resume-content mr-auto">
              <h3 class="mb-0">Medieinstitutet Malmö</h3>
              <div class="subheading mb-3">Web development</div>
              <div>2 year program in web development primarily focused on backend.</div>
            </div>
            <div class="resume-date text-md-right">
              <span class="text-primary">August 2017 - May 2019</span>
            </div>
          </div>
          <hr>
          <div class="resume-item d-flex flex-column flex-md-row mb-5">
            <div class="resume-content mr-auto">
              <h3 class="mb-0">Malmö University</h3>
              <div class="subheading mb-3">Computer Sience - Game Development</div>
              <p>40 credits in computer sience</p>
            </div>
            <div class="resume-date text-md-right">
              <span class="text-primary">August 2014 - January 2015</span>
            </div>
          </div>
          <hr>
          <div class="resume-item d-flex flex-column flex-md-row mb-5">
            <div class="resume-content mr-auto">
              <h3 class="mb-0">Nicolaiskolan Helsingborg</h3>
              <div class="subheading mb-3">High school - Business and administration</div>
              <p>3 year program in business and administration</p>
            </div>
            <div class="resume-date text-md-right">
              <span class="text-primary">August 2017 - June 2010</span>
            </div>
          </div>

        </div>
      </section>

      <section class="resume-section p-3 p-lg-5 d-flex flex-column" id="skills">
        <div class="my-auto">
          <h2 class="mb-5">Skills</h2>
          <div class="subheading mb-3">What you can expect from me</div>
          <ul class="fa-ul mb-0">
            <li>
              <i class="fa-li fa fa-check"></i>
              Comfortable working with agile methods</li>
            <li>
              <i class="fa-li fa fa-check"></i>
              Building functional and beautiful applications</li>
            <li>
              <i class="fa-li fa fa-check"></i>
              Working with a team of developers</li>
            <li>
              <i class="fa-li fa fa-check"></i>
              Always hungry to learn more</li>
            <li>
              <i class="fa-li fa fa-check"></i>
              ALOT of coffee drinking</li>
          </ul>
          <br>
          <div class="subheading mb-3">Technologies I'm working with
          <ul class="list-inline list-icons">
            <li class="list-inline-item">
              <a href="https://laravel.com/" target="_blank" class="devicon-laravel-plain colored"></a>
            </li>
            <li class="list-inline-item">
              <a href="https://vuejs.org/" target="_blank" class="devicon-vuejs-plain colored"></a>
            </li>
            <li class="list-inline-item">
              <a href="https://jquery.com/" target="_blank" class="devicon-jquery-plain-wordmark colored"></a>
            </li>
            <li class="list-inline-item">
              <a href="https://sass-lang.com/" target="_blank" class="devicon-sass-original colored"></a>
            </li>
            <li class="list-inline-item">
              <a href="https://sv.wordpress.org/" target="_blank" class="devicon-wordpress-plain colored"></a>
            </li>
            <li class="list-inline-item">
              <a href="https://www.mysql.com/" target="_blank" class="devicon-mysql-plain colored"></a>
            </li>
            <li class="list-inline-item">
              <i class="devicon-git-plain colored"></i>
            </li>
          </ul>
          </div>
        </div>
      </section>

      <section class="resume-section p-3 p-lg-5 d-flex flex-column" id="Work">
        <div class="my-auto">
          <h2 class="mb-5">Reference work</h2>
          <div class="thesis">
            <div class="subheading mb-3">Thesis. Laravel/Vue chat application </div>
            <p>Github link to a chat application that was made with Laravel/Vue.js powered by pusher for my thesis in school. Complete source code is available on the link below.</p>
            <a href="https://github.com/mikalehti/Laravelchatwcm17" class="btn btn-primary" role="button" target="_blank">View Github</a>
          </div>
          <hr>
          <div class="oldpage">
            <div class="subheading mb-3">Old website design</div>
            <p>My old website design custom made with PHP and Jquery powered by Wordpress. It was a presentation website much like this, the website's source code is available on the link below.</p>
            <!-- <a href="/web/viewer.html?file=old_website.pdf" class="btn btn-primary" role="button" target="_blank">View Project</a> -->
            <a href="https://github.com/amlstudio/AML-theme-repo" class="btn btn-primary" role="button" target="_blank">View Github</a>
          </div>
          <hr>
          <div class="bombdefuser">
            <div class="subheading mb-3">Bomb Defuser</div>
            <p>A platform game where you're supposed to get to the end of the level and defuse the bomb before the time run out. We created this game as a group project in school where I primarily worked on the level editor and drew alot of the graphics and created a 3D-rendered animation scene.</p>            </div>
            <a href="https://play.google.com/store/apps/details?id=com.BombDefuser.android&hl=sv" class="btn btn-primary" role="button" target="_blank">View Project</a>
        </div>
      </section>
      <section class="resume-section p-3 p-lg-5 d-flex flex-column" id="interests">
        <div class="my-auto">
          <h2 class="mb-5">Interests</h2>
          <p>Apart from web development I have a general passion for technology, I enjoy experimenting with computers and software of all aspects. I do also enjoy art in the form of sketching and 3D-modeling. I love reading about new and exciting technologies in the web development world and explore them more in-depth. </p>
          <p class="mb-0">As for outdoor activites, I'm a skateboarder and have been riding my board for well over 10 years. I do also enjoy an occasional walk in the forest. I believe its key to keep your body healthy in order to have a healthy mind.</p>
        </div>
      </section>
    </div>
  </div>
</template>

<script>
export default {
  data () {
    return {
      title: 'Mika Lehtinen',
      name: 'MIKA',
      surname: 'LEHTINEN',
      address: 'Web developer · Sweden, Helsingborg · (+46)731 55 22 13 ·',
      email: 'mika@lehtidigital.se',
      aboutMe: "My name is Mika and I'm 28 years old. I'm a web developer with great passion for information and design and always strive to create beautiful and robust software.  I'm very passionate about technology and I love working alongside other developers that feel the same as I do about the products that we're creating.",
      experience: [
        {
          position: 'Technical specialist / UX-analytic',
          company: 'Bofakta AB',
          description: 'Was attending a dozen fairs across the country where my primary role was to showcase the system for the visitors and guiding them through testing it. I was also analyzing the user experience for the application and answered techincally related questions.',
          startDate: 'Octobre 2018',
          endDate: 'January 2019'
        },
        {
          position: 'Web Developer Intern',
          company: 'Bofakta AB',
          description: 'Working with backend-development on their current system where I mostly fixed existing bugs and built new functionality. I was also in charge for a project where I was creating a prototype for a external system that generates documents.',
          startDate: 'July 2018',
          endDate: 'November 2018'
        }
      ]
    }
  },
  mounted () {
    const $ = this.jquery
    this.$nextTick(() => {
      $('a.js-scroll-trigger[href*="#"]:not([href="#"])').click(function () {
        if (location.pathname.replace(/^\//, '') === this.pathname.replace(/^\//, '') && location.hostname === this.hostname) {
          var target = $(this.hash)
          target = target.length ? target : $('[name=' + this.hash.slice(1) + ']')
          if (target.length) {
            $('html, body').animate({
              scrollTop: (target.offset().top)
            }, 1000, 'easeInOutExpo')
            return false
          }
        }
      })
      $('.js-scroll-trigger').click(function () {
        $('.navbar-collapse').collapse('hide')
      })
      $('body').scrollspy({
        target: '#sideNav'
      })
    })
  }
}
</script>
