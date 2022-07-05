# goit-markup-hw-05

:root {
--main-color: #757575;
--secondary-color: #212121;
--accent-color: #2196f3;
--logo-header-color: #000000;
--footer-color: #ffffff;
--filter-background: #f5f4fa;
--footer-background: #2f303a;
--header-border: #ececec;
--card-border: #eeeeee;
--footer-contacts: rgba(255, 255, 255, 0.6);
--hero-btn-hover: #188ce8;
--icon-color: #afb1b8;
--hero-bckgrnd: #c4c4c4;
--timing-function: cubic-bezier(0.4, 0, 0.2, 1);
}
body {
font-family: "Roboto", sans-serif;
color: var(--main-color);
font-size: 14px;
letter-spacing: 0.03em;
background-color: var(--footer-color);
}
h1,
h2,
h3,
h4,
p,
ul {
margin: 0px;
padding: 0px;
list-style: none;
}
/_ шапка _/
.header-logo {
display: block;
padding-bottom: 25px;
padding-top: 24px;
margin-right: 93px;

color: var(--logo-header-color);
text-decoration: none;
font-family: "Raleway", sans-serif;
font-weight: 700;
font-size: 26px;
line-height: 1.19;
}
.logo-accent {
color: var(--accent-color);
}
.nav-li {
display: block;
padding-top: 32px;
padding-bottom: 32px;

color: var(--secondary-color);
text-decoration: none;
font-weight: 500;
line-height: 1.14;
letter-spacing: 0.02em;

transition: color 250ms var(--timing-function);
}

.current,
.nav-li:hover,
.nav-li:focus,
.contacts-links:hover,
.contacts-links:focus {
color: var(--accent-color);
}
.main-nav-li {
position: relative;
}
.current::after {
position: absolute;
bottom: 0;
content: "";
display: block;
height: 4px;
width: 100%;
background-color: var(--accent-color);
border-radius: 2px;
}

.contacts-links {
display: flex;
align-items: center;
padding-top: 32px;
padding-bottom: 32px;
text-decoration: none;
color: var(--main-color);
font-weight: 500;
line-height: 1.14;
letter-spacing: 0.02em;

transition: color 250ms var(--timing-function);
}
.container {
width: 1200px;
padding-left: 15px;
padding-right: 15px;
margin: auto;
}
.header {
height: 80px;
border-bottom: 1px solid var(--header-border);
}
.main-nav,
.header-contacts,
.nav {
display: flex;
}
.header .container {
display: flex;
justify-content: space-between;
}
.main-nav-li:not(:last-child),
.header-contacts-li:nth-child(1) {
margin-right: 50px;
}
.header-icon {
fill: currentColor;
margin-right: 10px;
}

/_ герой _/

.section {
padding-top: 94px;
padding-bottom: 94px;
}
.section.hero {
max-width: 1600px;
height: 600px;
margin-left: auto;
margin-right: auto;

background-color: var(--hero-bckgrnd);
background-image: linear-gradient(
rgba(47, 48, 58, 0.4),
rgba(47, 48, 58, 0.4)
),
url(../images/hero.jpg);
background-size: cover;
background-repeat: no-repeat;
background-position: center;
padding-top: 200px;
padding-bottom: 200px;
text-align: center;
}
.hero-title {
margin-bottom: 30px;
padding-left: 252px;
padding-right: 252px;
color: var(--footer-color);
font-weight: 900;
font-size: 44px;
line-height: 1.36;
letter-spacing: 0.06em;
text-transform: uppercase;
}
.hero-btn {
min-width: 200px;
padding: 10px 32px;
color: var(--footer-color);
background-color: var(--accent-color);
font-weight: 700;
font-size: 16px;
line-height: 1.88;
letter-spacing: 0.06em;
cursor: pointer;

border-radius: 4px;
border-width: 0px;
box-shadow: 0px 4px 4px rgba(0, 0, 0, 0.15);

transition: background-color 250ms var(--timing-function);
}
.hero-btn:hover,
.hero-btn:focus {
background-color: var(--hero-btn-hover);
}
/_ преимущества _/
.benefits-li-div {
display: flex;
justify-content: center;
align-items: center;
width: 270px;
height: 120px;
margin-bottom: 30px;
background-color: var(--filter-background);
border-radius: 4px;
}
.benefits-title {
margin-bottom: 10px;
color: var(--secondary-color);
font-weight: 700;
font-size: 14px;
line-height: 1.14;
text-transform: uppercase;
}
.benefits-descr {
color: var(--main-color);
line-height: 1.71;
}
.visually-hidden {
position: absolute;
width: 1px;
height: 1px;
margin: -1px;
border: 0;
padding: 0;

white-space: nowrap;
clip-path: inset(100%);
clip: rect(0 0 0 0);
overflow: hidden;
}
.benefits-ul {
display: flex;
}
.benefits-li {
width: 270px;
}
.benefits-li:not(:last-child) {
margin-right: 30px;
}
/_ чем мы занимаемся,
наша команда_/
.section.activities {
padding-top: 0px;
}
.activities-title,
.team-title,
.clients-title {
margin-bottom: 50px;
color: var(--secondary-color);
font-weight: 700;
font-size: 36px;
line-height: 1.17;
text-align: center;
}
.activities-li {
display: block;
}
.activities-ul {
display: flex;
justify-content: space-between;
}
.activities-overlay {
position: relative;
}
.activities-text {
position: absolute;
bottom: 0;
width: 100%;
height: 70px;
display: flex;
align-items: center;
justify-content: center;

font-weight: 700;
line-height: 1.14;
text-transform: uppercase;
color: var(--footer-color);
background-color: rgba(47, 48, 58, 0.8);
}
/_ наша команда _/
.team {
padding-top: 94px;
padding-bottom: 94px;
background-color: var(--filter-background);
}
.team-name {
margin-bottom: 10px;
color: var(--secondary-color);
font-weight: 500;
font-size: 16px;
line-height: 1.19;
}
.job-title {
margin-bottom: 16px;
color: var(--main-color);
font-size: 16px;
line-height: 1.19;
}
.team-ul {
display: flex;
justify-content: space-between;
}
.team-card {
padding-top: 30px;
padding-bottom: 30px;
text-align: center;
}
.team-item {
box-shadow: 0px 1px 3px rgba(0, 0, 0, 0.12), 0px 1px 1px rgba(0, 0, 0, 0.14),
0px 2px 1px rgba(0, 0, 0, 0.2);
border-radius: 0px 0px 4px 4px;
background-color: var(--footer-color);
}
.ellipse {
display: flex;
justify-content: center;
align-items: center;
width: 44px;
height: 44px;
border-radius: 50%;
transition: background-color 250ms var(--timing-function);
}
.socials {
display: flex;
padding-left: 32px;
padding-right: 32px;
justify-content: space-between;
}
.team-icon {
fill: var(--icon-color);
transition: fill 250ms var(--timing-function);
}
.social-link:hover .ellipse,
.social-link:focus .ellipse {
background-color: #2196f3;
}
.social-link:hover .team-icon,
.social-link:focus .team-icon {
fill: var(--footer-color);
}

/_ Постоянные клиенты _/

.clients-list {
display: flex;
justify-content: space-between;
}
.rectangle {
display: flex;
justify-content: center;
align-items: center;
width: 170px;
height: 92px;

border: 1px solid var(--icon-color);
border-radius: 4px;

transition: border-color 250ms var(--timing-function);
}
.clients-icon {
fill: var(--icon-color);
transition: fill 250ms var(--timing-function);
}
.clients-link:hover .clients-icon,
.clients-link:focus .clients-icon {
fill: var(--accent-color);
}
.clients-link:hover .rectangle,
.clients-link:focus .rectangle {
border-color: var(--accent-color);
}
/_ подвал _/

.footer {
padding-top: 60px;
padding-bottom: 60px;
background-color: var(--footer-background);
}
.footer-logo {
display: inline-block;
margin-bottom: 20px;
font-family: "Raleway", sans-serif;
color: var(--footer-color);
text-decoration: none;
font-weight: 700;
font-size: 26px;
line-height: 1.19;
}
.footer-adress {
color: var(--footer-color);
font-style: normal;
line-height: 1.71;
}
.footer-contacts {
text-decoration: none;
color: var(--footer-contacts);
transition: color 250ms var(--timing-function);
}
.adress-item:nth-child(-n + 2) {
margin-bottom: 9px;
}
.footer-contacts:hover,
.footer-contacts:focus {
color: var(--accent-color);
}
.footer-right {
min-width: 206px;
}
.footer .ellipse {
background-color: rgba(255, 255, 255, 0.1);
}
.footer .team-icon {
fill: var(--footer-color);
}
.footer-left {
min-width: 231px;
margin-right: 70px;
}
.footer .socials {
padding-left: 0px;
padding-right: 0px;
}
.footer .container {
display: flex;
align-items: baseline;
}
.appeal {
margin-bottom: 20px;
text-transform: uppercase;
color: var(--footer-color);
font-weight: 700;
line-height: 1.14;
}

/_ СТРАНИЦА ПОРТФОЛИО _/
.portfolio {
padding: 94px inherit;
}
.filter-ul {
display: flex;
justify-content: center;
margin-bottom: 50px;
}
.filter-li:not(:last-child) {
margin-right: 8px;
}
.portfolio-btn {
min-width: 73px;
padding: 6px 22px;
color: var(--secondary-color);
background-color: var(--filter-background);
cursor: pointer;
font-weight: 500;
font-size: 16px;
line-height: 1.62;
border-width: 0px;
border-radius: 4px;
box-shadow: none;

transition: color 250ms var(--timing-function),
background-color 250ms var(--timing-function),
box-shadow 250ms var(--timing-function);
}
.portfolio-btn:hover,
.portfolio-btn:focus {
color: var(--footer-color);
background-color: var(--accent-color);
box-shadow: 0px 3px 1px rgba(0, 0, 0, 0.1), 0px 1px 2px rgba(0, 0, 0, 0.08),
0px 2px 2px rgba(0, 0, 0, 0.12);
}
.portfolio-list {
display: flex;
flex-wrap: wrap;
}
.portfolio-list-item {
flex-basis: calc((100% - 60px) / 3);
margin-right: 30px;
margin-bottom: 30px;
}
.portfolio-list-item:nth-child(3n) {
margin-right: 0px;
}
.portfolio-list-item:nth-child(n + 7) {
margin-bottom: 0px;
}
.pic {
display: block;
max-width: 100%;
height: auto;
}

.portfolio-overlay {
position: relative;
overflow: hidden;
}
.portfolio-overlay-text {
position: absolute;
bottom: 0;
padding: 63px 24px;
width: 100%;
height: 100%;
font-size: 18px;
line-height: 1.56;
color: var(--footer-color);
background-color: rgba(33, 150, 243, 0.9);

transform: translateY(101%);
transition: transform 250ms var(--timing-function);
}
.portfolio-list-item:hover .portfolio-overlay-text {
transform: translateY(0);
}

.card-bottom {
padding-bottom: 20px;
padding-top: 20px;
padding-left: 24px;
border: 1px solid var(--card-border);
border-top-width: 0px;
}
.portfolio-list-title {
margin-bottom: 4px;
color: var(--secondary-color);
font-weight: 700;
font-size: 18px;
line-height: 2;
letter-spacing: 0.06em;
}
.portfolio-list-descr {
color: var(--main-color);
font-size: 16px;
line-height: 1.88;
}
.portfolio-link {
display: block;
text-decoration: none;
box-shadow: none;
transition: box-shadow 250ms var(--timing-function);
}
.portfolio-link:hover,
.portfolio-link:focus {
box-shadow: 0px 1px 1px rgba(0, 0, 0, 0.12), 0px 4px 4px rgba(0, 0, 0, 0.06),
1px 4px 6px rgba(0, 0, 0, 0.16);
}

/_ моадльное окно _/
.backdrop {
position: fixed;
top: 0;
left: 0;
width: 100%;
height: 100%;
background-color: rgba(0, 0, 0, 0.2);
opacity: 1;
transition: opacity 250ms var(--timing-function);
}
.backdrop.is-hidden {
opacity: 0;
pointer-events: none;
}
.backdrop.is-hidden .modal {
transform: translate(-50%, -50%) scale(2);
}
.modal {
position: absolute;
top: 50%;
left: 50%;
transform: translate(-50%, -50%) scale(1);
min-width: 528px;
min-height: 581px;

background-color: var(--footer-color);
box-shadow: 0px 1px 3px rgba(0, 0, 0, 0.12), 0px 1px 1px rgba(0, 0, 0, 0.14),
0px 2px 1px rgba(0, 0, 0, 0.2);
border-radius: 4px;
transition: transform 250ms var(--timing-function);
}
.close-btn {
position: absolute;
right: 8px;
top: 8px;
width: 30px;
height: 30px;
border: 1px solid rgba(0, 0, 0, 0.1);
background-color: var(--footer-color);
border-radius: 50%;
cursor: pointer;
}
.modal-icon {
position: absolute;
left: 50%;
top: 50%;
transform: translate(-50%, -50%);
}
