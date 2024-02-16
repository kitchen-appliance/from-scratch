| opcode        | addr/im              | description                           |
| ------------- | -------------------- | ------------------------------------- |
| 00 add.r8>r8m | modrm (sib disp)     | add r8->r8m (r8m=r8m+r8)              |
| 01 add.r>rm   | modrm (sib disp)     | add r->rm (rm=rm+r)                   |
| 02 add.r8m>r8 | modrm (sib disp)     | add r8m->r8 (r8=r8+r8m)               |
| 03 add.rm>r   | modrm (sib disp)     | add rm->r (r=r+rm)                    |
| 04 add.im8>al | im8                  | add im8->al (al=al+im8)               |
| 05 add.im>a   | im                   | add im->a (a=a+im)                    |
| 06 invalid    |                      | Invalid Instruction in 64-Bit Mode    |
| 07 invalid    |                      | Invalid Instruction in 64-Bit Mode    |
| 08 or.r8>r8m  | modrm (sib disp)     | bitwise or r8->r8m (r8m=r8m|r8)       |
| 09 or.r>rm    | modrm (sib disp)     | bitwise or r->rm (rm=rm|r)            |
| 0A or.r8m>r8  | modrm (sib disp)     | bitwise or r8m->r8 (r8=r8|r8m)        |
| 0B or.rm>r    | modrm (sib disp)     | bitwise or rm->r (r=r|rm)             |
| 0C or.im8>al  | im8                  | bitwise or im8->al (al=al|im8)        |
| 0D or.im>a    | im                   | bitwise or im->a (a=a|im)             |
| 0E invalid    |                      | Invalid Instruction in 64-Bit Mode    |
| 0F esc        |                      | two-byte instructions prefix          |
| 10 adc.r8>r8m | modrm (sib disp)     | add w/carry r8->r8m (r8m=r8m+r8+CF)   |
| 11 adc.r>rm   | modrm (sib disp)     | add w/carry r->rm (rm=rm+r+CF)        |
| 12 adc.r8m>r8 | modrm (sib disp)     | add w/carry r8m->r8 (r8=r8+r8m+CF)    |
| 13 adc.rm>r   | modrm (sib disp)     | add w/carry rm->r (r=r+rm+CF)         |
| 14 adc.im8>al | im8                  | add w/carry im8->al (al=al+im8+CF)    |
| 15 adc.im>a   | im                   | add w/carry im->a (a=a+im+CF)         |
| 16 invalid    |                      | Invalid Instruction in 64-Bit Mode    |
| 17 invalid    |                      | Invalid Instruction in 64-Bit Mode    |
| 18 sbb.r8>r8m | modrm (sib disp)     | sub w/borrow r8>r8m (r8m=r8m-r8-CF)   |
| 19 sbb.r>rm   | modrm (sib disp)     | sub w/borrow r->rm (rm=rm-r-CF)       |
| 1A sbb.r8m>r8 | modrm (sib disp)     | sub w/borrow r8m->r8 (r8=r8-r8m-CF)   |
| 1B sbb.rm>r   | modrm (sib disp)     | sub w/borrow rm->r (r=r-rm-CF)        |
| 1C sbb.im8>al | im8                  | sub w/borrow im8->al (a=a-im8-CF)     |
| 1D sbb.im>a   | im                   | sub w/borrow im->a (a=a-im-CF)        |
| 1E invalid    |                      | Invalid Instruction in 64-Bit Mode    |
| 1F invalid    |                      | Invalid Instruction in 64-Bit Mode    |
| 20 and.r8>r8m | modrm (sib disp)     | bitwise and r8->r8m (r8m=r8m&r8)      |
| 21 and.r>rm   | modrm (sib disp)     | bitwise and r->rm (rm=rm&r)           |
| 22 and.r8m>r8 | modrm (sib disp)     | bitwise and r8m->r8 (r8=r8&r8m)       |
| 23 and rm>r   | modrm (sib disp)     | bitwise and rm->r (r=r&rm)            |
| 24 and.im8>al | im8                  | bitwise and im8->al (al=al&im8)       |
| 25 and.im>a   | im                   | bitwise and im->a (a=a&im)            |
| 26 null       |                      | Null Prefix in 64-bit Mode            |
| 27 invalid    |                      | Invalid Instruction in 64-Bit Mode    |
| 28 sub.r8>r8m | modrm (sib disp)     | sub r8->r8 (r8m=r8m-r8)               |
| 29 sub.r>rm   | modrm (sib disp)     | sub r->rm (rm=rm-r)                   |
| 2A sub.r8m>r8 | modrm (sib disp)     | sub r8m->r8 (r8=r8-r8m)               |
| 2B sub.rm>r   | modrm (sib disp)     | sub rm->r (r=r-rm)                    |
| 2C sub.im8>al | im8                  | sub im8->al (al=al-im8)               |
| 2D sub.im>a   | im                   | sub im->a (a=a-im)                    |
| 2E null       |                      | Null Prefix in 64-bit Mode            |
| 2F invalid    |                      | Invalid Instruction in 64-Bit Mode    |
| 30 xor.r8>r8m | modrm (sib disp)     | bitwise xor r8->r8m                   |
| 31 xor.r>rm   | modrm (sib disp)     | bitwise xor r->rm                     |
| 32 xor.r8m>r8 | modrm (sib disp)     | bitwise xor r8m->r8                   |
| 33 xor.rm>r   | modrm (sib disp)     | bitwise xor rm->r                     |
| 34 xor.im8>al | im8                  | bitwise xor im8->al                   |
| 35 xor.im>a   | im                   | bitwise xor im->a                     |
| 36 null       |                      | Null Prefix in 64-bit Mode            |
| 37 invalid    |                      | Invalid Instruction in 64-Bit Mode    |
| 38 cmp.r8m-r8 | modrm (sib disp)     | compare by subtracting r8m-r8         |
| 39 cmp.rm-r   | modrm (sib disp)     | compare by subtracting rm-r           |
| 3A cmp.r8-r8m | modrm (sib disp)     | compare by subtracting r8-r8m         |
| 3B cmp.r-rm   | modrm (sib disp)     | compare by subtracting r-rm           |
| 3C cmp.al-im8 | im8                  | compare by subtracting al-im8         |
| 3D cmp.a-im   | im                   | compare by subtracting a-im           |
| 3E null       |                      | Null Prefix in 64-bit Mode            |
| 3F invalid    |                      | Invalid Instruction in 64-Bit Mode    |
| 40 rex        |                      | Access to new 8-bit registers         |
| 41 rex.b      |                      | Extension of ModR/M rm field          |
| 42 rex.x      |                      | Extension of SIB index field          |
| 43 rex.xb     |                      | Combination of REX.X and REX.B        |
| 44 rex.r      |                      | Extension of ModR/M r field           |
| 45 rex.rb     |                      | Combination of REX.R and REX.B        |
| 46 rex.rx     |                      | Combination of REX.R and REX.X        |
| 47 rex.rxb    |                      | Combination of REX.R, REX.X and REX.B |
| 48 rex.w      |                      | 64 Bit Operand Size                   |
| 49 rex.wb     |                      | Combination of REX.W and REX.B        |
| 4A rex.wx     |                      | Combination of REX.W and REX.X        |
| 4B rex.wxb    |                      | Combination of REX.W, REX.X and REX.B |
| 4C rex.wr     |                      | Combination of REX.X and REX.R        |
| 4D rex.wrb    |                      | Combination of REX.W, REX.R and REX.B |
| 4E rex.wrx    |                      | Combination of REX.W, REX.R and REX.X |
| 4F rex.wrxb   |                      | Combination of REX.W,R,X and B        |
| 50 push rax   |                      | push rax onto the stack               |
| 51 push rcx   |                      | push rcx onto the stack               |
| 52 push rdx   |                      | push rdx onto the stack               |
| 53 push rbx   |                      | push rbx onto the stack               |
| 54 push rsp   |                      | push rsp onto the stack               |
| 55 push rbp   |                      | push rbp onto the stack               |
| 56 push rsi   |                      | push rsi onto the stack               |
| 57 push rdi   |                      | push rdi onto the stack               |
| 58 pop rax    |                      | pop the stack into rax                |
| 59 pop rcx    |                      | pop the stack into rcx                |
| 5A pop rdx    |                      | pop the stack into rdx                |
| 5B pop rbx    |                      | pop the stack into rbx                |
| 5C pop rsp    |                      | pop the stack into rsp                |
| 5D pop rbp    |                      | pop the stack into rbp                |
| 5E pop rsi    |                      | pop the stack into rsi                |
| 5F pop rdi    |                      | pop the stack into rdi                |
| 60 invalid    |                      | Invalid Instruction in 64-Bit Mode    |
| 61 invalid    |                      | Invalid Instruction in 64-Bit Mode    |
| 62 invalid    |                      | Invalid Instruction in 64-Bit Mode    |
| 63 movsxd     |                      |                                       |
| 64 ovrd.fs    |                      | FS segment override prefix            |
| 65 ovrd.gs    |                      | GS segment override prefix            |
| 66 ovrd.op    |                      | operand-size override prefix          |
| 67 ovrd.addr  |                      | address-size override prefix          |
| 68 push.im    | im                   | push im                               |
| 69 imul       |                      |                                       |
| 6A push.im8   | im8                  | push im8                              |
| 6B imul       |                      |                                       |
| 6C insb       |                      |                                       |
| 6D ins        |                      |                                       |
| 6E outsb      |                      |                                       |
| 6F outs       |                      |                                       |
| 70 jo         | rel8                 | jmp if overlow flag                   |
| 71 jno        | rel8                 | jmp if not overlow flag               |
| 72 jb         | rel8                 | jmp if below                          |
| 72 jc         | rel8                 | jmp if carry flag                     |
| 73 jae        | rel8                 | jmp if above or equal                 |
| 73 jnc        | rel8                 | jmp if not carry flag                 |
| 74 je         | rel8                 | jmp if equal                          |
| 74 jz         | rel8                 | jmp if zero flag                      |
| 75 jne        | rel8                 | jmp if not equal                      |
| 75 jnz        | rel8                 | jmp if not zero flag                  |
| 76 jbe        | rel8                 | jmp if below or equal                 |
| 76 jna        | rel8                 | jmp if not above                      |
| 76 (jcz)      | rel8                 | jmp if carry or zero flag             |
| 77 ja         | rel8                 | jmp if above                          |
| 77 jnbe       | rel8                 | jmp if not below or equal             |
| 77 (jncz)     | rel8                 | jmp if not carry and not zero flag    |
| 78 js         | rel8                 | jmp if sign flag                      |
| 79 jns        | rel8                 | jmp if not sign flag                  |
| 7A jp         | rel8                 | jmp if parity flag                    |
| 7A jpe        | rel8                 | jmp if parity even                    |
| 7B jnp        | rel8                 | jmp if not parity flag                |
| 7B jpo        | rel8                 | jmp if parity odd                     |
| 7C jl         | rel8                 | jmp if less                           |
| 7C jnge       | rel8                 | jmp if not greater or equal           |
| 7C (jsno)     | rel8                 | jmp if sign flag is not overflow flag |
| 7D jnl        | rel8                 | jmp if not less                       |
| 7D jge        | rel8                 | jmp if greater or equal               |
| 7D (jso)      | rel8                 | jmp if sign flag is overflow flag     |
| 7E jle        | rel8                 | jmp if less or equal                  |
| 7E jng        | rel8                 | jmp if not greater                    |
| 7E (jzsno)    | rel8                 | jmp if Z or S flag is not O flag      |
| 7F jg         | rel8                 | jmp if greater                        |
| 7F jnle       | rel8                 | jmp if not less or equal              |
| 7F (jnzso)    | rel8                 | jmp if not Z and S flag is O flag     |
| 80 grp1im8rm8 | modrm (sib disp) im8 | op im8->r8m                           |
| 81 grp1im>rm  | modrm (sib disp) im  | op im->rm                             |
| 82 invalid    |                      | Invalid Instruction in 64-Bit Mode    |
| 83 grp1im8>rm | modrm (sib disp) im8 | op im8->rm                            |
| 84 test.r8r8m | modrm (sib disp)     | test by r8&r8m                        |
| 85 test.rrm   | modrm (sib disp)     | test by r&rm                          |
| 86 xchg.r8r8m | modrm (sib disp)     |                                       |
| 87 xchg.rrm   | modrm (sib disp)     |                                       |
| 88 mov.r8>rm8 | modrm (sib disp)     | mov r8->rm8                           |
| 89 mov.r>rm   | modrm (sib disp)     | mov r->rm                             |
| 8A mov.rm8>r8 | modrm (sib disp)     | mov rm8->r8                           |
| 8B mov.rm>r   | modrm (sib disp)     | mov rm->r                             |
| 8C mov.s>rm   | modrm (sib disp)     | mov s->rm                             |
| 8D lea.m>r    | modrm (sib disp)     | lea m->r                              |
| 8E mov.rm>s   | modrm (sib disp)     | mov rm->s                             |
| 8F pop>rm     | modrm (sib disp)     | pop from stack to rm                  |
| 90 nop        |                      | No Operation                          |
| 91 xchga.c    |                      | Exchange a and c register             |
| 92 xchga.d    |                      | Exchange a and d register             |
| 93 xchga.b    |                      | Exchange a and b register             |
| 94 xchga.sp   |                      | Exchange a and sp register            |
| 95 xchga.bp   |                      | Exchange a and bp register            |
| 96 xchga.si   |                      | Exchange a and si register            |
| 97 xchga.di   |                      | Exchange a and di register            |
| 98 conv.a>a   |                      | Sign extends a to double size of a    |
| 99 conv.a>da  |                      | Sign ext. a > d:a each same size as a |
| 9A invalid    |                      | Invalid Instruction in 64-Bit Mode    |
| 9B wait       |                      | Wait Prefix                           |
| 9C pushf      |                      | Push rFLAGS Register onto the Stack   |
| 9D popf       |                      | Pop Stack into rFLAGS Register        |
| 9E sahf       |                      | Store ah into flags                   |
| 9F lahf       |                      | Load flags into ah                    |
| A0 mov.off>al | off                  | mov off->al                           |
| A1 mov.off>a  | off                  | mov off->a                            |
| A2 mov.al>off | off                  | mov al->off                           |
| A3 mov.a>off  | off                  | mov a->off                            |
| A4 movsb      |                      | mov int8@mds:si->mes:di               |
| A5 movs       |                      | mov int@mds:si->mes:di                |
| A6 cmpsb      |                      | cmp int8@ds:si-int8@es:di             |
| A7 cmps       |                      | cmp int@ds:si-int@es:di               |
| A8 test.al    | im8                  | test al&im8                           |
| A9 test.a     | im                   | test a&im                             |
| AA stosb      |                      | al->mes:di                            |
| AB stos       |                      | a->mes:di                             |
| AC lodsb      |                      |                                       |
| AD lods       |                      |                                       |
| AE scasb      |                      |                                       |
| AF scas       |                      |                                       |
| B0 mov.im8>al | im8                  | mov im8->al                           |
| B1 mov.im8>cl | im8                  | mov im8->cl                           |
| B2 mov.im8>dl | im8                  | mov im8->dl                           |
| B3 mov.im8>bl | im8                  | mov im8->bl                           |
| B4 mov.im8>ah | im8                  | mov im8->ah                           |
| B5 mov.im8>ch | im8                  | mov im8->ch                           |
| B6 mov.im8>dh | im8                  | mov im8->dh                           |
| B7 mov.im8>bh | im8                  | mov im8->bh                           |
| B8 mov.im>a   | im                   | mov im->a                             |
| B8 mov.im>8   | im                   | rexb mov im->8                        |
| B9 mov.im>c   | im                   | mov im->c                             |
| B9 mov.im>9   | im                   | rexb mov im->9                        |
| BA mov.im>d   | im                   | mov im->d                             |
| BA mov.im>10  | im                   | rexb mov im->10                       |
| BB mov.im>b   | im                   | mov im->b                             |
| BC mov.im>sp  | im                   | mov im->sp                            |
| BD mov.im>bp  | im                   | mov im->bp                            |
| BE mov.im>si  | im                   | mov im->si                            |
| BF mov.im>di  | im                   | mov im->di                            |
| C0 grp2rm8im8 | modrm (sib disp) im8 | grp2op r8m im8 times                  |
| C1 grp2rmim8  | modrm (sib disp) im8 | grp2op rm im8 times                   |
| C2 retn       | im16                 | near ret from call and pop im16 bytes |
| C3 retn       |                      | near return from call                 |
| C4 invalid    |                      | Invalid Instruction in 64-Bit Mode    |
| C5 invalid    |                      | Invalid Instruction in 64-Bit Mode    |
| C6 mov.im8>rm | modrm (sib disp) im8 | mov im8->rm                           |
| C7 mov.im>rm  | modrm (sib disp) im  | mov im->rm                            |
| C8 enter      |                      |                                       |
| C9 leave      |                      |                                       |
| CA retf       | im16                 | far ret from call and pop im16 bytes  |
| CB retf       |                      | far return from call                  |
| CC int3       |                      | generate breakpoint trap              |
| CD int        | im8                  | call to interrupt procedure im8       |
| CE into       |                      | generate overflow trap if o flag is 1 |
| CF iret       |                      |                                       |
| D0 grp2r8m    | modrm (sib disp)     | grp2 op r8m 1 time                    |
| D1 grp2rm     | modrm (sib disp)     | shift grp op rm 1 time                |
| D2 grp2r8mcl  | modrm (sib disp)     | shift grp op r8m cl times             |
| D3 grp2rmcl   | modrm (sib disp)     | shift grp op rm cl times              |
| D4 invalid    |                      | Invalid Instruction in 64-Bit Mode    |
| D5 invalid    |                      | Invalid Instruction in 64-Bit Mode    |
| D6 invalid    |                      | Invalid Instruction in 64-Bit Mode    |
| D7 xlat       |                      | byte at ds:eax -> al                  |
| D8 fp0        | modrm                | floating point instructions           |
| D9 fp1        | modrm                | floating point instructions           |
| DA fp2        | modrm                | floating point instructions           |
| DB fp3        | modrm                | floating point instructions           |
| DC fp4        | modrm                | floating point instructions           |
| DD fp5        | modrm                | floating point instructions           |
| DE fp6        | modrm                | floating point instructions           |
| DF fp7        | modrm                | floating point instructions           |
| E0 loopnz     | rel8                 |                                       |
| E1 loopz      | rel8                 |                                       |
| E2 loop       | rel8                 |                                       |
| E3 jrcxz      | rel8                 | jump if rcx is 0                      |
| E4 in.im8>al  | im8                  | input byte from port addr im8 to al   |
| E5 in.im8>a   | im8                  | input byte from port addr im8 to a    |
| E6 out.al>im8 | im8                  | output byte from al to port addr im8  |
| E7 out.a>im8  | im8                  | output byte from a to port addr im8   |
| E8 call       | rel16/32             | call to rel16/32                      |
| E9 jmp32      | rel16/32             | jump tp rel16/32                      |
| EA invalid    |                      | Invalid Instruction in 64-Bit Mode    |
| EB jmp8       | rel8                 | jump to rel8                          |
| EC in.d>al    |                      | input byte from port addr d to al     |
| ED in.d>a     |                      | input byte from port addr d to a      |
| EE out.al>d   |                      | output byte from al to port addr d    |
| EF out.a>d    |                      | output byte from a to port addr d     |
| F0 esc        |                      | second operand escape                 |
| F1 int1       |                      | generate debug trap                   |
| F2 repnz      |                      | repeat string op while rcx=0          |
| F3 repz       |                      | repeat string op while not rcx=0      |
| F4 hlt        |                      | halt                                  |
| F5 cmc        |                      | complement carry flag                 |
| F6 grp3.r8m   | modrm (sib disp) im8 | group 3 instructions                  |
| F7 grp3.rm    | modrm (sib disp) im  | group 3 instructions                  |
| F8 clc        |                      | clear carry flag                      |
| F9 stc        |                      | set carry flag                        |
| FA cli        |                      | clear interrupt flag                  |
| FB sti        |                      | set interrupt flag                    |
| FC cld        |                      | clear direction flag                  |
| FD std        |                      | set direction flag                    |
| FE grp4       | modrm (sib disp)     | group 4 instructions                  |
| FF grp5       | modrm (sib disp)     | group 5 instructions                  |
