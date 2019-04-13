# Homework #2

## STEP 1

_Note: The commands below presume you're using Linux/Mac.  For Windows, please_  
_look for an equivalent (or reach out for help)._

1.  Create a new ssh key pair using the following command:  
    ```ssh-keygen -t rsa -b 4096 -m pem -C "your@email.com"```  
    _(When prompted, you should probably use a filename and path separate from your main id_rsa key)_

2.  Add a pem version of your public key using the following command:  
    ```ssh-keygen -f your_key.pub -e -m pem > your_key.pub.pem```

3.  Send the `your_key.pub.pem` file to Ben:
    - Email Ben at `bjblock@gmail.com`
    - Slack Ben at `@Ben Block`

## STEP 2

Within 48 hours of sending your public key to Ben, he will send back an encrypted file `PROJECT.md`.

To discover your project assignment, decrypt the PROJECT.md file with your private key.
This will include instructions of which homework assignment has been assigned to you.

The coding requirements and grading rubric can be found in [requirements.md](requirements.md).

A starting point for Python 3 applications is included as `sample_project.py`.

When you're ready to turn in your code, update this file
with instructions on how we can install and run your project,
as well as any simplifying assumptions and decisions you
made along the way.
