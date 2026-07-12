<pre style="background:#0D1117;color:#C9D1D9;padding:20px;border-radius:10px;font-family:'Fira Code','JetBrains Mono',monospace;line-height:1.45;overflow-x:auto;">

<span style="color:#61AFEF;">0x7fffffffdf00</span>   <span style="color:#D19A66;">+---------------------+</span>
                 <span style="color:#D19A66;">|</span> <span style="color:#C9D1D9;">Buffer</span>              <span style="color:#D19A66;">|</span>
                 <span style="color:#D19A66;">|</span> <span style="color:#98C379;">\x90 \x90 \x90 \x90</span> <span style="color:#D19A66;">|</span>
<span style="color:#61AFEF;">0x7fffffffdf04</span>   <span style="color:#D19A66;">|</span> <span style="color:#98C379;">\x90 \x90 \x90 \x90</span> <span style="color:#D19A66;">|</span>
<span style="color:#61AFEF;">0x7fffffffdf08</span>   <span style="color:#D19A66;">|</span> <span style="color:#98C379;">\x90 \x90 \x90 \x90</span> <span style="color:#D19A66;">|</span>
<span style="color:#61AFEF;">0x7fffffffdf0c</span>   <span style="color:#D19A66;">|</span> <span style="color:#98C379;">\x90 \x90 \x90 \x90</span> <span style="color:#D19A66;">|</span>
<span style="color:#61AFEF;">0x7fffffffdf10</span>   <span style="color:#D19A66;">+---------------------+</span>
                 <span style="color:#D19A66;">|</span> <span style="color:#C9D1D9;">Saved RBP</span>           <span style="color:#D19A66;">|</span>
                 <span style="color:#D19A66;">|</span> <span style="color:#98C379;">\x90 \x90 \x90 \x90</span> <span style="color:#D19A66;">|</span>
<span style="color:#61AFEF;">0x7fffffffdf14</span>   <span style="color:#D19A66;">|</span> <span style="color:#98C379;">\x90 \x90 \x90 \x90</span> <span style="color:#D19A66;">|</span>
<span style="color:#61AFEF;">0x7fffffffdf18</span>   <span style="color:#D19A66;">+---------------------+</span>
                 <span style="color:#D19A66;">|</span> <span style="color:#E06C75;">Return Address</span>      <span style="color:#D19A66;">|</span>
                 <span style="color:#D19A66;">|</span> <span style="color:#61AFEF;">0x7fffffffdf20</span>      <span style="color:#D19A66;">|</span>---+
<span style="color:#61AFEF;">0x7fffffffdf20</span>   <span style="color:#D19A66;">+---------------------+</span>   |
                 <span style="color:#D19A66;">|</span> <span style="color:#E5C07B;">Shellcode</span>           <span style="color:#D19A66;">|</span>&lt;--+
                 <span style="color:#D19A66;">|</span> <span style="color:#98C379;">\x48 \x31 \xf6 \x48</span> <span style="color:#D19A66;">|</span>
<span style="color:#61AFEF;">0x7fffffffdf24</span>   <span style="color:#D19A66;">|</span> <span style="color:#98C379;">\x31 \xd2 \x4d \x31</span> <span style="color:#D19A66;">|</span>
<span style="color:#61AFEF;">0x7fffffffdf28</span>   <span style="color:#D19A66;">|</span> <span style="color:#98C379;">\xc0 \x48 \xbb \x2f</span> <span style="color:#D19A66;">|</span>
<span style="color:#61AFEF;">0x7fffffffdf2c</span>   <span style="color:#D19A66;">|</span> <span style="color:#98C379;">\x62 \x69 \x6e \x2f</span> <span style="color:#D19A66;">|</span>
<span style="color:#61AFEF;">0x7fffffffdf30</span>   <span style="color:#D19A66;">|</span> <span style="color:#98C379;">\x73 \x68 \x00 \x53</span> <span style="color:#D19A66;">|</span>
<span style="color:#61AFEF;">0x7fffffffdf34</span>   <span style="color:#D19A66;">+---------------------+</span>

</pre>
