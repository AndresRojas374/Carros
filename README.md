x = 500
y = 300

def setup():
    size(x, y)
    
class Carro1:
    def __init__ (self):
        self.c = color(255)
        self.posX1 = 100
        self.posY1 = 100 
        self.velx1 = 1
miCarro1 = Carro1()

def draw():
    background(200)
    fill(255, 0, 50,30)
    noStroke()
    rect (miCarro1.posX1, miCarro1.posY1, 30, 30)
    miCarro1.posX1 = miCarro1.posX1 + miCarro1.velx1
    if miCarro1.posX1 > 500:
        miCarro1.posX1 = 0
