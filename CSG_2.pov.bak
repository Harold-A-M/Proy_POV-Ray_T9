#include "colors.inc"
//establecemos un fondo de color gris
background {
    color Gray
}
//posicionamos la camara
camera{
    location<0,3,-5>
    look_at<0,1,0>
}
//representamos la lampara por medio del spotlight
//le decimos que tiene un radio de 5 y el falloff nos ayuda 
// a representar la iluminación de la lámpara en el piso
// de igual manera le decimos que la luz apunta hacia el point_at
light_source{
    <0,10,0>
    color White
    spotlight
    radius 5
    falloff 15
    point_at <0, 0, 0>
}

merge{
    sphere{
       <0, 1, 0>, 1
       texture{
            pigment{color Yellow transmit .8}
            finish{phong .1}}
            interior{ior 1}                                                            
       }
   }
   union{
    sphere { <0, 0, 0>, 1
        translate -0.5*x
        pigment{Green}
    }
    sphere { <0, 0, 0>, 1
        translate 0.5*x
        pigment{Grey}
    }
    translate 1*y
    }

plane{
    <0,1,0>0
    pigment{
        color Gray
    }
}