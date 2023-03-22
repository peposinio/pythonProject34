# pythonProject34


import socket
x = 0
while x <= 101:  #  import socket
    s = socket.socket()
    s.settimeout(1)
    try:
        s.connect(("172.30.230.69", x))
        print(f"{x} port is opened")
        x += 1
    except:
        print(f"The port {x} is closed")

    finally:
        s.close()
