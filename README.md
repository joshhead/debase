Usage: debase file.zip 

Output:
<pre>
&lt;!DOCTYPE html&gt;
&lt;html&gt;
&lt;body&gt;
&lt;p&gt;Encoded Data Follows. To automatically decode, please enable JavaScript.&lt;br /&gt;
MIME type: application/zip&lt;/p&gt;
&lt;pre id="encoded_data"&gt;
UEsDBBQAAAAIABJydD/7dxYusAAAALIAAAAKABwA
c3F1YXJlLmdpZlVUCQADE1LJThhSyU51eAsAAQTo
AwAABOgDAABz93SzsEzkYeBhaJFmyOi53rn0Qcey
B53LHkxa83jymkdzNj+Zs/np0t3Pl+5+sf7Qqx2n
3uw49fbQxfeHL74/c+PjmRufrt7/cu/Zt/vPvr94
++PFu5+fvvz5+PX3x69/Pn39/enrn/+oQPEnCyMX
gzyDDgMQgOxkYNV/oJq1ZGrnjFDGnNdBk7SZg012
XyzePmHz5t6j/AcCeEQ7FR8ZmIi0tTQqOCzlW9Mo
wGANAFBLAQIeAxQAAAAIABJydD/7dxYusAAAALIA
AAAKABgAAAAAAAAAAAC0gQAAAABzcXVhcmUuZ2lm
VVQFAAMTUslOdXgLAAEE6AMAAAToAwAAUEsFBgAA
AAABAAEAUAAAAPQAAAAAAA==
&lt;/pre&gt;
&lt;script type="text/javascript"&gt;
location.href="data:application/zip;base64,"+
document.getElementById("encoded_data").innerHTML;
&lt;/script&gt;
&lt;/body&gt;
&lt;/html&gt;
</pre>

Save the text as file.zip.html and open in a modern web browser. When prompted, save the download as file.zip to recover the original data.

The MIME type is included with the data, so images and some text may be displayed directly in the browser.

___

*Rationale*

Have you every wanted to send somebody a file but found it needlessly difficult?
Maybe your mail provider won't let you send executables.
Maybe you have a remote desktop solution for accessing a PC that supports clipboard sharing but no file transfer.
Maybe you are sending instant messages but are unable to get file transfer working.

It's often easier to send somebody plain text over the Internet than to send binary data.
One workaround is to encode a file as base64 data (there are many tools to do this).
It seemed like a natural step to produce a self-decoding file.
Almost everyone has a web browser installed, so using javascript to do the decoding seemed like a good angle.
In fact, I hardly needed any javascript since data links are supported by the browser and take care of the decoding.

Hopefully you will never need this tool because file transfer works fine for you. :)

In any case, it was an interesting exercise for me.
