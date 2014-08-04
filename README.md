Setting proxy to your terminal:
============================

in mac osx .bash_profile loads every time you login to a terminal
so what i did was to add

in .bash_profile file
==============
alias i:'source ~/.bashrc'

in .bashrc file
==============

export http_proxy="http://10.10.78.22:3128"
export https_proxy="http://10.10.78.22:3128"

hit i on terminal to set it to proxy
=======

eg

vissu:~ Viswatejag$ curl www.google.com
curl: (7) Failed to connect to 2404:6800:4007:801::1010: No route to host
vissu:~ Viswatejag$ i
vissu:~ Viswatejag$ curl www.google.com
<HTML><HEAD><meta http-equiv="content-type" content="text/html;charset=utf-8">
<TITLE>302 Moved</TITLE></HEAD><BODY>
<H1>302 Moved</H1>
The document has moved
<A HREF="http://www.google.co.in/?gfe_rd=cr&amp;ei=7W7fU7TvK4bV8gfy_4DwCA">here</A>.
</BODY></HTML>



making git woring on the terminal under proxy settings mac os x


