## Clock UI By NorthFox Developers

##### 📫 Connect with me here:<br />
 <br />
 <p>
  <a href="https://www.instagram.com/princu.09">
    <img src="https://img.shields.io/badge/princu.09-386938188?style=flat&logo=instagram&color=black">
  </a> &nbsp; 
  <a href="https://twitter.com/princu09">
    <img src="https://img.shields.io/badge/@princu09-30302f?style=flat&logo=twitter&color=black">
  </a>&nbsp; 
  <a href="https://github.com/princu09">
    <img src="https://img.shields.io/badge/@princu09-30302f?style=flat&logo=github&color=black">
  </a>&nbsp;
    <a href="https://www.t.me/proghub09">
    <img src="https://img.shields.io/badge/ProgHub09-386938188?style=flat&logo=telegram&color=black">
  </a>
</p>

[![Clock UI](https://github.com/princu09/Digital-Clock/blob/master/Screen%20Rec.gif?raw=true)](https://github.com/princu09/Digital-Clock)


### Clock UI Code Direct :


- ##### Html File : index.html
```
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="style.css">
    <title>Digital Clock</title>
</head>

<body>
    <div id="clock">
        <h2>The Time is</h2>
        <div id="time">
            <div><span id="hour">00</span><span>Hours</span></div>
            <div><span id="minutes">00</span><span>Minutes</span></div>
            <div><span id="seconds">00</span><span>Seconds</span></div>
        </div>
    </div>

    <script>
        function clock() {
            var hours = document.getElementById('hour');
            var minutes = document.getElementById('minutes');
            var seconds = document.getElementById('seconds');


            var h = new Date().getHours();
            var m = new Date().getMinutes();
            var s = new Date().getSeconds();

            hours.innerHTML = h;
            minutes.innerHTML = m;
            seconds.innerHTML = s;
        }

        var interval = setInterval(clock, 1000);
    </script>
</body>

</html>
```



- ##### CSS File : style.html
```
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Open Sans', sans-serif;
}

body {
    display: flex;
    justify-content: center;
    align-items: center;
    min-height: 100vh;
    background: #060a1f;
}

#clock h2 {
    position: relative;
    display: block;
    color: #fff;
    text-align: center;
    margin: 10px 0;
    font-weight: 700;
    text-transform: uppercase;
    letter-spacing: 0.4em;
    font-size: 2em;
}

#clock #time {
    display: flex;
}

#clock #time div {
    position: relative;
    margin: 0 10px;
    -webkit-box-reflect: below 1px linear-gradient( transparent, #0004);
}

#clock #time div span {
    position: relative;
    display: block;
    height: 150px;
    width: 170px;
    background: #2196f3;
    color: #fff;
    font-weight: 300;
    display: flex;
    justify-content: center;
    align-items: center;
    font-size: 5em;
    z-index: 10;
    box-shadow: 0 0 0 1px rgba(0, 0, 0, .2);
}

#clock #time div span:nth-child(2) {
    height: 50px;
    font-size: 1em;
    font-weight: 700;
    letter-spacing: 0.2em;
    z-index: 9;
    box-shadow: none;
    background-color: #127fd6;
    text-transform: uppercase;
}

#clock #time div:last-child span {
    background: #ff006a;
}

#clock #time div:last-child span:nth-child(2) {
    background: #ec0062;
}
```
