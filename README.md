```ansi
0x7fffffffdf00   +---------------------+
                 | Buffer              |
                 | \x90 \x90 \x90 \x90 |
0x7fffffffdf04   | \x90 \x90 \x90 \x90 |
0x7fffffffdf08   | \x90 \x90 \x90 \x90 |
0x7fffffffdf0c   | \x90 \x90 \x90 \x90 |
0x7fffffffdf10   +---------------------+
                 | Saved RBP           |
                 | \x90 \x90 \x90 \x90 |
0x7fffffffdf14   | \x90 \x90 \x90 \x90 |
0x7fffffffdf18   +---------------------+
                 | Return Address      |
                 | 0x7fffffffdf20      |---+
0x7fffffffdf20   +---------------------+   |
                 | Shellcode           |<--+
                 | \x48 \x31 \xf6 \x48 |
0x7fffffffdf24   | \x31 \xd2 \x4d \x31 |
0x7fffffffdf28   | \xc0 \x48 \xbb \x2f |
0x7fffffffdf2c   | \x62 \x69 \x6e \x2f |
0x7fffffffdf30   | \x73 \x68 \x00 \x53 |
0x7fffffffdf34   +---------------------+
```
