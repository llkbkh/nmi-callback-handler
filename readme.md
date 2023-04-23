# NMI Callback Handler

This is a simple project (WIP) with the goal of exploring how NMIs can be used to stackwalk the interrupted threads to determine if the thread is or has been executing memory from unsigned regions (i.e manually mapped drivers)

![image](image.png)

Example above shows a kernal driver that reads/writes directly to physical memory of a game, mapped with the default kdmapper, being found via the stackwalk.