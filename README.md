# Getting Started with Dafny

---

## Introduction

From Dafny Repository:

Dafny is a verification-ready programming language. As you type in your program, Dafny's verifier 
constantly looks over your shoulder, flags any errors, shows you counterexamples, and 
congratulates you when your code matches your specifications. When you're done, Dafny can compile 
your code to C#, Go, Python, Java, or JavaScript (more to come!), so it can integrate with your 
existing workflow.


---

## Installing Dafny in Windows:

    https://github.com/dafny-lang/dafny/wiki/INSTALL#windows-source



    Install (if not already present) .NET Core 6.0: https://dotnet.microsoft.com/download/dotnet/6.0
     download the windows zip file from the releases page and save it to your disk.
    Then, before you open or unzip it, right-click on it and select Properties; at the bottom of 
     the dialog, click the Unblock button and then the OK button.
    Now, open the zip file and copy its contents into a directory on your machine. 
     (You can now delete the zip file.)
    

### Add binary path to Environment Variable, to run dafny from terminal

In Windows, Open the start menu, and type "env"

Click on the option:

    Edit the system environment variables

Click then on Environment Variables

On the top part (User variables) click on the Path variable, and then click edit

Click New, and add the path to the folder you extracted from the Repo. Be sure to put this in an 
sdk folder.
    
---

## Writing a Simple Hello World in Dafny

    method Main() {
        print "Hello, world!";
    }


--- 

## Compiling with Dafny

    dafny HelloWorld.dfy

---

## Executing with DotNet

**Note: This requires Dotnet 6.0 (cross platform, no worries). The Dafny compiler generates this
 .dll file to be executed like this:

    dotnet HelloWorld.dll


Which should then print:

    >: Hello, world!

---


