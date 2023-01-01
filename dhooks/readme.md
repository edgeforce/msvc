[![www.digitalmars.com](dmlogo.gif)](http://www.digitalmars.com/) [[Home](http://www.digitalmars.com/ "www.digitalmars.com")] [[FAQ](http://www.digitalmars.com/faq.html "Frequently Asked Questions")] [[Search](http://www.digitalmars.com/advancedsearch.html "Search web site")] [[<font color="red">**D**</font>](http://www.digitalmars.com/d/index.html "The D Programming Language")] [[DMC++ CD](http://www.digitalmars.com/shop.html "Digital Mars CD")] [[Gifts](http://www.digitalmars.com/gift/index.html "Gift Shop")]

<table frame="hsides" summary="this table is for layout only" border="1">

<tbody>

<tr>

<td valign="top">

# Digital Mars C/C++ Compilers

## Downloaded Version

The documentation is available online at:

[www.digitalmars.com](http://www.digitalmars.com/)

Much more software (over 300Mb) comes with the CD version, available at:

[www.digitalmars/shop.html](http://www.digitalmars.com/shop.html)

Many useful additional utilities are available:

[Extended Utility Package](http://www.digitalmars.com/eup.html "Extended Utility Package")

For tech support, please use our [online forums](http://www.digitalmars.com/drn-bin/wwwnews?newsgroups=*). These are also accessible as [News Groups](http://www.digitalmars.com/NewsGroup.html "tech support & discussion").

### Installing the Downloaded Version

Digital Mars has a different view of installation than most software products. It doesn't need registry entries, environment variable settings, nor does it need to install anything in the \windows\system directory.

Consequently, the compiler can be run without any need for an install. Just run the programs in \dm\bin. This is most convenient for cases where a particular version of the compiler is needed, or to just try it out.

Installing is as simple as going to the root directory of the hard disk and unzipping the downloaded dm???c.zip file:

<pre>	unzip dm???c.zip
</pre>

The compiler is \dm\bin\dmc.exe. Too make it even more convenient, add

<pre>	c:\dm\bin
</pre>

to the PATH environment variable setting (c: is the drive it is installed on). To compile a simple hello.c program:

<pre>	\dm\bin\dmc hello
</pre>

will compile and link to create hello.exe.

Notes:

*   To use <tt><iostream></tt> and other STL code, download [STLport 4.5.3](ftp://ftp.digitalmars.com/Digital_Mars_C++/STL/stlport.zip "download STLport 4.5.3") as well. Be sure and use the switch:

    <pre><tt>-I\dm\stlport\stlport</tt>
    </pre>

    so that the compiler can find **<iostream>**.
*   Do not install into a subdirectory with spaces, tabs, + signs, commas, or # characters in the subdirectory or path names.

## Full CD Version

Documentation is provided in HTML format, which means it is easiest to read it in a browser, such as Netscape or Explorer.

To read the [documentation](index.html), bring up the browser, and type in:

<pre>	g:\dm\index.html
</pre>

where g is the drive letter of the cdrom drive the Digital Mars CD is in.

## C++ Seminars

If you want to hone your C++ programming skills, see the [Extraordinary C++](http://www.astoriaseminar.com) seminar.

## Questions?

Tech support is provided via the Digital Mars [newsgroup forums](http://www.digitalmars.com/NewsGroup.html).</td>

<td valign="top">[![www.digitalmars.com/d/](images/tdpl.gif)](http://www.digitalmars.com/d/)

[![Empire, the Wargame of the Century (tm)](images/empire200300.jpg)](http://www.classicempire.com/)

[![Maxwell's Equations T-Shirt](images/maxwell.jpg)](http://www.cafepress.com/digitalmars "Maxwell's Equations T-shirt")

[![enquire about advertising](images/dmadvert.gif)](http://www.digitalmars.com/)

</td>

</tr>

</tbody>

</table>