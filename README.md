# Horiseon SEO

## Technology Used 

| Technology Used         | Resource URL           | 
| ------------- |:-------------:| 
| HTML    | [https://developer.mozilla.org/en-US/docs/Web/HTML](https://developer.mozilla.org/en-US/docs/Web/HTML) | 
| CSS     | [https://developer.mozilla.org/en-US/docs/Web/CSS](https://developer.mozilla.org/en-US/docs/Web/CSS)      |   
| Git | [https://git-scm.com/](https://git-scm.com/)     |    

## Description 

[Visit the Deployed Site](https://rossfahan.github.io/Horiseon-v2/)

Horiseon is an SEO and digital marketing service aimed at providing services to improve buisnesses online presence, visibility, reputation, and customer acquisition using various strategies and techniques.

In this refactoring project, I took steps to make changesspecifically improve accessibility, search engine optimization of the Horiseon website itself, improved code readability and maintainability using comments and semnatic HTML, and insured code followed a logical structure. These changes a better user experience for all visitors and improves its visibility in search engine rankings, and also makes the code easier to maintain in the future.


## Landing Page
![Site Langing Page](./assets/images/landing-page.png)


## Code Refactor Examples


```html
<div class="header">
        <h1>Hori<span class="seo">seo</span>n</h1>
        <div>
            <ul>
                <li>
                    <a href="#search-engine-optimization">Search Engine Optimization</a>
                </li>
                <li>
                    <a href="#online-reputation-management">Online Reputation Management</a>
                </li>
                <li>
                    <a href="#social-media-marketing">Social Media Marketing</a>
                </li>
            </ul>
        </div>
    </div>
```

Converting the above non-semantic div with the class of 'header' to an appropriate [<header> semantic element](https://www.w3schools.com/html/html5_semantic_elements.asp). 

```html
<header>
        <h1>Hori<span class="seo">seo</span>n</h1>
        <nav>
            <ul>
                <li>
                    <a href="#search-engine-optimization">Search Engine Optimization</a>
                </li>
                <li>
                    <a href="#online-reputation-management">Online Reputation Management</a>
                </li>
                <li>
                    <a href="#social-media-marketing">Social Media Marketing</a>
                </li>
            </ul>
        </nav>
    </header>

```

This change require some additional modification to the CSS selector: 

```css
.header {
    padding: 20px;
    font-family: 'Trebuchet MS', 'Lucida Sans Unicode', 'Lucida Grande', 'Lucida Sans', Arial, sans-serif;
    background-color: #2a607c;
    color: #ffffff;
}
```

No longer targeting the element on the page with the class of 'header' but instead the css selector targeting the 'header' element 

```css
header {
    padding: 20px;
    font-family: 'Trebuchet MS', 'Lucida Sans Unicode', 'Lucida Grande', 'Lucida Sans', Arial, sans-serif;
    background-color: #2a607c;
    color: #ffffff;
}

```

## Learning Points 


Through this project, I learned about accessibility standards, best practices for Search Engine Optimization, make to make code more readabile and maintainable, and general best practices in web development. This was also a good lesson in being thorough giving attention to detail, as it is very easy to overlook small details. Furthermore, this was a good lesson in quality assurance as I had to make sure the project met all the given acceptance criteria.

I also learned the importance of version control, deploying a website, and making frequent meaningful commits to your repository with descriptive messages.


## Author Info

```md
### Links

* [LinkedIn](https://www.linkedin.com/in/rossfahan)
* [Github](https://github.com/RossFahan)
```


## Credits

Referenced the following:
* [W3schools](https://www.w3schools.com/)
* [Mozilla Developer Network (MDN)](https://developer.mozilla.org/)

## License

MIT License

Copyright (c) [2023] [Ross Fahan]

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.


© 2023 edX Boot Camps LLC. Confidential and Proprietary. All Rights Reserved.