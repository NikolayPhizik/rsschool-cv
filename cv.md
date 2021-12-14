
![Фото для профиля](img/ProfilePhoto.jpg "Фото для профиля")

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

Currently I work as an auto electrician diagnostician. I love to learn new things. While working as an auto electrician-diagnostician, he acquired the skill of analytical thinking, the skill of collecting data necessary for diagnostics and troubleshooting when communicating with a client, and the skill of working in a team.

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