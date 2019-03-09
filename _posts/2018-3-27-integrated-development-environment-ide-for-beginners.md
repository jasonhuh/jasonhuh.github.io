---
layout: post
title: Integrated Development Environment (IDE) for Beginners
permalink: /2018/03/27/integrated-development-environment-ide-for-beginners
---


When I taught Python to kids for the first time, I asked them to download JetBrain's PyCharm and install it to their laptops. While PyCharm is a wonderful IDE, I found it quite cumbersome when all I want to show them is to how easy it is to print "Hello World" in Python!

So, my students and I ended up using IDLE quite heavily during the class when they were learning specific topics or solving simple problems. When programs contain many lines of code or require debugging, we used PyCharm.

In some cases, they even wrote Python using a note pad, and ran it from a console. I personally use Visual Studio Code, Jupyter Notebok or good old command line, but then I digress. The moral of the story is that there is no single IDE that fits all especially when learning a programming language. The key of an IDE is that the IDE should help learning rather than hindering. For example, Python's IDLE is an excellent tool when students need to learn how to print "Hello World" or quickly prototype a simple function. For a homework assignment that requires 20 lines of code, PyCharm is a better IDE because it automatically saves code to a file and it has lots of features to make programming easier.

In the old days, if you wanted to write "Hello World" in Java, you had to download and install Eclipse, create a workspace, create a project, create a class, create a static main method just to write "Hello World." In these days, students can just visit <a href="http://www.javarepl.com>Java Repl</a> or open `Jshell` and type `System.out.println("Hello World")`! And they feel the sense of accomplishment for seeing "Hello World" working instead of being exhausted with all the plumbing of downloading and installing JDK from Oracle, downloading and installing Eclipse and creating a workspace and project just to write "Hello World".

Here is the list of IDEs for different languages that I use when I teach students. With these IDEs, anyone can easily explore features of programming languages without writing all the plumbings. I intentionally listed only free softwares.

<table>
<tr>
	<th>Language</th>
	<th>Simple IDE or REPL</th>
	<th>More Advanced IDE (Free)</th>
</tr>
<tr>
	<td>Python</td>
	<td><a href="https://www.python.org/downloads/">IDLE</a></td>
        <td>Use PyCharm Community Edition, Visual Studio Code, Atom or Jupyter Notebook</td>
</tr>
<tr>
	<td>JavaScript</td>
	<td>Launch Google Chrome, and hold down `CTRL` and `SHIFT` and press `J`</td>
        <td>Use <a href="http://brackets.io/">Brackets</a> or Atom</td>
</tr>
<tr>
	<td>Java</td>
	<td><a href="http://www.javarepl.com/">Java REPL</a> or JShell.</td>
        <td>Use Eclipse or JetBrain's IntelliJ Community Edition</td>
<tr>
	<td>C++</td>
	<td>Unfortunately, mainstream REPL does not seem to exist for C++ yet.</td>
        <td>Use Xcode for Mac, and use Visual Studio Community Edition for Windows</td>
</tr>
<tr>
	<td>GoLang</td>
	<td><a href="https://play.golang.org/">The Go Playground</a></td>
	<td>Use Visual Studio Code or Atom</td>
</tr>
</table>
