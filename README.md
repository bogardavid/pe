Reverse engineering is hard, and it is hard to find people who are good at it.
Many times , people tend to stop at opening a SRE and learning about architectures. However, that does not answer where the disassembly comes from, and what to do when your SRE fails.
Without understanding file structures, it is not really possible to understand how a SRE works. This problem comes to life when facing static obfuscation, tricking disassemblers and debuggers into outputting mostly junk data, making analysis very difficult if not impossible.
It is true that PE structure modification is not the only way to obfuscate - there is also dynamic obfuscation, which is aimed towards making dynamic analysis more difficult. 

Hence, I have decided to research the PE structure - and I made this repo to share resources that have been useful along the way.

I will be sharing any information that I have found useful along the way, and I will reason why I found it useful.
Hope it helps!

1)
https://en.wikipedia.org/wiki/Portable_Executable#History
- Very nice [drawing](https://upload.wikimedia.org/wikipedia/commons/thumb/1/1b/Portable_Executable_32_bit_Structure_in_SVG_fixed.svg/800px-Portable_Executable_32_bit_Structure_in_SVG_fixed.svg.png) for the PE structure, which is useful for knowing offsets to any data field inside the PE.
- Some technical details about potential uses for the PE sections , for example determining if the architecture is x86 or x64 ( and locating virtually anything via the drawing mentioned earlier).
- 
