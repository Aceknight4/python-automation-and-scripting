###### The following Python script collects system information (like OS, CPU, RAM, IP address, etc.) and saves it to a text file named system_report.txt.



#### Importing Required modules

import platform  (It access OS and hardware)
import os (interface with the OS)
import socket (helps get network related information)
import psutil (system and process utilities)


### Functions to get the operations
def get_system_info():
    info = (
        f"🔹 SYSTEM INFORMATION 🔹\n"
        f"📌 OS: {platform.system()} {platform.release()} ({platform.version()})\n"
        f"📌 Architecture: {platform.architecture()[0]}\n"
        f"📌 Machine: {platform.machine()}\n"
        f"📌 Hostname: {socket.gethostname()}\n"
        f"📌 IP Address: {socket.gethostbyname(socket.gethostname())}\n"
        f"📌 CPU: {platform.processor()}\n"
        f"📌 RAM: {round(psutil.virtual_memory().total / (1024 ** 3), 2)} GB\n"
    )
    return info


### Function to get the current logged in user
def get_active_users():
    users = os.popen("who").read().strip()
    return f"\n👤 Active Users:\n{users if users else 'No active users found.'}"


### Function to get the current processes running
def get_running_processes():
    processes = "\n".join(f"PID: {proc.info['pid']} - {proc.info['name']}" for proc in psutil.process_iter(['pid', 'name']))
    return f"\n⚡ Running Processes:\n{processes}"


### Function to save all the information on system_report.txt file
def save_report():
    report = f"{get_system_info()}\n{get_active_users()}\n{get_running_processes()}"
    with open("system_report.txt", "w") as file:
        file.write(report)
    print("\n📂 System report saved as 'system_report.txt'.")



### Code to run all the function
if __name__ == "__main__":
    print(get_system_info())
    print(get_active_users())
    print(get_running_processes())
    save_report()
