# mario_bross_css


*{
margin: 0;
padding: 0;
box-sizing: border-box;   
}

.gamer-board {
  width: 100%;
  height: 900px;
  border-bottom: 15px solid rgb(35, 160, 35);
  margin: 0 auto;
  position: relative;
  overflow: hidden;
  background: linear-gradient(#87ceeb, #e0f6ff);

}

.pipe{
  width: 90px;
  position: absolute;
  bottom: 0;
  right: 0;
  animation: pipe-animation 10s infinite linear;
}

.mario{
  width: 150px;
  position: absolute;
  bottom: 0;
}

.jump{
  animation: jump 500ms ease-out;

}

.clouds{
  width: 550px;
  position: absolute;
  animation: clouds-animation 20s infinite linear;
}

.clouds2{
  width: 550px;
  position: absolute;
  animation: clouds2-animation 20s infinite linear;
  bottom: 50%;

}
.bulletbills{ 
  position: absolute;
  height: 100px;
  bottom:15%;
  right: 0;
  animation: bulletbills-animation 20s infinite linear;
  width: 100px;

}
.cactus{

  width: 100%;
  position: static;
  bottom: 0;
}


@keyframes pipe-animation{
  from{
    right: -90%;
}

  to{
    right: 100%;

}
}

@keyframes jump{

  0% {
    bottom: 0;

  }
  40%{

    bottom: 180px;
  }
  50%{

    bottom: 180px;
  }
  60%{

    bottom: 180px;

  }
  100%{ 

    bottom: 0;
  }
}
@keyframes clouds-animation {
  from{
    right: -550px;
  }
  to{
    right:100%;
  }
  
}


@keyframes bulletbills-animation{

  from{
    right: -50px;
  }
  to{
    right:100%;
  }

}

@keyframes clouds2-animation {
  from{
    right: -550px;
  }
  to{
    right:100%;
  }
  
}
