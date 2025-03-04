# Ghost
its a ghostly mouse

It hovers around and randomly presses tab and space every one out of four loops

import pyautogui
import time
import random

print("Starting in 5 seconds... Move your cursor where you want it to begin!")
time.sleep(5)

screen_width, screen_height = pyautogui.size()
print(f"Screen size: {screen_width}x{screen_height}")

while True:
    pyautogui.moveTo( random.randint(196,723), random.randint(276, 654), duration=1)
    time.sleep(random.randint(4, 27))  # Pause before next loop
    cointoss = random.randint(1, 100)
    print(cointoss)
    if cointoss > 75:
        pyautogui.press('Tab')
        pyautogui.press('space')
