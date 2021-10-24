# React-routing-reload-build-required-file
React-routing-reload-build-required-file

Create ".htaccess" and paste below text file and push with bild file it's resolve reload issue of your reactJs Project
<IfModule mod_rewrite.c>

  RewriteEngine On
  RewriteBase /
  RewriteRule ^index\.html$ - [L]
  RewriteCond %{REQUEST_FILENAME} !-f
  RewriteCond %{REQUEST_FILENAME} !-d
  RewriteCond %{REQUEST_FILENAME} !-l
  RewriteRule . /index.html [L]

</IfModule>
