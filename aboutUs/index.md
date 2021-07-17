<!DOCTYPE html>
<html>
<head>
    <title>Pet Photos</title>
    <link rel="stylesheet" href="https://unpkg.com/mvp.css">
</head>
<body>
    <header>
        <h1>Pet Photos</h1>
        <nav class="navbar">
            <ul>
                <li><a href='/'>Home</a></li>
                <li><a href="/aboutUs">About Us</a></li>
            </ul>
        </nav>
    </header>
    <!-- added horizontal line which is why <hr> is present-->
    <hr>
    <main>
    <h1>About Us</h1>
    <p>       
        As a team, we implemented a website showcasing pet 
        photos. We extracted information about the pet photos 
        from the Unsplash dataset (Lite Version) to construct 
        our website. The information we extracted consists of 
        the metadata and captions of the pet photos. We used 
        Static Site Generator to create the HTML for the site 
        instead of managing 100 photos by hand. </p>
        
        <p>Eleventy was used
        to turn the data in the directory into a site with one 
        webpage for each photo. This meant that each photo had
        its own individual page. From each HTML file, the 
        front-matter data was used along with Eleventy templates.
        The templates were used to create enhanced pages for 
        each picture plus credit and additional information for each 
        photo. We had to validate our markup and enhance the site-wide 
        layout so the site would include the standard page elements. 
        We then added an additional feature which allows the user to go
        to the previous and next picture. </p> 
        
        <p>
        In order to create the previous, current, and next page, we 
        had to get the number part of the url. The number was converted 
        into a string number to integer. Then we only rendered the 
        pageable tab when the current page was not the first or last 
        page. If the number page is greater than zero and less than nine, 
        then 00 is added to the previous and next value before converting 
        back to a string. If the number page is 9, 00 is added to the previous 
        and next value. If the number page is 10, 00 is added to the previous 
        and next value. Lastly, if the number page is greater than 10, 0 is 
        added to front before converting back to a string. The pageable tab 
        is rendered one more time for page 0 and page 99. Page 0 doesn’t have 
        a previous and page 99 doesn’t have a next. Therefore, we reload the 
        the either page 0 or 99 if the user clicks previous/next.

        Lastly, this project could have not been completed 
        without the

        <a href="https://github.com/unsplash/datasets">Unplash dataset.</a><br></p>
       
    <ul>
        <li>Created by:
        <li>Andy Lopez </li>
        <li>Benjamin Jacobs</li> 
        <li>Bradley Vo </li>
       <li>Britney Fernandez</li> 

    </ul>

    <hr>
    <footer>
        <!-- Added Copyright symbol, credit to Bradley -->
        <p>&copy;Copyright Team 6. All rights Reserved!</p>
        <nav>
        <!-- site map at bottom of page so user has easy access to home/aboutUs  -->
        <h3>Site Map:</h3>
        <ul>
            <li><a href='/'>Home </a>
            <li><a href="/aboutUs">About Us</a>
        </ul>
        </nav>
    </footer>
</main>
</body>
</html>