# TDD-Console
Basic TDD "hands-on" concept for a small console app / script

## Goal
Take first steps with Test-Driven Development, with very few prerequisites. Most editing is done online in a public repository at github.com (recommended).

### Development
A console application is being developed step-by-step. Any programming language and environment may be used, as long as...

1. the application can be invoked with a command line like this:
```
<*> <your-app-param-1> <your-app-param-2> ... <your-app-param-n>
```
\* whatever commands, parameters, etc., are needed to launch your app. An optional compile step is also supported.

_And_
2. it is able to print to "standard" - and possibly also "error" - output, and then finishes. I.e., a GUI is not needed, and probably even undesired, as it is not subject to test evaluation, and may cause the execution flow to block etc.

The code is created and elaborated online, and should fit into one file.

### Test code
The test "code" is also created and elaborated online, in a Markdown (`.md`) file. Actually only the "app parameters" and the expected results are specified.

## Running
An online code editing and versioning platform like github.com doesn't run code. Even if it did, the TDD learner's favorite language may not be supported.
So this concept suggests two ways to run (test) the code:

### On a device at hand
This may (or may not) be the same device as the one used for online editing the test and code in the public repository.

A small app(lication) has to be downloaded and started, which (1) obtains fresh copies of the online files and (2) executes the console application being developed, according to the current test specification. The results are displayed. Steps 1-2 are repeated as requested by the user, until this "test looper" app(lication) is closed.

Currently, a `.cmd` script is [available for Windows](#windows-test-looper), but similar tools may be created for all kinds of platforms, provided that an app(lication) on a given platform is allowed to download code from the repository, and execute it.

If a compiler or interpreter isn't available for the programming language to be used for development, additional software installation may be needed in order to get the setup up and running. E.g., no current version of Windows has a PHP interpreter installed by default. Installing XAMPP is an option in this case, and it also provides a Perl interpreter.

### On a reachable web server
In this case, the test loop is triggered via a web UI, and also the test results are displayed that way, since the test and code are being run on a remote machine (but still, not on the _repository_ server).

An advantage of this setup is the fact that only the "terminal" device needs to be at hand. It is used for code editing as well as triggering and viewing the test, and thus only needs to access the respective web servers - and preferably it has a decent screen and keyboard. In any case, no particular installation and execution privileges are needed on this device.

