<h1 align="center">
  <img src="https://readme-typing-svg.demolab.com/?font=Fira+Code&size=22&pause=1000&color=39FF14&center=true&vCenter=true&width=650&lines=whoami+%3D%3E+tharun;pwn+%2B+full-stack+dev;overflowing+the+stack%2C+not+the+deadline" alt="typing-svg" />
</h1>

<p align="center">
  <img src="https://komarev.com/ghpvc/?username=THARUN-BART&label=PROFILE+VIEWS&color=39FF14&style=for-the-badge" />
  <img src="https://img.shields.io/github/followers/THARUN-BART?label=FOLLOWERS&style=for-the-badge&color=39FF14&logo=github&logoColor=black" />
</p>

<p align="center"><i>gdb-peda$ file tharun.elf</i></p>
<p align="center"><code>tharun.elf: ELF 64-bit LSB, human, dynamically linked, not stripped</code></p>

<br>

## 0x00 — whoami

```bash
$ ./whoami
> Computer Science student. Full-stack dev. Rust compiler contributor.
> Goal: land a SWE seat @ a top product company.
> Uptime: 19 years, 7 months, 12 days — no reboot yet.
```

## 0x01 — stack_frame (tharun.elf)

```text
                    ┌── STACK MEMORY — grows downward ⬇ ──┐
   high addr
   0x7ffd21e0e050 │ argv[] / envp[]                       │ OS : Arch Linux · Windows 11 · Android
   0x7ffd21e0e048 │ >> RETURN ADDRESS <<  ────────────┐   │ overwritten → redirects rip below
                  │                                    │   │
   0x7ffd21e0e040 │ saved RBP     = 0x00000c5 (CS-BASE)│   │ Kernel : Computer Science Student
   0x7ffd21e0e038 │ stack canary  = 0xdeadb17e          │   │ Achv.  : contributed to the Rust compiler
   0x7ffd21e0e030 │ buf[64]  "GOAL=swe_at_top_product…"│   │ Goal   : Software Engineer @ Top Product Co
   0x7ffd21e0e020 │ buf[40]  ide  = vscode, android-std │   │ IDE    : VS Code, Android Studio
   0x7ffd21e0e010 │ buf[24]  ▓▓▓▓▓ overflow padding ▓▓▓▓ │
   low addr        └────────────────────────────────────┘
                                                            │
                    rip hijacked ──────────────────────────┘
                        │
                        ▼
                  jmp 0x0badc0de   ; see shellcode.payload below
```

## 0x02 — shellcode.payload  *(what the hijacked `rip` jumps to)*

```asm
section .payload
_shellcode:
    ; --- registers loaded with skillset before syscall ---
    mov rax, [langs_programming]   ; C++, Python, Dart, SQL, Rust
    mov rbx, [langs_computer]      ; JSON, YAML, Markdown
    mov rcx, [langs_human]         ; English, Tamil

    mov rdx, [hobbies_software]    ; Flutter App Dev, LeetCoding
    mov rsi, [hobbies_cloudops]    ; Cloud Infrastructure, Self-Hosting
    mov rdi, [currently_learning]  ; System Design, DSA, DevSecOps, Rust

    xor r8,  r8                    ; bugs remaining (asymptotically → 0)
    syscall                        ; execve("/bin/ship_it", NULL, NULL)
```

<p align="center">
  <img src="https://img.shields.io/badge/C%2B%2B-00599C?style=for-the-badge&logo=cplusplus&logoColor=white" />
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/Dart-0175C2?style=for-the-badge&logo=dart&logoColor=white" />
  <img src="https://img.shields.io/badge/SQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white" />
  <img src="https://img.shields.io/badge/Rust-000000?style=for-the-badge&logo=rust&logoColor=white" />
  <br>
  <img src="https://img.shields.io/badge/JSON-000000?style=for-the-badge&logo=json&logoColor=white" />
  <img src="https://img.shields.io/badge/YAML-CB171E?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Markdown-000000?style=for-the-badge&logo=markdown&logoColor=white" />
  <img src="https://img.shields.io/badge/Flutter-02569B?style=for-the-badge&logo=flutter&logoColor=white" />
  <img src="https://img.shields.io/badge/VS%20Code-007ACC?style=for-the-badge&logo=visualstudiocode&logoColor=white" />
  <br>
  <img src="https://img.shields.io/badge/Arch%20Linux-1793D1?style=for-the-badge&logo=arch-linux&logoColor=white" />
  <img src="https://img.shields.io/badge/Windows%2011-0078D6?style=for-the-badge&logo=windows11&logoColor=white" />
  <img src="https://img.shields.io/badge/Android-3DDC84?style=for-the-badge&logo=android&logoColor=white" />
  <img src="https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white" />
</p>

## 0x03 — currently_fuzzing *(learning right now)*

```diff
+ System Design
+ Data Structures & Algorithms
+ DevSecOps
+ Rust (going deeper)
```

## 0x04 — resolved_symbols  *(contact)*

```text
readelf --dyn-syms tharun.elf | grep GLOBAL
```

<p align="center">
  <a href="mailto:tharunpoongavanam@gmail.com">
    <img src="https://img.shields.io/badge/Email-tharunpoongavanam%40gmail.com-39FF14?style=for-the-badge&logo=gmail&logoColor=black" />
  </a>
  <br>
  <a href="https://linkedin.com/in/tharundeveloper">
    <img src="https://img.shields.io/badge/LinkedIn-tharundeveloper-39FF14?style=for-the-badge&logo=linkedin&logoColor=black" />
  </a>
  <br>
  <a href="https://instagram.com/bart_simpson_og_001">
    <img src="https://img.shields.io/badge/Instagram-bart__simpson__og__001-39FF14?style=for-the-badge&logo=instagram&logoColor=black" />
  </a>
  <br>
  <a href="https://github.com/THARUN-BART">
    <img src="https://img.shields.io/badge/GitHub-THARUN--BART-39FF14?style=for-the-badge&logo=github&logoColor=black" />
  </a>
</p>

## 0x05 — gdb$ info stats

<p align="center">
  <img height="165" src="https://github-readme-stats.vercel.app/api?username=THARUN-BART&show_icons=true&theme=merko&hide_border=true&bg_color=0D1117&title_color=39FF14&icon_color=39FF14&text_color=c9d1d9" />
  <img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=THARUN-BART&layout=compact&theme=merko&hide_border=true&bg_color=0D1117&title_color=39FF14&text_color=c9d1d9" />
</p>

<p align="center">
  <img src="https://streak-stats.demolab.com?user=THARUN-BART&theme=merko&hide_border=true&background=0D1117&ring=39FF14&fire=39FF14&currStreakLabel=39FF14" />
</p>

<p align="center">
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=THARUN-BART&theme=react-dark&bg_color=0D1117&color=39FF14&line=39FF14&point=c9d1d9&hide_border=true" />
</p>

---

<p align="center">
<pre align="center">
[+] Exploit successful — shell spawned as tharun-bart
[*] Segfault-free since git init
[$] echo "thanks for stopping by — drop a ⭐ if you like the exploit"
</pre>
</p>
