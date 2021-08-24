- <html>
<head>
    <title>Music Website - MJC </title>
    <link rel="stylesheet" href="style.css"
</head>  
<body>
    <div class="container">
         <div class="navbar"></div>
         <img src="media/logo.png" class="Logo">
         <text font-face="MJC" size="7"></text>
        </div>
        <div class="content">
           <div class="left-col">
               <h1>THE<br>REAL<br>SOUND</h1>
           </div>
           <div class="right-col">
               <p>Click Here To Listen</p>
               <img src="media/play.png" id="icon">        
            </div>
    </div>

    <audio id="mySong">
        <source src="media/riseup.mp3.mp3" type="audio/mp3">
    </audio>

<script>
        
    var mySong = document.getElementById("mySong");
    var icon = document.getElementById("icon");

    icon.onclick = function(){
        if(mySong.paused){
            mySong.play();
            icon.src = "media/pause.png"
        }else{
            mySong.pause();
            icon.src = "media/play.png"
        }

    }    
    
</script>

</body>  
</html>
