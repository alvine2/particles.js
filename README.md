particles.js
A lightweight JavaScript library for creating particles.

Usage
Load particles.js and configure the particles:

index.html ####
<div id="particles-js"></div>

<script src="particles.js"></script>

app.js #####
/* particlesJS.load(@dom-id, @path-json, @callback (optional)); */
particlesJS.load('particles-js', 'assets/particles.json', function() {
  console.log('callback - particles.js config loaded');
});

particles.json #######
{
  "particles": {
    "number": {
      "value": 80,
      "density": {
        "enable": true,
        "value_area": 800
      }
    },
    "color": {
      "value": "#ffffff"
    },
    "shape": {
      "type": "circle",
      "stroke": {
        "width": 0,
        "color": "#000000"
      },
      "polygon": {
        "nb_sides": 5
      },
      "image": {
        "src": "img/github.svg",
        "width": 100,
        "height": 100
      }
    },
    "opacity": {
      "value": 0.5,
      "random": false,
      "anim": {
        "enable": false,
        "speed": 1,
        "opacity_min": 0.1,
        "sync": false
      }
    },
    "size": {
      "value": 10,
      "random": true,
      "anim": {
        "enable": false,
        "speed": 80,
        "size_min": 0.1,
        "sync": false
      }
    },
    "line_linked": {
      "enable": true,
      "distance": 300,
      "color": "#ffffff",
      "opacity": 0.4,
      "width": 2
    },
    "move": {
      "enable": true,
      "speed": 12,
      "direction": "none",
      "random": false,
      "straight": false,
      "out_mode": "out",
      "bounce": false,
      "attract": {
        "enable": false,
        "rotateX": 600,
        "rotateY": 1200
      }
    }
  },
  "interactivity": {
    "detect_on": "canvas",
    "events": {
      "onhover": {
        "enable": false,
        "mode": "repulse"
      },
      "onclick": {
        "enable": true,
        "mode": "push"
      },
      "resize": true
    },
    "modes": {
      "grab": {
        "distance": 800,
        "line_linked": {
          "opacity": 1
        }
      },
      "bubble": {
        "distance": 800,
        "size": 80,
        "duration": 2,
        "opacity": 0.8,
        "speed": 3
      },
      "repulse": {
        "distance": 400,
        "duration": 0.4
      },
      "push": {
        "particles_nb": 4
      },
      "remove": {
        "particles_nb": 2
      }
    }
  },
  "retina_detect": true
}


Options
key	option type / notes	example
particles.number.value	number	40
particles.number.density.enable	boolean	true / false
particles.number.density.value_area	number	800
particles.color.value	HEX (string) <br /> RGB (object) <br /> HSL (object) <br /> array selection (HEX) <br /> random (string)	"#b61924" <br /> {r:182, g:25, b:36} <br /> {h:356, s:76, l:41} <br /> ["#b61924", "#333333", "999999"] <br /> "random"
particles.shape.type	string <br /> array selection	"circle" <br /> "edge" <br /> "triangle" <br /> "polygon" <br /> "star" <br /> "image" <br /> ["circle", "triangle", "image"]
particles.shape.stroke.width	number	2
particles.shape.stroke.color	HEX (string)	"#222222"
particles.shape.polygon.nb_slides	number	5
particles.shape.image.src	path link <br /> svg / png / gif / jpg	"assets/
particles.shape.image.width	number <br />(for aspect ratio)	100
particles.shape.image.height	number <br />(for aspect ratio)	100
particles.opacity.value	number (0 to 1)	0.75
particles.opacity.random	boolean	true / false
particles.opacity.anim.enable	boolean	true / false
particles.opacity.anim.speed	number	3
particles.opacity.anim.opacity_min	number (0 to 1)	0.25
particles.opacity.anim.sync	boolean	true / false
particles.size.value	number	20
particles.size.random	boolean	true / false
particles.size.anim.enable	boolean	true / false
particles.size.anim.speed	number	3
particles.size.anim.size_min	number	0.25
particles.size.anim.sync	boolean	true / false
particles.line_linked.enable	boolean	true / false
particles.line_linked.distance	number	150
particles.line_linked.color	HEX (string)	#ffffff
particles.line_linked.opacity	number (0 to 1)	0.5
particles.line_linked.width	number	1.5
particles.move.enable	boolean	true / false
particles.move.speed	number	4
particles.move.direction	string	"none" <br /> "top" <br /> "top-right" <br /> "right" <br /> "bottom-right" <br /> "bottom" <br /> "bottom-left" <br /> "left" <br />



