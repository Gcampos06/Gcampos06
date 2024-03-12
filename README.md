- 👋 Hi, I’m @Gcampos06
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...

<!---
Gcampos06/Gcampos06 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
<!--Estructura |CSS - BEGIN| completa del CSS-->

<style>
@import url('https://fonte.googleapis.com/ css?family=poppins:200,300,400,500,600,700,800,900&display=swap');
*
{
margin: 0;
padding: 0;
box-sizing: border-box;
font-family: 'Poppins',san-serif;

}
section
{
position: relative;
width: 100%;
min-height: 100vh;
padding: 100px;
display: flex;
justify-content: space-between;
align-items: center;
background: #fff;

}

header
{
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    padding: 20px 100px;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

header .logo
{
    position: relative;
    max-width: 80px;
}
 
header ul
{
    position: relative;
    display: flex;
}
header ul li
{
    list-style: none;
}
header ul li a
{
   display: inline-block;
   color: #333;
   font-weight: 400;
   margin-left: 40px;
   text-decoration: none;
}
.content
{
position: relative;
width: 100%;
display: flex;
justify-content: space-between;
align-items: center;
}
.content .textBox
{
    position: relative;
    max-width: 600px;
}
.content .textBox h2
{
   color: #333;
   font-size: 4em;
   line-height: 1.4em;
   font-weight: 500; 
}
.content .textBox h2 span
{
    color: #017143;
    font-size: 1.2em;
    font-weight: 900;
}
.content .textBox p
{
color: #333;
}
.content .textBox a
{
 display: inline-block;
 margin-top: 20px;
 padding:  8px 20px;
 background: #017143;
 border-radius: 40px;
 color: #fff;
 font-weight: 500;
 letter-spacing: 1px;
 text-decoration: none;
}

.content .imgBox
{
    width: 600px;
    display: flex;
    justify-content: flex-end;
    padding-right:50px;
    margin-top: 50px;
}
.content .imgBox img
{
    max-width: 340px;

}
.thumb
{
    position: absolute;
    left: 50%;
    bottom: 20px;
    transform: translateX(-50%);
    display: flex;
}
.thumb li
{
    list-style: none;
    display: inline-block;
    margin: 0 20px;
    cursor: pointer;
}

.thumb li:hover
{
 transform: translateY(-15px);
}
.thumb li img
{
 max-width: 60px;
}
.sci
{
    position: absolute;
    top: 50%;
    right: 30px;
    transform: translateY(-50%);
    display: flex;
    justify-content: center;
    align-items: center ;
    flex-direction: column;
}
.sci li
{
list-style: none;
}
.sci li a 
{
display: inline-block;
margin: 5px 0px;
transform: scale(0.6);
}
.circle
{
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background: #017143;
    clip-path: circle(600px at right 800px) ;
}

</style>

<!--Estructura |CSS - END| completa del CSS-->


<!DOCTYPE html> 
<html>
    <head>
     <meta charset="UTF-8">
     <!--Nombre: BEGIN- del sitio web landing-->
     <title>Starbucks Website Landing page</title>
    <!--Nombre: END- del sitio web landing-->

     <link rel="stylesheet" href="style.css">
    </head>
<body>
    <section>
        <div class="circle"></div>
        <header>
            <a href="#"><img src="logo.png" class="logo"></a>
            <ul>
                <li><a href="#"> Inicio</a></li>
                <li><a href="#"> Menú</a></li>
                <li><a href="#"> Lo más nuevo</a></li>
                <li><a href="#"> Contacto</a></li>
            </ul>
        </header>
        <div class="content">
           <div class="textBox">
             <h2> It's not just coffe <br>It's <span>Starbucks</span></h2>
             <p>
              Lorem ipsum dolor, sit amet consectetur adipisicing elit. Recusandae maxime dignissimos nemo eum optio officia eaque nam ipsa provident, similique animi ipsum, dicta, debitis repudiandae labore quibusdam distinctio molestiae perferendis.
             </p>
             <a href="#">Learn More</a>
        </div>
           <div class="imgBox">
                <img src="img1.png" class="starbucks">
           </div>   
        </div>
        <!--IMAGENES| SUB IMAGENES| COLOR DEL CIRCULO -->
        <ul class="thumb">
            <li><img src="thumb1.png" onclick="imgSlider('img1.png');cambiocolor('#017143')" ></li>
            <li><img src="thumb2.png" onclick="imgSlider('img2.png');cambiocolor('#eb7495')" ></li>
            <li><img src="thumb3.png" onclick="imgSlider('img3.png');cambiocolor('#d752b1')"></li>
        </ul>
                <!--| REDES SOCIALES | -->

        <ul class="sci">
            <li><a href="#"><img src="facebook.png"></a></li>
            <li><a href="#"><img src="twitter.png"></a></li>
            <li><a href="#"><img src="instagram.png"></a></li>

        </ul>
    </section>
    <!--Script BEGIN-- para los selectores de los productos-->
    <script type="text/javascript"> 
     function imgSlider(anything){
        document.querySelector('.starbucks').src = anything;
     }  
     function cambiocolor(color){
        const circle = document.querySelector('.circle');
        circle.style.background = color;
     }
    </script>
   <!--Script END-- para los selectores de los productos-->

</body>
</html>
