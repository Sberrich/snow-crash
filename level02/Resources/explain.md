level02

PCAP "packet capture" Extention

1 --> First step we Download the level02.pcap in this path by using "scp -P 4242 level02@10.12.100.128:/home/user/level02/level02.pcap /Users/sberrich/Desktop/snowcrach/level02/Resources"
2 --> Go in to https://www.cloudshark.org/captures then we upload the file in cloudshark then enter to the analysis tools then Follow TCP Stream 0 in level02.pcap
3 --> we get the password in this format : Password:
f
t
\_
w
a
n
d
r
.
.
.
N
D
R
e
l
.
L
0
L

"NB" --> The dots are "non-printable" characters (i.e. there is no ASCII representation of them). They are likely to be binary data values. The hex display pane will show the the exact values

4 --> in this case the dots == del So the password it will be like this = ft_waNDReL0L
5 --> su flag02 with the password : ft_waNDReL0L
6 --> Don't forget to launch getflag !'
7 --> Check flag.Here is your token : kooda2puivaav1idi4f57q8iq
