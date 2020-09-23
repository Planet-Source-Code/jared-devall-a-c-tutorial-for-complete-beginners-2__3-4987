<div align="center">

## A C\+\+ Tutorial for Complete Beginners \#2


</div>

### Description

This is the followup tutorial to "A C++ Tutorial for Complete Beginners #1". This article explains Variables!
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Jared Devall](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/jared-devall.md)
**Level**          |Beginner
**User Rating**    |4.6 (311 globes from 67 users)
**Compatibility**  |C\+\+ \(general\), Microsoft Visual C\+\+, Borland C\+\+, UNIX C\+\+
**Category**       |[Miscellaneous](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/miscellaneous__3-1.md)
**World**          |[C / C\+\+](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/c-c.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/jared-devall-a-c-tutorial-for-complete-beginners-2__3-4987/archive/master.zip)





### Source Code

<font size = "2">
<BR><BR>
Well, Hello World, Again! It's been quite a while since my previous Tutorial; time for a new
one!<BR><BR>
This tutorial will assume you've read "<a href =
"http://www.planet-source-code.com/vb/scripts/ShowCode.asp?txtCodeId=2040&lngWId=3"> A C++
Tutorial for Complete Beginners #1</a>" as this is #2. This tutorial will also assume you
understand the concepts presented in the previous tutorial and can make use out of it.
:)<BR><BR>
<font size = "1"> *Note: I've since changed to using MS Visual C++ 6.0 </font><BR><BR>
Notes:<BR>
- <font color="blue">Blue</font> denotes a <a href = "#">keyword</a><BR>
- Term Dictionary still not in use. ( Links don't work. )<BR><BR>
I'm going to cover variables in this article. So, get ready! :)<BR><BR>
<b>Variables:</b><BR>
<a href = "#">Variable</a>s are aliases for memory locations. That is, they hold some kind
of data that you put inside of it. You declare a variable by choosing a <a href = "#">data
type</a>, and choose a name or keyword to assign to the variable. There are, however,
reserved KEYWORDS that you cannot use, as they are critical to C++ Programming. <BR><BR>
A list of Data Types:<BR>
<ul>
<font size = "2">
<li> char - 1 byte - This represents ONE character. e.g. b</li>
<li> int - 2 or 4 bytes - This for a number. e.g. 500 or -500</li>
<li> short - 2 bytes - This is also a number, but is smaller than int.</li>
<li> long - 4 or 8 bytes - This is the largest number type.</li>
<li> bool - 1 byte - This is a boolean value. ( true or false )</li>
</font>
</ul>
Data types can change from system to system, but these are the 'normal' sizes for these
types. There can be both signed, and <font color="blue">unsigned</font> numbers. Signed
meaning the number can be negative, and <font color="blue">unsigned</font> meaning the
lowest value the variable can have is 0.<BR><BR>
Size   Sign   Minimum Value   Maximum
Value<BR>
 1     signed  -128            127<BR>
 1   unsigned  0               255 (normal <b>char</b>)<BR>
 2     signed  -32768          32768 (normal <b>short/int</b>)<BR>
 2   unsigned  0               65535<BR>
 4     signed  -2147483548     2147483647 (normal <b>long</b>)<BR>
 4   unsigned  0               4294967295<BR>
<BR>
Types default to signed unless you specify that it is <font color="blue">unsigned</font>,
like so:<br>
<i>unsigned int</i><BR><BR>
C++ is a very CASE-SENSITIVE language. What this means is that if you have 3 variables:<BR>
<i>TestVariable<BR>
testVariable<BR>
testvariable</i><BR><BR>
These variables are different. It's important to develop a consistent style of naming
variables. I normally keep variables lowercase, with an uppercase specifying a new word,
like so:<BR>
<i>testVariable</i><BR><BR>
Now that you know what data types and variables are you can <a href = "#">declare</a> them.
You declare them like so:<BR>
<i><font color="blue">int</font> myNumber;</i> <font size = "1">*Note: You must have the
semi-colon at the end!</font><BR>
You can also <a href = "#">define</a> them in their declaration:<BR>
<i><font color="blue">int</font> myNumber = 2002;</i><BR><BR>
<font color="blue">Char</font>'s are done close to the same way, except when you define them
you must put the letter in <b>single quotations</b> (  <i>'</i>  ). Character <a
href = "#">string</a>s, however, must be done a different way since the <font
color="blue">char</font> type can only hold ONE character at a time. ( Yes, that mean it can
only hold one A or one B at a time! ). Strings will be discussed in a later tutorial.
<BR><BR>
A <font color="blue">bool</font>(ean) can only be <font color="blue">true</font> or <font
color="blue">false</font>, or their counterparts: 0 and 1. Booleans are normally used in
<font color="blue">if</font> statements and other C++ goodies.<BR><BR>
Okay, wipe that sweat from your brow! This was a difficult and large chunk of information to
swallow. Let's end this up with a small program that utilizes what was presented
here.<BR><BR><BR>
Open up whatever program you used in the last tutorial and follow the steps on compiling I
showed you before. Again, remove the numbers from the source code as they are only there to
help analyze the code! Save as tutorial.cpp<BR><BR>
<HR>
1. #include <iostream.h><BR>
2. <BR>
3. int main( )<BR>
4. {<BR>
5. 	<font color="blue">int</font> myNumber;<BR>
6. 	<font color="blue">long</font> myNumber2 = 5;<BR>
7.	<font color="blue">char</font> myCharacter;<BR>
8.	<font color="blue">char</font> myCharacter2 = 'c';<BR>
9.	<font color="blue">bool</font> myBoolean;<BR>
10.	<font color="blue">bool</font> myBoolean2 = <font color="blue">true</font>;<BR>
11.<BR>
12.<BR>
13.	myNumber = 3678;<BR>
14.	myCharacter = 'a';<BR>
15.	myBoolean = <font color="blue">false</font>;<BR>
16.<BR>
17.	cout << "myNumber = " << myNumber << endl;<BR>
18.	cout << "myNumber2 = " << myNumber2 << endl << endl;<BR>
19.<BR>
20.	cout << "myCharater = " << myCharacter << endl;<BR>
21.	cout << "myCharacter2 = " << myCharacter2 << endl << endl;<BR>
22.<BR>
23.	return 0;<BR>
24. }<BR><BR>
<hr>
Okay, now, the line-by-line analysis!<BR><BR>
Line 1: This includes the <i>iostream.h</i> header. This, ofcourse, is needed for cout and
endl.<BR><BR>
Line 2: This is just whitespace.<BR><BR>
Line 3: This is the main function mentioned in the last tutorial. You will always see one of
these in any C++ program.<BR><BR>
Line 4: This is just the opening brace for the main function.<BR><BR>
Line 5 & 6: These two lines declare one <font color="blue">int</font> and one <font
color="blue">long</font> variable. <i>myNumber2</i> is also defined on this line with the
value 5.<BR><BR>
Line 7 & 8: These two lines both declare a <font color="blue">char</font> variable.
<i>myCharacter2</i> also defines itself with the value c.<BR><BR>
Line 9 & 10: These two lines both declare a <font color="blue">bool</font> variable.
<i>myBoolean2</i> also defines itself to <font color="blue">true</font><BR><BR>
Line 11 & 12: Both of these lines are cosmetics: a.k.a. whitespace.<BR><BR>
Line 13 - 15: These lines define these variables to a specific value.<BR><BR>
Line 16: Whitespace again!<BR><BR>
Line 17 & 18: These lines display the variables' values to the screen, sending an 'endl' to
go to the next line.<BR><BR>
Line 19: Guess what this is! Yup, you guessed it, whitespace!<BR><BR>
Line 20 & 21: These lines also display the variables' values to the screen, sending an
'endl' to the next line.<BR><BR>
Line 22: ...whitespace...<BR><BR>
Line 23: This is the return statement. This will be explained in the next tutorial, along
with the mystical "function". <BR><BR>
Line 24: This is simply the closing brace. This ends the function, and effectively ends our
program. ( When <i>main</i> is done, our program is done! )<BR><BR><BR>
For ease of explanation, whitespace will not be mentioned in future tutorials. I think we
all know what it is. :)<BR><BR>
This program simply declares and defines a few simple variables. It then takes those
variables with printable values and prints them to the screen with <i>cout</i>. Again, this
program will most likely close immediately upon execution. Just open up some kind of
command-line and run it from there.<BR><BR>
This concludes "A C++ Tutorial for Complete Beginners #2". As always, if anything is too
complicated to understand or if I screwd up, be sure to let me know. Please let me know if
you would like something explained a little more indepth, or whatever else. ( Please have it
pertain to the topics discussed in this tutorial. ) I'll try to get the fixes when I
can!<BR><BR>
- Jared
</font>

