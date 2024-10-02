js
function updateclock(){
    const now= new Date();
    let hours=now.getHours();
    const meridiem=hours >= 12?"AM":"PM";
    hours=hours%12||12;
    hours=hours.toString().padStart(2,0);
    const minutes=now.getMinutes().toString().padStart(2,0);
    const seconds=now.getSeconds().toString().padStart(2,0);
    const timeString=`${hours}:${minutes}:${seconds} ${meridiem} `;
    document.getElementById("Clock").textContent=timeString;
}

updateclock();
setInterval(updateclock,1000);
csss
body{
    background-image:url(shoes.jpg) ;
    background-position: center;
    background-repeat:no-repeat ;
    background-size: cover;
    background-attachment: fixed;
    margin: 0;
}
#clock-container{
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
}
#Clock{

    font-family: monospace;
    font-size: 6.5rem;
    font-weight: bold;


    text-align: center;
    color:rgb(0, 0, 0);
    backdrop-filter:blur(5px);
    background-color: hsla(0, o%, 100%, 0.1);
    width: 100%;
}
html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>digitalclock</title>
    <link rel="stylesheet" href="style..css")
    
</head>
<body>
    <div id="clock-container">
        <div id="Clock">00:00:00</div>
    </div>
    
         <script src="deep.js"></script>

</body>
</html>
