
![Profile photo](img/ProfilePhoto.jpg "Profile photo")

# Nikolay Yeremin
### Junior Frontend Developer

&nbsp;
## 📞 Contact info

Phone number | +77051072781
-------------|--------------
Email | nikolay.eremin82@mail.ru
Discord | Nikolay#2026
GitHub | NikolayPhizik
Skype | nikolay.phizik
LinkedIn | [linkedin](https://www.linkedin.com/in/nikolayphizik)

&nbsp;
## 📝 About me

My goal is to start a career as a junior front-end developer and develop to a full understanding of building the architecture of complex projects.

Currently I work as an auto electrician diagnostician. While working as an auto electrician-diagnostician, he acquired the skill of analytical thinking, the skill of collecting data necessary for diagnostics and troubleshooting when communicating with a client, and the skill of working in a team.


&nbsp;
## 🧩 Skills

* HTML + CSS
* JavaScript
* React 
* Redux
* Git

&nbsp;
## 💾 Code examples

React component for displaying pagination on the page

```
const Paginator = ({pageSize, totalUsersCount, requestTotalUsersCount, onPageChanged}) => {

    const [portionNumber, setpPortionNumber] = useState(1);
    const [currentPage, setCurrentPage] = useState(1);

    let pagesCount = Math.ceil(totalUsersCount / pageSize);
    let pages = [];
    for (let i = 1; i <= pagesCount; i++) {
        pages.push(i);
    }

    let portionSize = 3;
    let portionCount = Math.ceil(pagesCount / portionSize);
    let leftPortionPageNumber = (portionNumber - 1) * portionSize + 1;
    let rightPortionPageNumber = portionNumber * portionSize;

    requestTotalUsersCount();
    return (
        <div className={classes.paginator_box}>
            <div className={classes.button_back}>
                {portionNumber > 1 && <button className={classes.button} 
                onClick={() => {setpPortionNumber(portionNumber - 1)}}>Back</button>}
            </div>
            <div className={classes.container}>
                {pages.filter(p => p >= leftPortionPageNumber && p <= rightPortionPageNumber).map(p => {
                    return <div className={classNames(
                        {[classes.selectedPage]: currentPage === p}, 
                        classes.span)} key={p} onClick={(e) => {
                        onPageChanged(p);
                        setCurrentPage(p);
                    }}>{p}</div>
                })}
            </div>
            <div className={classes.button_next}>
                {portionCount > portionNumber && <button className={classes.button} 
                onClick={() => {setpPortionNumber(portionNumber + 1)}}>Next</button>}
            </div>
        </div>
    );
};

export default Paginator;
```
link to all [code](https://github.com/NikolayPhizik/Test1.git)

&nbsp;
## 👨‍💻 Experience
I created my own social network while studying the course react the way of the samurai. During the development process, I gained skills in working with such libraries as React, Redux, React-Redux, creating asynchronous requests to the server using the axios library, using Redux-form, Redux-thunk. Gained the understanding and skill of creating a three-layer architecture of applications: UI, BLL, DAL. Link to the source code of this project
* [Link to the source code of this project](https://github.com/NikolayPhizik/SocialNetworkCode.git)

While learning JavaScript, I created an oscillating circuit calculator and a text encoder. Both programs are my authorship. While studying JavaScript, I learned how to solve all sorts of algorithmic problems and work with the Git version control system.
The results of the work can be viewed on Github Pages:
* [Calculator link](https://nikolayphizik.github.io/Calculator/)
* [calculator source code](https://github.com/NikolayPhizik/Calculator)
* [Link to the encryptor](https://nikolayphizik.github.io/Shifrator/)
* [encoder source code](https://github.com/NikolayPhizik/Shifrator)

While studying on the HTML Academy platform, I studied semantic layout, as well as got acquainted with the concept of accessibility, and during the training I made up the site.
* [Link to Github Pages](https://nikolayphizik.github.io/Barbershop/)
* [Link to source code](https://github.com/NikolayPhizik/Barbershop)

&nbsp;
## 🎓 Education

### Online learning

July - November 2021 | [Course react the way of the samurai](https://www.youtube.com/playlist?list=PLcvhF2Wqh7DNVy1OCUpG3i5lyxyBWhGZ8)
----------------------|-----------------------------------------
April - July 2021 | [JavaScript](https://learn.javascript.ru/) and the book "Expressive JavaScript" by Marein Haverbeke.
February - April 2021 | [HTML Academy](https://htmlacademy.ru)

&nbsp;
## 📚 English
* My English level is now - A1. I am currently studying on my own.
