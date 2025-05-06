import RPi.GPIO as GPIO
import time

LED_PIN = 17  # You can change this to any GPIO pin you’re using

# Setup
GPIO.setmode(GPIO.BCM)
GPIO.setup(LED_PIN, GPIO.OUT)

try:
    while True:
        GPIO.output(LED_PIN, GPIO.HIGH)  # Turn on LED
        time.sleep(1)                    # Wait 1 second
        GPIO.output(LED_PIN, GPIO.LOW)   # Turn off LED
        time.sleep(1)                    # Wait remaining 1 second (total cycle = 2 sec)

except KeyboardInterrupt:
    print("Program stopped manually")

finally:
    GPIO.cleanup()
