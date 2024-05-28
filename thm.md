Your first hack

Click the "Start Machine" button. Once loaded in Split View in your browser, you will have access to a machine you'll use to hack a fake bank application called FakeBank. If you don't see the machine appear, use the blue Show Split View button on the top-left of this page.

Start Machine
We will use a command-line application called "GoBuster" to brute-force FakeBank's website to find hidden directories and pages. GoBuster will take a list of potential page or directory names and tries accessing a website with each of them; if the page exists, it tells you.

Step 1) Open a terminal

A terminal, also known as the command-line, allows us to interact with a computer without using a graphical user interface. On the machine, open the terminal using the Terminal icon:  

Stuck? See video


Step 2) Find hidden website pages

Most companies will have an admin portal page, giving their staff access to basic admin controls for day-to-day operations. For a bank, an employee might need to transfer money to and from client accounts. Often these pages are not made private, allowing attackers to find hidden pages that show, or give access to, admin controls or sensitive data.

Type the following command into the terminal to find potentially hidden pages on FakeBank's website using GoBuster (a command-line security application).

`` gobuster -u http://fakebank.com -w wordlist.txt dir ``
The command will run and show you an output similar to this:
