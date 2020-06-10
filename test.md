---


---

<h1 id="files--directories">Files &amp; Directories</h1>
<h2 id="file-management-in-bash">File management in Bash</h2>
<hr>
<p>Files are collections of bits or characters stored in directories/folders (those terms are interchangeable). Let’s start by looking at directories…</p>
<h3 id="home-sweet-home">Home sweet home</h3>
<p>Every linux user has a home directory, let’s move to ours. To do so we use <code>cd</code>{{execute}} (try it now). We can see what the current directory, called the working directory, is by issuing the command <code>pwd</code>{{execute}} or outputting the <code>$PWD</code> variable: <code>echo $PWD</code>{{execute}}. The home directory is where bash looks for its initialisation scripts, which start with one called .bashrc (more about that later).</p>
<p>Your home directory can also be referred to by the symbol <code>~</code>, which is called ‘Tilda’, or by the variable <code>$HOME</code>.</p>
<h3 id="create-new-directories">Create new directories</h3>
<p>To create a new directory called ‘wibble’ we would type <code>mkdir wibble</code>{{execute}} (I use the term ‘wibble’ a lot, because its fast to search for with few false positive results). To create a set of nested directories all at once we would use the <code>-p</code> flag like this <code>mkdir -p src/main/java</code>{{execute}}. The <code>-p</code> flag also promises to never throw an error, which can be quite a useful feature when creating directories in a script. Once a directory is created we can move to it <code>cd src/main/java</code>{{execute}}.</p>
<h3 id="files">Files</h3>
<p>In Linux almost everything is a file. A file is actually a pointer to a collection of bytes, and some very strange things are classed as files in Linux. We can create an empty file using the command <code>touch</code>, as in <code>touch myfile.txt</code>{{execute}}.</p>

