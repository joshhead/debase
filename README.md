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

* Because I could
* The free version of a remote desktop application supported clipboard sharing but not file transfer.
* It seemed like a good idea at the time.

Almost everyone has a web browser installed, so using javascript to do the decoding seemed like a good angle.
In fact, I hardly needed any javascript since data links are supported by the browser and take care of the decoding.

