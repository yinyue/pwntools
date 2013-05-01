This is the CTF framework used by pwnies in every CTF.

Most code is inside the pwn folder, which is typically used as:

    from pwn import *
    context('i386', 'linux')

    # EXPLOIT HERE

However we have made command-line frontends for much of the functionality
inside the pwnlib. These are:

* cyclic: De Bruijn sequence generator and lookup tool
* hex/unhex: Command line tools for doing common hexing/unhexing operations
* nops: Tool for generating random nopsleds.
* peek/poke: Simple tool for sending files over a LAN
* randomua: Returns a random user agent
* scramble: Shellcode packer
* shellcraft: Frontend to our shellcode

We also have the following tools, not dependent on the pwnlib:

* asm/disasm: Small wrapper for nasm
* binutils: Assemblers and disassemblers for various architectures
* demo: Tool for testing shellcode

All of these tools are symlinked to the bin folder.

To install it, just update your PYTHONPATH and PATH variables. Alternatively
you can run install.sh.

If you have any questions not worthy of a bug report, feel free to join us
at #zomg\_pwnies and ask away.