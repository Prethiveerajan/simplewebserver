# Developing a Simple Webserver
## AIM:
To develop a simple webserver to serve html pages.

## DESIGN STEPS:
### Step 1: 
HTML content creation
### Step 2:
Design of webserver workflow
### Step 3:
Implementation using Python code
### Step 4:
Serving the HTML pages.
### Step 5:
Testing the webserver

## PROGRAM:
from http.server import HTTPServer, BaseHTTPRequestHandler
content = """
<!DOCTYPE html>
<html>
<head>
<title>My webserver</title>
</head>
<body>
<h1>Top 5 programming langauges </h1>

<h2>JAVA SCRIPT</h2><br>

<h3>java script often abbreviated as JS, is a programming language that conforms to the ECMAScript specification. JavaScript is high-level, often just-in-time compiled and multi-paradigm. It has dynamic typing, prototype-based object-orientation and first-class functions.</h3>


<h2> advantages of java script </h2>


<h3>  1. Client-side JavaScript is very fast because it can be run immediately within the client-side browser. Unless outside resources are required, JavaScript is unhindered by network calls to a backend server.<br>

2. JavaScript is relatively simple to learn and implement.<br>

3. JavaScript is used everywhere on the web.<br>

4. JavaScript plays nicely with other languages and can be used in a huge variety of applications.<br>

5. Being client-side reduces the demand on the website server. 
Gives the ability to create rich interfaces.</h3> <br>



<h2> disadvantages of java script </h2>  

<h3>1.Side Security. Because the code executes on the users’ computer, in some cases it can be exploited for malicious purposes. This is one reason some people choose to disable Javascript.<br>

2. JavaScript is sometimes interpreted differently by different browsers. This makes it somewhat difficult to write cross-browser code.  </h3> <br>  

<h2>PYTHON </h2>

<h3>Python is an interpreted high-level general-purpose programming language. Its design philosophy emphasizes code readability with its use of significant indentation. Its language constructs as well as its object-oriented approach aim to help …
</h3><br>
<h2> advantages of python</h2>

<h3> 1. Extensive Libraries
Python downloads with an extensive library and contains code for various purposes like regular expressions, documentation-generation, unit-testing, web browsers, threading, databases, CGI, email, image manipulation, and more.
<br>  
2. Affordable
Python is free therefore individuals, small companies or big organizations can leverage the free available resources to build applications.
Python is popular and widely used so it gives you better community support.
The 2019 Github annual survey showed us that Python has overtaken Java in the most popular programming language category.<br>

3. Python is for Everyone
Python code can run on any machine whether it is Linux, Mac or Windows.
Programmers need to learn different languages for different jobs but with Python, you can professionally build web apps, perform data analysis and machine learning, automate things, do web scraping and also build games and powerful visualizations.<br>

<h2>disadvantage of python </h2> 

<h3> 1. Speed Limitations
We have seen that Python code is executed line by line. But since Python is interpreted, it often results in slow execution.
This, however, isn’t a problem unless speed is a focal point for the project.<br>

2. Weak in Mobile Computing and Browsers
While it serves as an excellent server-side language, Python is much rarely seen on the client-side.
Besides that, it is rarely ever used to implement smartphone-based applications. One such application is called Carbonnelle.
The reason it is not so famous despite the existence of Brython is that it isn’t that secure<br>
 </h3> 

 <h2> C++ </h2>

 <h3>C++ is a general-purpose programming language created by Bjarne Stroustrup as an extension of the C programming language, or "C with Classes". The language has expanded significantly over time, and modern C++ now has object-oriented, generic, and functional features in addition to facilities for low-level memory manipulation </h3>

<h2>advantages of c++ </h2>

<h3> 1.C++ provides this feature of portability allowing us to develop codes without caring about the hardware. This lets us move the development of a program from one platform to another.

For example, you’re working on Windows OS and for some reason, you have to switch to LINUX, the codes from Windows OS will also run in the LINUX OS without any error.

2. Mid-level programming language
Being a mid-level programming language, we can treat it as both a low-level and high-level language. Features of high-level language help to develop games and desktop applications, whereas features of low-level language help make kernels and drivers. </h3>

<h2>  disadvantages of c++ </h2>

<h3>1.When it comes to pointers in C++, it is a very tough conception compared to other topics. Uninitialized pointers might result in system failure
Memory corruption can also take place if one puts wrong values in the same. To sum up, debugging pointer bugs is very difficult and hence one of the major disadvantages of C++.<br>
2.C++ doesn’t support garbage collectors, this means that the entire power to manage the data memory goes in the hands of the user. Absence of the same results in redundant data being stored in turn increasing the memory<br>.
3. C++ is unsafe in a strong sense. The presence of pointers, global variables, etc. is the main reason behind these security issues. It means it is possible to corrupt the entire program just by using a part of the memory as an incorrect type.<br>
  </h3>
  

  <h2>JAVA </h2>
      
   <h3> Java is a high-level, class-based, object-oriented programming language that is designed to have as few implementation dependencies as possible. It is a general-purpose programming language intended to let programmers write once, run anywhere (WORA), meaning that compiled Java …  </h3>   
   
   <h2>advantages of java </h2>
 

<h3>1.It is anything but difficult to program, compose, gather, investigate, and learn than elective programming dialects. Java might be a more modest sum convoluted than C++; therefore, Java utilizes programmed memory portion and trash assortment.<br>
2.It grants you to make standard projects and reusable code.<br>
3.It runs on any machine that needn’t bother with any unique programming to be introduced, however, the JVM should be available on the machine.<br>
4.Java is a dispersed language as it gives an instrument for dividing information and projects between numerous PCs that improve the presentation and proficiency of the framework. The RMI(Remote Method Invocation) is something that bolsters the dispersed handling in Java. <br>  </h3>

     
   <h2> disadvantages of java </h2>
    <h3>
1.It is a more slow language when contrasted with different dialects as it is a memory burning-through language.<br>

2.The default look of GUI applications written in Java utilizing the Swing toolbox is very not quite the same as local applications.<br>

3.In Java, Memory is overseen through trash pickup, at whatever point the refuse gatherer runs, it influences the exhibition of the apparatus. This is frequently in light of the fact that all different strings inside the require to be halted to allow the junk authority string to figure.<br>

4.Java requires a critical or significant measure of memory space when contrasted with different dialects like C and C++. During the execution of trash assortment, the memory productivity and the exhibition of the framework might be unfavorably influenced. <br>
</h3>


<h2>Swift</h2><BR>
<h3>Apple in 2014 created Swift for Linux and Mac applications. It is an
open source programming language which is not difficult to learn. It
upholds nearly everything from programming language Objective. Contrasted with other programming dialects, quick takes less
coding.</h3>
<h2> advantages of swift </h2>
<h3>1. Easy to read <BR> 
2.Easy to add new lineaments <BR>
3. No long guidelines<br>
4. Prevents memory leakage </h3> <BR>
<h2> disadvantages of swift </h2> <br>
 <h3>1. Volatile due to continuous updation <br>
 2. Limited </h3>

</body>
</html>
"""
class myhandler(BaseHTTPRequestHandler):
    def do_GET(self):
        print("request received")
        self.send_response(200)
        self.send_header('content-type', 'text/html; charset=utf-8')
        self.end_headers()
        self.wfile.write(content.encode())
server_address = ('',8080)
httpd = HTTPServer(server_address,myhandler)
print("my webserver is running...")
httpd.serve_forever()


## OUTPUT:


## RESULT:
