# website-template
A template for a personal website
theme
    style.csv contains all the themeing of your website except for photo.html
    you can change the page backgrounf with the background-colour atribute under main
    you can change the colour of the navbar in the topnav background-image property and the background-colour property. for the selected item it is under .topnav a:hover and background-colour
    the pages background image you under html, body find background image whate you swap resource/background.jpg for the location of your background image but for this make sure to use the whole url

home page
    (index.html)
    you can change the picture, add, remove, or change any text you like, insert iframes, and change and add pictures but this pre configured page i personally find enjoyable

blog
    (blog.html, blog folder, RSS.xml, and resource/blog directory)
    this has no background colour just the image
    to add more entries to the list copy line 13, change the link and change the name to the title
    to create a new entry copy ex1.html in the blog folder, rename it to a summarised article, and change all the fields and write all the rest of the text with standard html code
    to setup an rss feed you must create an item, add a title, link the website, add a guid (identifier so if you are lazy your entry url), add the date it was published, and discribe the entry

topnav
    (topnav.html)
    this is a file that is on evrey page that links to all the main pages you would want to acess.
    if you want to add items add an a tag with the link and the title
    you can also un-comment the photo link to show the photos page

photos
    (photo.html, photo-RSS.xml)
    the photo page is whare you go if you feel as if you want to only publish a photo
    this page starts with an image caurocell you can add as many images as you wish to by coppying the pre existing image elements and paste them
    the first image in the caurocell (from the top) is displayed first
    if you wish do dump a bunch of images you can add these to resource/photos, and display them together seperated by a title or date and caption by using an img tag wit a h2 tag above and a p tag below.
    to create an rss feed use the photo-RSS.xml to add a title or date in the title tag, a link to the photo page in the link tag, an identifier in the guid tag, the date it was published in the pubdate tag, the images under the image tag with a url tag, and a caption in the discription

contact
    (contact.html, friends.html, friends.csv)
    on the contact page it has a little about you, your email, a list of friends and links to thier websites, and links to your social media
    to change the email you change the email agresses after mailto to your ones
    for the other social sites you can change the links in the a elements under href
    to add friends do not touch the friends.html
    instead change the friends.csv adding the name in the first line, the url in the second, and the place you want them pinned if you want them pined