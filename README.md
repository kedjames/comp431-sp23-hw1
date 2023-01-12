# COMP 431 - Spring 2023 - Homework 1 
## Baby-steps Towards the Construction of a Mail Server — Parsing in Python
The goal for the first half of the course is to build a simple mail server and mail reader that will work with standard Internet mail servers using SMTP (Simple Mail Transfer Protocol) and POP (Post Office Protocol), and mail readers such as Gmail, Apple Mail, and certain versions of Thunderbird or Microsoft Outlook. This assignment is the first (very!) small piece of the mail server: a simple string parser that we will build upon in later assignments. 
**For a detailed description of the assignment, please see the assignment documentation.**

**This repo contains the following files:**
1. A python file named ``parse.py`` with basic starter code.
2. A valid test input file called ``valid_test_input_1.py``.
3. An invalid test input file called ``invalid_test_input_1.py``.

Once you have completed coding your parser, you can test it with both the valid and invalid input files provided in this repo. To test the program with the valid file, execute the command ``python3 valid_test_input_1.py > valid_file``. Next, execute the command ``python3 parse.py < valid_file``. Your program must output the following lines:


``MAIL FROM:<jeffay@cs.unc.edu>`` <br /> ``Sender ok``

Repeat the above steps with the invalid file, and your output must match the following:

``MAIL FROM: <jeffay @cs.unc.edu>`` <br /> ``ERROR -- mailbox``



