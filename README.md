<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Hellow I am Janeesha Kavishan 👋</title>
</head>
<style>
    @property --d{
  syntax: '<angle>';
  inherits: true;
  initial-value: 0deg;
}
button {
  width: 200px;
  aspect-ratio:1;
  font-size:30px;
  color: #fff;
  background: none;
  border: none;
  border-radius: 20px; 
  position: relative;
  z-index: 0;
  transition: .3s;
  cursor: pointer;
}
button:before {
  content: "";
  position: absolute;
  inset: -8px;
  padding: 8px;
  border-radius: 28px; 
  background: conic-gradient(from var(--d,0deg),
  #21D4FD ,
        #0000 30deg 120deg,
        #B721FF 150deg 180deg,
        #0000 210deg 300deg,
        #21D4FD 330deg
    );
    -webkit-mask:
        linear-gradient(#000 0 0) content-box,
        linear-gradient(#000 0 0);
    -webkit-mask-composite: xor;
            mask-composite: intersect
    }
    button:after {
    content: "";
    position: absolute;
    inset: -100px;
    background:
        radial-gradient(80px at left  150px top    120px,#21D4FD 98%,#0000),
        radial-gradient(80px at right 150px bottom 120px,#B721FF 98%,#0000);
    filter: blur(60px);
    opacity: .5;
    }

    button:before,
    button:after {
    transition:.5s, 99999s 99999s transform, 99999s 99999s --d;
    }
    button:hover {
    box-shadow: 0 0 0 1px #666;
    }


    button:hover:after {
    transform: rotate(3600deg);
    transition: .5s,60s linear transform;
    }
    button:hover:before {
    --d: 3600deg;
    transition: .5s,60s linear --d;
    }
    button:hover:before {
    background-color: #222;
    }

    body {
    margin: 0;
    min-height: 100vh;
    display: grid;
    place-content: center;
    grid-auto-flow: column;
    background-color: #1b1b1c;
    }
</style>
<body>
    <button><font-size=3> Hellow I am Janeesha Kavishan 👋</font-size></button>
</body>
</html>
