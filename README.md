<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Patel Farhan</title>
    <link rel="stylesheet" href="style.css">
    <script src="https://kit.fontawesome.com/a339054b85.js" crossorigin="anonymous"></script>

</head>

<body>
    <DIV id="header">
        <div class="container">
            <nav>
                <img src="image/logo.jpeg" class="logo">
                <ul id="sidemenu">
                    <li><a href="#header">Home</a></li>
                    <li><a href="#about">About</a></li>
                    <li><a href="#services">Services</a></li>
                    <li><a href="#portfoilo">Portfoilo</a></li>
                    <li><a href="#contact">Contact</a></li>
                    <i class="fa-solid fa-circle-xmark" onclick="closemenu()"></i>
                </ul>
                <i class="fa-solid fa-bars" onclick="openmenu()"></i>
            </nav>
            <div class="header-text">
                <p>Webpage Designer</p>
                <h1>Hi, I'm <span>PATEL FARHAN</span><br>From India</h1>
            </div>
        </div>
    </DIV>
    <!----------about---------->
    <div id="about">
        <div class="container">
            <div class="row">
                <div class="about-col-1">
                    <img src="image/user.jpg">
                </div>
                <div class="about-col-2">
                    <h1 class="sub-title">About Me</h1>
                    <P>Hi, I am Patel Farhan, current webpage Designer, from '<span class="a">IN</span><span class="b">D</span><span class="c">IA</span>'.</P>
                    <div class="tab-titles">
                        <p class="tab-links active-link" onclick="opentab('Skills')">Skills</p>
                        <p class="tab-links" onclick="opentab('experience')">Experience</p>
                        <p class="tab-links" onclick="opentab('education')">Education</p>
                    </div>
                    <div class="tab-contents active-tab" id="skills">
                        <ul>
                            
                            <li><span>Web Designing</span><BR>Webpage  Designing</li>
                            <li><span>App Development</span><BR>Building Android/ios apps</li>
                        </ul>
                    </div>
                    <div class="tab-contents" id="experience">
                        <ul>
                        <li><span>current</span><br>Intership at TECHOMAX Solution. </li>
                        </ul>
                    </div>
                    <div class="tab-contents" id="education">
                        <ul>
                            <li><span>2022</span><BR>WEB Designing Training at TECHOMAX Solution</li>
                            <li><span>current</span><BR>Diploma from Shri K.J.polytechnic, Bharuch</li>
            
                        </ul>
                    </div>
                </div>

            </div>
        </div>
    </div>
    <!-- services -->
    <div id="services">
        <div class="container">
            <h1 class="sub-title">My Services</h1>
            <div class="services-list">
                <div>
                    <i class="fa-solid fa-code"></i>


                    <h2>Webpage Designing</h2>
                    <p>Webpage design is the process of planning,conceptualing,and arranging content online</p>
                    <a href="#">Learn more</a>

                </div>
                <div>

                    <i class="fa-brands fa-app-store-ios"></i>

                    <h2>App developer</h2>
                    <p>Mobile app development is the act or process by which a mobile app devoloped for  mobile devices.</p>
                    <a href="#">Learn more</a>

                </div>

            </div>
        </div>

    </div>
    <!-- Portfoilo -->
    <div id="portfoilo">
        <div class="container">
            <h1 class="sub-title">My Work</h1>
            <div class="work-list">
                <div class="work">
                    <img src="image/web1.jpg">
                    <div class="layer">
                        <h3>Social Media websites</h3>
                        <p>The websites connect you all around the world.</p>
                        <a href="#"> <i class="fa-solid fa-up-right-from-square"></i></a>





                    </div>
                </div>
                <div class="work">
                    <img src="image/web2.jpg">
                    <div class="layer">
                        <h3> Apps developer</h3>
                        <p>The app connect you all around the world.</p>
                        <a href="#"> <i class="fa-solid fa-up-right-from-square"></i>
                        </a>

                    </div>
                </div>
            </div>
            <a href="#" class="btn"> See more</a>
        </div>
    </div>
    <!-- contact -->
    <div id="contact">
        <div class="container">
            <div class="row">
                <div class="contact-left">
                    <h1 class="sub-title">Contact Me</h1>
                    <p> <i class="fa-solid fa-paper-plane"></i>patelfarhan166@gmail.com</p>
                    <p><i class="fa-solid fa-phone"></i> 7487999818</p>
                    <div class="social-icons">
                        <a href=""><i class="fa-brands fa-facebook"></i></a>
                        <a href="https://instagram.com/patel__farhan_"><i class="fa-brands fa-instagram"></i></a>
                        <a href=""><i class="fa-brands fa-twitter"></i></a>
                    </div>
                    <a href="images/my-cv.pdf" download class="btn btn2">Download CV</a>
                </div>

                <div class="contact-right">
                    <form name="submit-to-google-sheet">
                        <input type="text" name="Name" placeholder="Your Name" required>
                        <input type="email" name="Email" placeholder="Your Email" required>
                        <textarea name="Message" rows="6" placeholder="Your Message"></textarea>
                        <button type="submit" class="btn btn2" >Submit</button>
                    </form>
                    <span id="msg"></span>
                </div>
            </div>
        </div>
        <div class="copyright">
            <p>copyright <i class="fa-solid fa-copyright"></i>
             Het. Mode with <i class="fa-solid fa-heart"></i>

                internet Solution. </p>
        </div>
    </div>

    <script>
        var tablinks = document.getElementsByClassName("tab-links");
        var tabcontents = document.getElementsByClassName("tab-contents");

        function opentab(tabname) {
            for (tablink of tablinks) {
                tablink.classList.remove("active-link");
            }
            for (tabcontent of tabcontents) {
                tabcontent.classList.remove("active-tab");
            }
            event.currentTarget.classList.add("active-link");
            document.getElementById(tabname).classList.add("active-tab");
        }
    </script>
    <script>
        var sidemenu=document.getElementById("sidemenu");
        function openmenu(){
            sidemenu.style.right="0";

        }
        function closemenu(){
            sidemenu.style.right="-200px";
        }
    </script>
    <script>
        const scriptURL = 'https://script.google.com/macros/s/AKfycbyXns4rqLD1M_TMsz9DOoR5MD4W6yKzTAkQhSclqkuKf5Owj-XevxdimlobsWe2Yrcjfw/exec'
        const form = document.forms['submit-to-google-sheet']
        const msg = document.getElementById("msg")
        form.addEventListener('submit', e => {
          e.preventDefault()
          fetch(scriptURL, { method: 'POST', body: new FormData(form)})
            .then(response => {
                msg.innerHTML="Message sent successfully"
                setTimeout(function(){
                    msg.innerHTML = ""
                },5000)
                form.reset()
            })
            .catch(error => console.error('Error!', error.message))
        })
      </script>
      
</body>

</html>
