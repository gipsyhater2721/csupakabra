from machine import Pin
from time import sleep

# LED kimenetek
led_left = Pin(14, Pin.OUT)
led_right = Pin(18, Pin.OUT)
led_frontleft = Pin(10, Pin.OUT)
led_frontright = Pin(19, Pin.OUT)

# Gomb beállítása (pl. GPIO 15)
button = Pin(15, Pin.IN, Pin.PULL_UP)  # Pulldown ellenállás, alapértelmezés szerint magas (3.3V)

# Folyamat állapotának nyomon követése
running = True

while running:
    # Ellenőrizzük, hogy a gombot lenyomták-e (alacsony jel)
    if not button.value(0):  # Ha lenyomva van a gomb, alacsony (GND) lesz
        running = True
    
    #Villogtatjuk a LED-eket sorrendben
        led_left.toggle()
        sleep(0.5)
        led_frontleft.toggle()
        sleep(0.5)
        led_frontright.toggle()
        sleep(0.5)
        led_right.toggle()
        sleep(0.5)
    #else
        #led_left.off()
        #led_right.off()
        #led_frontleft.off()
        #led_frontright.off()

# Leállás után kikapcsolhatjuk az összes LED-et
