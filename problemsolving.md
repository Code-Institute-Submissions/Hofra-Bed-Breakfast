# logo-img

## Position not centered

    index.html
    <div>
        <a href="valkommen.html">
            <img class="logo-img" src="./image/logo.png" alt="Hofra B&B Breakfast">
        </a>
    </div>

    stylesheet.css
    .logo-img {
        heigth: 150px;
        position: center;
    }


    Result after research thru old repositories, Google and testing

    index.html
    <div class="logo-img">&nbsp;
        <a href="valkommen.html"></a>
    </div>

    stylesheet.css
    .header-logo {
        background: url("../images/logo.png");
        background-repeat: no-repeat;
        background-size: contain;
        background-position: center;
        margin-top: 10px;
        min-height: 14vh;
    }

## Logo image link to index.html not working

    The link to the index.html was not working at all
    index.html
    <div class="logo-img">&nbsp;
        <a href="valkommen.html"></a>
    </div>

    The code was changed to after checking with Slack, Jim Morel, Slack username: JimLynx_lead, and it works fine. Changed also the code in the footer.

    <a href="index.html">
        <div class="container-fluid header-logo">&nbsp;</div>
    </a> 

# Navigation bar

## Navigation bar used from Bootstrap "Navs" 
    When adding class= "Navbar", to add my own class name, the navigation items jumped from center to left side. After checking Bootstrap I noticed that Bootstrap is using this for its "Navbar's".
    Removed the class in total.

    Can't get space inbetwen nav-items
    Tried with different class path but nothing works.
    Wrote a message on Slack, suggestion was made to target .nav-item which I already tried which was not working.
    Jim Morel, Slack username: JimLynx_lead, and I had a short call to fix the issue but I run out of credits on Gitpod. Issue still alive.

    Issue solved by changing the comment in stylesheet.css from <--- ---> to /* */.

## Navigation bar on smaller screen don't get horizontal

    Tried with flexbox but no response. Tried to cut the div outside the <nav> but still no response.
    Ask Slack for help. Anthony O'Brien, Slack username: Anthony(finsishedCourse, stillJinja) and I had a live call in Slack.
    The issue seemed to be that bootstrap for some reason added a padding in the column line so it used the whole width of the row.
    The solution was to move the classes d-block and d-sm-none from .row to .col-4 line.

# Hero Image Welcome

## hero-image-welcome was not responsive
    To seperate the hero images for the different features I added the welcome to the class hero-image-welcome. I did change the class in the stylesheet but not for the responsive design.
    The solution was to correct all hero-image classes.


# Features

## Features of The barn had different sizes
    The features for the two packages had different heigth due to less text in one of them. I found a simple solution on Slack, using the class name cards.


# Quotes

## Quotes image and quotes will not wrap
    Changed class col-lg-6 to col-md-6 but forgot to check if this will effect anything in the stylesheet.
    After correcting class name in stylesheet it worked again.
    