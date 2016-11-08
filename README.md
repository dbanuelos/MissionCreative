# MissionCreative
play """
  F ^G C' F'
  [=G'E] C' ^G
  =G' [^G'^D] C'
  ^G ^G' [=D'D]
  A^ F D'
  [C^=C'] ^G F
  ^G21/3 C' ^G F
  [=G^DG,][F,F^G]
  [=^gff,]2
"""

speed 10
a = new Turtle orchid
b = new Turtle lightblue
c = new Turtle pink
for [1..20]
 (random [a,b,c]).fd 20
 (random [a,b,c]).rt 88

sync a, b, c
a.dot orchid, 125
b.dot lightblue, 125
c.dot pink, 125

w= new Webcam
w.rt 360
w.fd 100

w = new Webcam
button 'stop', ->
  do w.cut

s = new Sprite
  color: lightgrey
  height: 130
  width: 130
s.pen lightgrey
s.rt 180
s.fd 100

