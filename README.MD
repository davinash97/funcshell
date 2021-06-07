<h1 align="center">Welcome</h1>
<h2><u>Introduction</u></h2>
<div>
    <p>
        Hello There! Wassup? I Remember When I was new to Linux, I used to Struggle with some of these Commands. So,
        Here it is for those users, who are new to linux. And upto Learning Terminal Stuffs. So, let's just start
        without wasting out time.
    </p>
</div><br>
<h2><u>Funtions</u></h2>
<div>
    <ol>
        <li>
            <details>
                <summary>print</summary><br>
                So, Let's just start by Printing "Hello World!" in the Shell Terminal. Open the <code>start.sh</code> file.
                And write<br><code>print "Hello World!"</code> (or) <code>print "Hello World!" "Green"</code><br><br>
                <b>You Can Use Various Colours.</b><br>
    <ul>
        <li>Some Predefined Colours are:<br></li>
            <code>
                black, red, green, yellow, blue, magenta, cyan, grey.
            </code><br>
        <li>You Can Also Change the Background of Particular Text.<br></li>
            <code>
                black_bg, red_bg, green_bg, yellow_bg, blue_bg, magenta_bg, cyan_bg, grey_bg, invert.<br>
            </code>
    </ul>
            </details>
        </li><br>
        <li>
            <details>
                <summary>print_logo</summary><br>
                Now, The Banner. Which can be seen On top of Every Project. Use <a href="https://www.askapache.com/online-tools/figlet-ascii/">figlet_generator</a>
                to make banners. Now copy that Banner, Make a file (Let's go with logo.txt) & Paste the Code inside the file. Now save and add a
                blank line above & below so that it gets properly Aligned in terminal, Now Close it. The Next Step is to Call the
                <code>print_logo</code>
                function.<br><br>The Syntax to use that function is, <br><code>print_logo "logo.txt"</code> (or) <code>print_logo "logo.txt" "green"</code>
            </details><br>
        </li>
        <li>
            <details>
                <summary>delete</summary><br>
                Now, the Next Function is <code>delete</code>. You can use this function to delete file (or) folder.<br>
                The Syntax for this function is <code>delete "logo.txt"</code>.
            </details><br>
        </li>
        <li>
            <details>
                <summary>permission</summary><br>
                In Linux, You Sometimes need Permission to Open, Execute File(s). To Get Permissions of that
                particular file, You just need to do <code>permission logo.txt</code> and You Can Now Execute (or) Open that
                file.<br><br>
                <b>Note That: You  will have to input your password, As we will need sudo to Change Permission</b>
            </details><br>
        </li>
        <li>
            <details>
                <summary>get_access</summary><br>
                Sometimes, you may have noticed some File(s)/Folder(s) having a Symbol of Lock in that Icon. To get
                Access to that File/Folder just call the <code>get_access</code> Function.Syntax for that funtion
                is<code>get_access "logo.txt"</code>.<br><br>
                <b>Note That: You will have to input your password, As we will need sudo to Change Permission</b>
            </details><br>
        </li>
        <li>
            <details>
                <summary>create_dir</summary><br>
                To Create a Folder named "Example", Do <code>create_dir "Example"</code>
            </details><br>
        </li>
        <li>
            <details>
                <summary>create_file</summary><br>
                To Create a File named "logo.txt", Do <code>create_file "logo.txt"</code>
            </details><br>
        </li>
        <li>
            <details>
                <summary>write</summary><br>
                To Write xyz in "logo.txt", Do <code>write "xyz" "logo.txt"</code>.<br>If the Directory (or) File
                doesn't Exist, Function will automatically Create it.
            </details>
        </li>
    </ol>
</div>
<h2><u>Credits:</u></h2>
<div>
    I would like to thank:
    <ul>
        <li>
            <a href="https://www.github.com/Astrako">Astrako</a>, Who Encouraged me to learn Shell (Now I am loving it).
        </li>
        <li>
            And <a href="https://www.github.com/neel0210">Neel</a>, Who Encouraged me to make this one for Beginners
        </li>
</div>