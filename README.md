# <p align="center"> Hi there 👋 I'm Mohammad Hossein 👨‍💻 </p>
<p align="center"> React Js expert and FrontEnd Developer from Iran.</p>

## Description Library
> Before you start the description if you want to install this package from the npmjs website, visit this [Link](https://www.npmjs.com/package/react-pagination-smooth)
>
> Of course, you can add the same Pagination folder in your project and use only one line of import and use
>
> Library ■ A very useful and efficient pagination library for React-Spa websites that shows data without refreshing the page
>
> It is very compact and optimized and has only `2 dependencies`, both react and react-dom.
>
> The way the package works is that first you enter all the data you need and the number of data you want on each page and leave the rest of the work to the package ☻
>
> High personalization capabilities such as color, background, visibility or lack of auxiliary arrows, etc.

## View of the Library

<img src="./public/Images/modes.png" width="500">

## Usage
- Import the pagination component first.

```javascript
import Pagination from 'Pagination';
```
- Then enter these essential items to launch pagination
```javascript
 <Pagination
    arrDatas={arrDatas}
    countDataPerPage={1}
    pathName={'/all-courses/page/'}
    onFilterDatas={handleFilterArrDatas}
/>
```
- An example in the project.
```javascript
import React, { useState, useEffect } from 'react'
import Pagination from 'Pagination';

export default function Test() {

    const [allDatas, setAllDatas] = useState([])
    const [filterDataPage, setFilterDataPage] = useState([])

    useEffect(() => {
        fetch(`http://localhost:3000/v1/datas`)
            .then(res => res.json())
            .then(datas => setAllCourses(datas))
    }, [])

    const handleFilterCourses = datas => setFilterCoursesPage(datas)

    return (
        <section>
            <div>
                {
                    filterDataPage.map((datas, index) => (
                        <Course key={index} {...datas} />
                    ))
                }
            </div>

            <div>
                <Pagination
                    arrDatas={arrDatas}
                    countDataPerPage={6}
                    pathName={'/all-datas/page/'}
                    onFilterDatas={handleFilterArrDatas}
                />
            </div>
        </section>
    )
}
```

___
>### Social Network
> [<img src="./public/Images/github.png" width="30">](https://github.com/khadem-mh)
> [<img src="./public/Images/linkedin.png" width="30">](https://www.linkedin.com/in/khadem-mh/)
> [<img src="./public/Images/telegram.png" width="30">](https://t.me/mhkhadem)
> [<img src="./public/Images/whatsapp.png" width="30">](https://wa.me/989031335939)
> [<img src="./public/Images/wakatimesvg.png" width="130">](https://wakatime.com/@khadem_mh)