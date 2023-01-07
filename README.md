# Cobh Children's Theatre

Cobh Children's Theatre is a  children's club website. Its primary goal is to provide information for the current members and future members alike. It is essentially a one stop shop for dance, speech and drama, music, and all kind of performing arts for children. It caters for children ages 4-12. The club run classes and activities all year round, including easter and summer camps. The club's ultimate goal is to provide a safe, fun and exciting environment for children so they can explore,grow, discover and reach their full potential while having the time of their lives. View the live website [here] ( https://aylamccarthy.github.io/cobh-childrens-theatre/)

![Mockup](docs/readme_images/mockup.png)

Features
Site wide
Navigation Menu
Contains links to the Home, Gallery and sign Up pages and will be responsive on all devices.
This will allow users to easily navigate between the pages within the site on any size device.
Nav Menu

Footer
This will contain icons as links to social media websites that will open in new tabs. Icons will be accessible to the visually impaired who may be using a screen reader, by the use of aria labels. The first part of the footer will contain contact information for 'Cobh Children's Theatre'.
This will allow the user to follow 'Cobh Children's Theatre' on various social media where they can get more up to date information that may not be displayed on the website. The contact information will allow the user to contact the club directly.
Footer


Landing Page
Landing page image
This is an image of our two gorgeous girl memebers performing.
This will help to immediately show and entice the user what the website is about and how much fun their children will have should they decide to sign them up.
Landing Page Image

Website information on 'Cobh Children's Theatre'
Information about the club and the websites purpose including the benefits all the acitivities can have on their members.
This information lets the user know what the site is about.


Sign Up form
A sign up form will be implemented to allow users to sign up to the club. The form will consist of the following fields and attributes:
Child's Name (required, type=text)
Parent/Guardian's Full Name (required, type=text)
Contact Number (required, type=tel)
Email (required, type=email)
On successful submission of the Sign form, the user will be navigated to contact.html displaying a success message.
This will allow user to contact the club if they have any queiries about the club, information about all the activities or membership.
Sign Up Form

Sign Up Form Received

Gallery Page
Gallery
The gallery will provide the user with photos of the club members in action.
This will give the user a glimpse of how much fun and exciting it is to be a member of the club.
Gallery




Details Dropdown

Existing Features
Responsive design
Sign up form and success page
Features Left to Implement
As a future enhancement, the Sign up form will be updated with javascript to send an email to the club with the contact information.


Design
Wireframes

Home page

Home Page large screen

Home Page small screen

Contact form successful submission page.

Contact form submission success

Contact form submission success

Adventures page

Adventures page large screen

Adventures page small screen

Gallery page

Gallery page large screen

Gallery page small screen

404 page

Gallery page large screen

Gallery page small screen




Technologies
HTML
The structure of the Website was developed using HTML as the main language.
CSS
The Website was styled using custom CSS in an external file.
GitHub
Source code is hosted on GitHub and delpoyed using Git Pages.
Git
Used to commit and push code during the development opf the Website
Font Awesome
Icons obtained from https://fontawesome.com/ were used as the Social media links in the footer section.
Tinyjpg
https://tinyjpg.com/ was used to reduce the size of the images used throughout the website
balsamiq
wireframes were created using balsamiq from https://balsamiq.com/wireframes/desktop/#
Testing
Responsiveness
All pages were tested to ensure responsiveness on screen sizes from 320px and upwards as defined in WCAG 2.1 Reflow criteria for responsive design on Chrome, Edge, Firefox and Opera browsers.

Steps to test:

Open browser and navigate to Cobh Children's Theatre
Open the developer tools (right click and inspect)
Set to responsive and decrease width to 320px
Set the zoom to 50%
Click and drag the responsive window to maximum width
Expected:

Website is responsive on all screen sizes and no images are pixelated or stretched. No horizontal scroll is present. No elements overlap.

Actual:

Website behaved as expected with the exception of switching to landscape view in Mozilla Firefox. Details can be found in Unfixed Bugs


Accessibility
Wave Accessibility tool was used throughout development and for final testing of the deployed website to check for any aid accessibility testing.

Testing was focused to ensure the following criteria were met:

All forms have associated labels or aria-labels so that this is read out on a screen reader to users who tab to form inputs
Color contrasts meet a minimum ratio as specified in WCAG 2.1 Contrast Guidelines
Heading levels are not missed or skipped to ensure the importance of content is relayed correctly to the end user
All content is contained within landmarks to ensure ease of use for assistive technology, allowing the user to navigate by page regions
All not textual content had alternative text or titles so descriptions are read out to screen readers
HTML page lang attribute has been set
Aria properties have been implemented correctly
WCAG 2.1 Coding best practices being followed
Manual tests were also performed to ensure the website was accessible as possible and an accessibility issue was identified.

Issue #1: Use of hidden check boxes and labels for the gallery filter and accordion on the gallery page were not accessible via the keyboard due to the property display: none;

Fix: I could not find a way to fix this issue with html and css alone so a tabindex of 0 was added to allow the label to be tabbed to and an onkeypress event to target and click the correct checkbox was implemented. Javascript code was taken from this Mozilla Doc

Issue #2: After keyboard controls were implemented, while testing the site with windows 'Narrator' screenreader, it was not clearly known what the purpose of the labels/checkboxes were. An aria-label label was added to the labels for screen readers to alert them that the labels were clickable and what their purpose was.

Lighthouse Testing
Home

Gallery

Adventures

Functional Testing
Navigation Links

Testing was performed to ensure all navigation links on the respective pages, navigated to the correct pages as per design. This was done by clicking on the navigation links on each page.

Navigation Link	Page to Load
Home	index.html
Sign Up	sign-up.html
Gallery	gallery.html
Links on all pages navigated to the correct pages as expected.

Form Testing

The form on the sign up page was tested to ensure it functioned as expected when correct data was input and when incorrect data was input. The following test scenarios were covered:

Scenario One - Correct Inputs

Steps to test:

Navigate to Cobh Childrens Theatre - Sign Up Page
Scroll down to the form and input the following data:
Child's Name: John
Parent/Guardian's Full Name: Mike McCarthy
Email: mmcarthy@gmail.com
Click Submit
User should be redirected to contact.html confirmation page
Expected:

Form submits with no warnings or errors and user is redirected to contact.html confirmation page.

Actual:

Website behaved as expected with no errors or warnings and redirected to contact.html.

Scenario Two - Missing Required Field First Name

Steps to test:

Navigate to Tacos Travels - Home Page
Scroll down to the form and input the following data:
First Name:
Last Name: 
Email: doe.
Click Submit
Expected:

The form does not submit and an Error is displayed to tell the user that the field is required.

Actual:

Website behaved as expected, error message was displayed and the form did not submit.

Scenario Three - Missing Required Field Last Name

Steps to test:

Navigate to Cobh Children's Theatre - Home Page
Scroll down to the form and input the following data:
First Name:Mike
Last Name:
Email: mmcarthy@gmail.com

Click Submit
Expected:

The form does not submit and an Error is displayed to tell the user that the field is required.

Actual:

Website behaved as expected, error message was displayed and the form did not submit.

Scenario Four - Missing Required Field Email

Steps to test:

Navigate to  Cobh Children's Theatre- Home Page
Scroll down to the form and input the following data:
First Name:John
Last Name: Mike
Email:
Click Submit
Expected:

The form does not submit and an Error is displayed to tell the user that the field is required.

Actual:

Website behaved as expected, error message was displayed and the form did not submit.

Scenario Six - Incorrect email format

Steps to test:

Navigate to Cobh Children's Theatre - Home Page
Scroll down to the form and input the following data:
First Name:John
Last Name: Mike
Email: mmcarthy.gmail.com
Click Submit
Expected:

The form does not submit and an Error is displayed to tell the user that a valid email is required and the format it should be in.

Actual:

Website behaved as expected, error message was displayed and the form did not submit.

Footer Social Media Icons / Links

Testing was performed on the Font Awesome Social Media icons in the footer to ensure that each one opened in a new tab and that each one had a hover affect of the orange branding color.

Each item opened a new tab when clicked as expected and correct hover color was present.

Footer Contact Information

Testing was performed on the phone number in the contact information section of the footer to ensure behaviour was as expected.

Steps to test Telephone Number

Navigate to Cobh Children's Theatre - Home Page
Click the phone number in the footer (01 123 456 789)
Expected:

A window is opened asking which device you would like to call from.

Actual:

Behavior was as expected and the window presented me with the following option to call:

Mobile Phone 0871376895

Steps to test Email Link

Navigate to Cobh Children's Theatre- Home Page
Click the email address in the footer (info.cobhtheatre@gmail.com)
Expected:

A windows popup is displayed asking what application you would like to send a mail from or your default email application is opened.

Actual:

Behavior was as expected and my outlook application was opened ready to send an email to the target address.

Validator Testing
HTML
No errors were returned when passing through the official W3C validator
Contact HTML Validator Results

Sign up HTML Validator Results

Home HTML Validator Results

Gallery HTML Validator Results


CSS
No errors were found when passing through the official (Jigsaw) validator
CSS Validator Results

Unfixed Bugs
Responsiveness of the website worked on all devices, screen sizes and orientation with the exception of landscape orientation on mozilla firefox. I was unable to resolve this bug on time but will address in a future release.

Deployment
Version Control
The site was created using the Visual Studio code editor and pushed to github to the remote repository ‘Cobh-Childrens-Theatre’.

The following git commands were used throughout development to push code to the remote repo:

git add <file> - This command was used to add the file(s) to the staging area before they are committed.

git commit -m “commit message” - This command was used to commit changes to the local repository queue ready for the final step.

git push - This command was used to push all committed code to the remote repository on github.

Deployment to Github Pages
The site was deployed to GitHub pages. The steps to deploy are as follows:
In the GitHub repository, navigate to the Settings tab
From the menu on left select 'Pages'
From the source section drop-down menu, select the Branch: main
Click 'Save'
A live link will be displayed in a green banner when published successfully.
The live link can be found here - /

Clone the Repository Code Locally
Navigate to the GitHub Repository you want to clone to use locally:

Click on the code drop down button
Click on HTTPS
Copy the repository link to the clipboard
Open your IDE of choice (git must be installed for the next steps)
Type git clone copied-git-url into the IDE terminal
The project will now of been cloned on your local machine for use.

Credits
Accordion without javascript
Code was used from this site to create the accordian effect on the adventures page sections for the hidden sections for each days travels. Styles were changed to suit styling on my Website.
Youtube Gallery Filter Tutorial
Gallery page was created with inspiration from this video. I adapted code to use flexbox rather than css grid to make the page responsive on every device.
Content
All content with
Media
Website Logo was 

Maps on the ..


[def]: docs/readme_images/readme_images.png