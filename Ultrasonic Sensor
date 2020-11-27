import smbus
import time

bus = smbus.SMBus(1)
address = 8 # I2C address for Ultrasonic bus

def distance():
    """Returns distance measured by ultrasonics in cm"""
    return bus.read_byte_data(address, 0)

while True:
    print(distance(), " cm")
    time.sleep(1.0)
