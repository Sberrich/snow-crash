NB

Le fichier /etc/passwd contient toutes les informations
relatives aux utilisateurs (login, mots de passe, ...).
Seul le superutilisateur (root) doit pouvoir le modifier.
Il faut donc modifier les droits de ce fichier de façon à ce qu'il soit
en lecture seule pour les autres utilisateurs.

1 --> Go To /etc/ then cat the passwd file
2 --> in the cat of the file we find this hash '42hDRfypTqqnw'
3 --> Download the john program
4 --> decrypt the hash with the john decrypter we get the password 'abcdefg'
5 --> su flag01 with the password 'abcdefg'
6 --> gettheflag Check flag.Here is your token : f2av5il02puano7naaf6adaaf
