# Instrucciones para intercambiar símbolos de teclas.
Estas instrucciones estan enfocadas en cambiar las teclas de paréntesis por las de corchetes (o llaves, según el idioma de su teclado). Esto es con el propósito de ahorrar tiempo (es más rápido y cómodo solo presionar una tecla que presionar _shift_ más esa misma tecla) que puede ser invertido en pensar cómo resolver sus prácticas. 

## Arch
### (o cualquier distro de linux)
- Dependiendo qué _layout_ usen debe editar el archivo de configuración de la siguiente forma:
  `$ sudo vim /usr/share/X11/xkb/symbols/latam
  Si usan teclado en ingles en lugar de `latam` editan `us`, si usan los dos, editan los dos.
  Para el caso en español, deben intercambiar braceleft por parenleft y braceright por parenright.
  Para el caso en inglés, deben intercambiar bracketleft por parenleft y bracketright por parenright.
  Guardan el archivo y salen.
- El siguiente paso es reestablecer el _layout_ que acaban de modificar.
  `$ setxkbmap latam`
- Paso opcional: Si utilizan el editor de texto **supremo**, i.e. vim, también es cómodo intercambiar _caps lock_ por _escape_, lo pueden hacer pasando la opción como sigue al establecer el _layout_:
  `$ setxkbmap -option caps:swapescape latam`
- Listo.

## Windows
Pueden usar autohotkeys para hacer el cambio. Aunque no es tan efectivo pues no hace distinción entre la tecla y la tecla con shift.
La sintáxis es así:
  ```
  (::[
  [::(
  )::]
  ]::)
  ```
Esas caritas tristes y felices van a su script de autohotkeys.

## MacOS
Buena suerte. Si lo logran sin utilidades de terceros tienen 0.01 adicional en sus prácticas.
