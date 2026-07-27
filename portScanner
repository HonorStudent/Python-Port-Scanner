#Joshua Thomas
#This program was originally written for the class Python Programming for Security Analysis and Penetration Testing in Spring 2022.

#This program scans all the ports on a entered IP address.

#Updated 7-26-26


import socket
import sys


def main():
    print("Hello, I am a port scanner. Use me wisely.")
    print("<---------------------------------------->")

    entered_ip = input("What IP do you want me to scan? ")
    print("Please wait while I scan", entered_ip)

    try:
        socket.setdefaulttimeout(1)

        for port in range(1, 65536):
            with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as sock:
                response = sock.connect_ex((entered_ip, port))

                if response == 0:
                    print(f"Port {port} is open")

    except KeyboardInterrupt:
        print("\nGoodbye for now.")
        sys.exit()

    except socket.gaierror:
        print("Sorry, I had a problem connecting to your host.")
        sys.exit()

    except socket.error:
        print("Sorry, I can't connect to your server.")
        sys.exit()

    print("Scan complete.")


if __name__ == "__main__":
    main()
