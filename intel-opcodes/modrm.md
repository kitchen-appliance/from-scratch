| ---------------------------------------------------------------------- |
|                                 modrm                                  |
| ---------------------------------------------------------------------- |
| rexw                | rexb                | bits                 | hex |
| ------------------- | ------------------- | -------------------- | --- |
| r[a]rm[ma]          | r[a]rm[m8]          | mod[00]r[000]rm[000] | 00  |
| r[a]rm[mc]          | r[a]rm[m9]          | mod[00]r[000]rm[001] | 01  |
| r[a]rm[md]          | r[a]rm[m10]         | mod[00]r[000]rm[010] | 02  |
| r[a]rm[mb]          | r[a]rm[m11]         | mod[00]r[000]rm[011] | 03  |
| r[a]rm[sib]         | r[a]rm[sib]         | mod[00]r[000]rm[100] | 04  |
| r[a]rm[disp32]      | r[a]rm[disp32]      | mod[00]r[000]rm[101] | 05  |
| r[a]rm[msi]         | r[a]rm[m14]         | mod[00]r[000]rm[110] | 06  |
| r[a]rm[mdi]         | r[a]rm[m15]         | mod[00]r[000]rm[111] | 07  |
| r[c]rm[ma]          | r[c]rm[m8]          | mod[00]r[001]rm[000] | 08  |
| r[c]rm[mc]          | r[c]rm[m9]          | mod[00]r[001]rm[001] | 09  |
| r[c]rm[md]          | r[c]rm[m10]         | mod[00]r[001]rm[010] | 0A  |
| r[c]rm[mb]          | r[c]rm[m11]         | mod[00]r[001]rm[011] | 0B  |
| r[c]rm[sib]         | r[c]rm[sib]         | mod[00]r[001]rm[100] | 0C  |
| r[c]rm[disp32]      | r[c]rm[disp32]      | mod[00]r[001]rm[101] | 0D  |
| r[c]rm[msi]         | r[c]rm[m14]         | mod[00]r[001]rm[110] | 0E  |
| r[c]rm[mdi]         | r[c]rm[m15]         | mod[00]r[001]rm[111] | 0F  |
| r[d]rm[ma]          | r[d]rm[m8]          | mod[00]r[010]rm[000] | 10  |
| r[d]rm[mc]          | r[d]rm[m9]          | mod[00]r[010]rm[001] | 11  |
| r[d]rm[md]          | r[d]rm[m10]         | mod[00]r[010]rm[010] | 12  |
| r[d]rm[mb]          | r[d]rm[m11]         | mod[00]r[010]rm[011] | 13  |
| r[d]rm[sib]         | r[d]rm[sib]         | mod[00]r[010]rm[100] | 14  |
| r[d]rm[disp32]      | r[d]rm[disp32]      | mod[00]r[010]rm[101] | 15  |
| r[d]rm[msi]         | r[d]rm[m14]         | mod[00]r[010]rm[110] | 16  |
| r[d]rm[mdi]         | r[d]rm[m15]         | mod[00]r[010]rm[111] | 17  |
| r[b]rm[ma]          | r[b]rm[m8]          | mod[00]r[011]rm[000] | 18  |
| r[b]rm[mc]          | r[b]rm[m9]          | mod[00]r[011]rm[001] | 19  |
| r[b]rm[md]          | r[b]rm[m10]         | mod[00]r[011]rm[010] | 1A  |
| r[b]rm[mb]          | r[b]rm[m11]         | mod[00]r[011]rm[011] | 1B  |
| r[b]rm[sib]         | r[b]rm[sib]         | mod[00]r[011]rm[100] | 1C  |
| r[b]rm[disp32]      | r[b]rm[disp32]      | mod[00]r[011]rm[101] | 1D  |
| r[b]rm[msi]         | r[b]rm[m14]         | mod[00]r[011]rm[110] | 1E  |
| r[b]rm[mdi]         | r[b]rm[m15]         | mod[00]r[011]rm[111] | 1F  |
| r[sp]rm[ma]         | r[sp]rm[m8]         | mod[00]r[100]rm[000] | 20  |
| r[sp]rm[mc]         | r[sp]rm[m9]         | mod[00]r[100]rm[001] | 21  |
| r[sp]rm[md]         | r[sp]rm[m10]        | mod[00]r[100]rm[010] | 22  |
| r[sp]rm[mb]         | r[sp]rm[m11]        | mod[00]r[100]rm[011] | 23  |
| r[sp]rm[sib]        | r[sp]rm[sib]        | mod[00]r[100]rm[100] | 24  |
| r[sp]rm[disp32]     | r[sp]rm[disp32]     | mod[00]r[100]rm[101] | 25  |
| r[sp]rm[msi]        | r[sp]rm[m14]        | mod[00]r[100]rm[110] | 26  |
| r[sp]rm[mdi]        | r[sp]rm[m15]        | mod[00]r[100]rm[111] | 27  |
| r[bp]rm[ma]         | r[bp]rm[m8]         | mod[00]r[101]rm[000] | 28  |
| r[bp]rm[mc]         | r[bp]rm[m9]         | mod[00]r[101]rm[001] | 29  |
| r[bp]rm[md]         | r[bp]rm[m10]        | mod[00]r[101]rm[010] | 2A  |
| r[bp]rm[mb]         | r[bp]rm[m11]        | mod[00]r[101]rm[011] | 2B  |
| r[bp]rm[sib]        | r[bp]rm[sib]        | mod[00]r[101]rm[100] | 2C  |
| r[bp]rm[disp32]     | r[bp]rm[disp32]     | mod[00]r[101]rm[101] | 2D  |
| r[bp]rm[msi]        | r[bp]rm[m14]        | mod[00]r[101]rm[110] | 2E  |
| r[bp]rm[mdi]        | r[bp]rm[m15]        | mod[00]r[101]rm[111] | 2F  |
| r[si]rm[ma]         | r[si]rm[m8]         | mod[00]r[110]rm[000] | 30  |
| r[si]rm[mc]         | r[si]rm[m9]         | mod[00]r[110]rm[001] | 31  |
| r[si]rm[md]         | r[si]rm[m10]        | mod[00]r[110]rm[010] | 32  |
| r[si]rm[mb]         | r[si]rm[m11]        | mod[00]r[110]rm[011] | 33  |
| r[si]rm[sib]        | r[si]rm[sib]        | mod[00]r[110]rm[100] | 34  |
| r[si]rm[disp32]     | r[si]rm[disp]       | mod[00]r[110]rm[101] | 35  |
| r[si]rm[msi]        | r[si]rm[m14]        | mod[00]r[110]rm[110] | 36  |
| r[si]rm[mdi]        | r[si]rm[m15]        | mod[00]r[110]rm[111] | 37  |
| r[di]rm[ma]         | r[di]rm[m8]         | mod[00]r[111]rm[000] | 38  |
| r[di]rm[mc]         | r[di]rm[m9]         | mod[00]r[111]rm[001] | 39  |
| r[di]rm[md]         | r[di]rm[m10]        | mod[00]r[111]rm[010] | 3A  |
| r[di]rm[mb]         | r[di]rm[m11]        | mod[00]r[111]rm[011] | 3B  |
| r[di]rm[sib]        | r[di]rm[sib]        | mod[00]r[111]rm[100] | 3C  |
| r[di]rm[disp32]     | r[di]rm[disp32]     | mod[00]r[111]rm[101] | 3D  |
| r[di]rm[msi]        | r[di]rm[m14]        | mod[00]r[111]rm[110] | 3E  |
| r[di]rm[mdi]        | r[di]rm[m15]        | mod[00]r[111]rm[111] | 3F  |
| r[a]rm[ma+disp8]    | r[a]rm[m8+disp8]    | mod[01]r[000]rm[000] | 40  |
| r[a]rm[mc+disp8]    | r[a]rm[m9+disp8]    | mod[01]r[000]rm[001] | 41  |
| r[a]rm[md+disp8]    | r[a]rm[m10+disp8]   | mod[01]r[000]rm[010] | 42  |
| r[a]rm[mb+disp8]    | r[a]rm[m11+disp8]   | mod[01]r[000]rm[011] | 43  |
| r[a]rm[sib+disp8]   | r[a]rm[sib+disp8]   | mod[01]r[000]rm[100] | 44  |
| r[a]rm[mbp+disp8]   | r[a]rm[m13+disp8]   | mod[01]r[000]rm[101] | 45  |
| r[a]rm[msi+disp8]   | r[a]rm[m14+disp8]   | mod[01]r[000]rm[110] | 46  |
| r[a]rm[mdi+disp8]   | r[a]rm[m15+disp8]   | mod[01]r[000]rm[111] | 47  |
| r[c]rm[ma+disp8]    | r[c]rm[m8+disp8]    | mod[01]r[001]rm[000] | 48  |
| r[c]rm[mc+disp8]    | r[c]rm[m9+disp8]    | mod[01]r[001]rm[001] | 49  |
| r[c]rm[md+disp8]    | r[c]rm[m10+disp8]   | mod[01]r[001]rm[010] | 4A  |
| r[c]rm[mb+disp8]    | r[c]rm[m11+disp8]   | mod[01]r[001]rm[011] | 4B  |
| r[c]rm[sib+disp8]   | r[c]rm[sib+disp8]   | mod[01]r[001]rm[100] | 4C  |
| r[c]rm[mbp+disp8]   | r[c]rm[m13+disp8]   | mod[01]r[001]rm[101] | 4D  |
| r[c]rm[msi+disp8]   | r[c]rm[m14+disp8]   | mod[01]r[001]rm[110] | 4E  |
| r[c]rm[mdi+disp8]   | r[c]rm[m15+disp8]   | mod[01]r[001]rm[111] | 4F  |
| r[d]rm[ma+disp8]    | r[d]rm[m8+disp8]    | mod[01]r[010]rm[000] | 50  |
| r[d]rm[mc+disp8]    | r[d]rm[m9+disp8]    | mod[01]r[010]rm[001] | 51  |
| r[d]rm[md+disp8]    | r[d]rm[m10+disp8]   | mod[01]r[010]rm[010] | 52  |
| r[d]rm[mb+disp8]    | r[d]rm[m11+disp8]   | mod[01]r[010]rm[011] | 53  |
| r[d]rm[sib+disp8]   | r[d]rm[sib+disp8]   | mod[01]r[010]rm[100] | 54  |
| r[d]rm[mbp+disp8]   | r[d]rm[m13+disp8]   | mod[01]r[010]rm[101] | 55  |
| r[d]rm[msi+disp8]   | r[d]rm[m14+disp8]   | mod[01]r[010]rm[110] | 56  |
| r[d]rm[mdi+disp8]   | r[d]rm[m15+disp8]   | mod[01]r[010]rm[111] | 57  |
| r[b]rm[ma+disp8]    | r[b]rm[m8+disp8]    | mod[01]r[011]rm[000] | 58  |
| r[b]rm[mc+disp8]    | r[b]rm[m9+disp8]    | mod[01]r[011]rm[001] | 59  |
| r[b]rm[md+disp8]    | r[b]rm[m10+disp8]   | mod[01]r[011]rm[010] | 5A  |
| r[b]rm[mb+disp8]    | r[b]rm[m11+disp8]   | mod[01]r[011]rm[011] | 5B  |
| r[b]rm[sib+disp8]   | r[b]rm[sib+disp8]   | mod[01]r[011]rm[100] | 5C  |
| r[b]rm[mbp+disp8]   | r[b]rm[m13+disp8]   | mod[01]r[011]rm[101] | 5D  |
| r[b]rm[msi+disp8]   | r[b]rm[m14+disp8]   | mod[01]r[011]rm[110] | 5E  |
| r[b]rm[mdi+disp8]   | r[b]rm[m15+disp8]   | mod[01]r[011]rm[111] | 5F  |
| r[sp]rm[ma+disp8]   | r[sp]rm[m8+disp8]   | mod[01]r[100]rm[000] | 60  |
| r[sp]rm[mc+disp8]   | r[sp]rm[m9+disp8]   | mod[01]r[100]rm[001] | 61  |
| r[sp]rm[md+disp8]   | r[sp]rm[m10+disp8]  | mod[01]r[100]rm[010] | 62  |
| r[sp]rm[mb+disp8]   | r[sp]rm[m11+disp8]  | mod[01]r[100]rm[011] | 63  |
| r[sp]rm[sib+disp8]  | r[sp]rm[sib+disp8]  | mod[01]r[100]rm[100] | 64  |
| r[sp]rm[mbp+disp8]  | r[sp]rm[m13+disp8]  | mod[01]r[100]rm[101] | 65  |
| r[sp]rm[msi+disp8]  | r[sp]rm[m14+disp8]  | mod[01]r[100]rm[110] | 66  |
| r[sp]rm[mdi+disp8]  | r[sp]rm[m15+disp8]  | mod[01]r[100]rm[111] | 67  |
| r[bp]rm[ma+disp8]   | r[bp]rm[m8+disp8]   | mod[01]r[101]rm[000] | 68  |
| r[bp]rm[mc+disp8]   | r[bp]rm[m9+disp8]   | mod[01]r[101]rm[001] | 69  |
| r[bp]rm[md+disp8]   | r[bp]rm[m10+disp8]  | mod[01]r[101]rm[010] | 6A  |
| r[bp]rm[mb+disp8]   | r[bp]rm[m11+disp8]  | mod[01]r[101]rm[011] | 6B  |
| r[bp]rm[sib+disp8]  | r[bp]rm[sib+disp8]  | mod[01]r[101]rm[100] | 6C  |
| r[bp]rm[mbp+disp8]  | r[bp]rm[m13+disp8]  | mod[01]r[101]rm[101] | 6D  |
| r[bp]rm[msi+disp8]  | r[bp]rm[m14+disp8]  | mod[01]r[101]rm[110] | 6E  |
| r[bp]rm[mdi+disp8]  | r[bp]rm[m15+disp8]  | mod[01]r[101]rm[111] | 6F  |
| r[si]rm[ma+disp8]   | r[si]rm[m8+disp32]  | mod[01]r[110]rm[000] | 70  |
| r[si]rm[mc+disp8]   | r[si]rm[m9+disp32]  | mod[01]r[110]rm[001] | 71  |
| r[si]rm[md+disp8]   | r[si]rm[m10+disp32] | mod[01]r[110]rm[010] | 72  |
| r[si]rm[mb+disp8]   | r[si]rm[m11+disp32] | mod[01]r[110]rm[011] | 73  |
| r[si]rm[sib+disp8]  | r[si]rm[sib+disp32] | mod[01]r[110]rm[100] | 74  |
| r[si]rm[mbp+disp8]  | r[si]rm[m13+disp32] | mod[01]r[110]rm[101] | 75  |
| r[si]rm[msi+disp8]  | r[si]rm[m14+disp32] | mod[01]r[110]rm[110] | 76  |
| r[si]rm[mdi+disp8]  | r[si]rm[m15+disp32] | mod[01]r[110]rm[111] | 77  |
| r[di]rm[ma+disp8]   | r[di]rm[m8+disp32]  | mod[01]r[111]rm[000] | 78  |
| r[di]rm[mc+disp8]   | r[di]rm[m9+disp32]  | mod[01]r[111]rm[001] | 79  |
| r[di]rm[md+disp8]   | r[di]rm[m10+disp32] | mod[01]r[111]rm[010] | 7A  |
| r[di]rm[mb+disp8]   | r[di]rm[m11+disp32] | mod[01]r[111]rm[011] | 7B  |
| r[di]rm[sib+disp8]  | r[di]rm[sib+disp32] | mod[01]r[111]rm[100] | 7C  |
| r[di]rm[mbp+disp8]  | r[di]rm[m13+disp32] | mod[01]r[111]rm[101] | 7D  |
| r[di]rm[msi+disp8]  | r[di]rm[m14+disp32] | mod[01]r[111]rm[110] | 7E  |
| r[di]rm[mdi+disp8]  | r[di]rm[m15+disp32] | mod[01]r[111]rm[111] | 7F  |
| r[a]rm[ma+disp32]   | r[a]rm[m8+disp32]   | mod[10]r[000]rm[000] | 80  |
| r[a]rm[mc+disp32]   | r[a]rm[m9+disp32]   | mod[10]r[000]rm[001] | 81  |
| r[a]rm[md+disp32]   | r[a]rm[m10+disp32]  | mod[10]r[000]rm[010] | 82  |
| r[a]rm[mb+disp32]   | r[a]rm[m11+disp32]  | mod[10]r[000]rm[011] | 83  |
| r[a]rm[sib+disp32]  | r[a]rm[sib+disp32]  | mod[10]r[000]rm[100] | 84  |
| r[a]rm[mbp+disp32]  | r[a]rm[m13+disp32]  | mod[10]r[000]rm[101] | 85  |
| r[a]rm[msi+disp32]  | r[a]rm[m14+disp32]  | mod[10]r[000]rm[110] | 86  |
| r[a]rm[mdi+disp32]  | r[a]rm[m15+disp32]  | mod[10]r[000]rm[111] | 87  |
| r[c]rm[ma+disp32]   | r[c]rm[m8+disp32]   | mod[10]r[001]rm[000] | 88  |
| r[c]rm[mc+disp32]   | r[c]rm[m9+disp32]   | mod[10]r[001]rm[001] | 89  |
| r[c]rm[md+disp32]   | r[c]rm[m10+disp32]  | mod[10]r[001]rm[010] | 8A  |
| r[c]rm[mb+disp32]   | r[c]rm[m11+disp32]  | mod[10]r[001]rm[011] | 8B  |
| r[c]rm[sib+disp32]  | r[c]rm[sib+disp32]  | mod[10]r[001]rm[100] | 8C  |
| r[c]rm[mbp+disp32]  | r[c]rm[m13+disp32]  | mod[10]r[001]rm[101] | 8D  |
| r[c]rm[msi+disp32]  | r[c]rm[m14+disp32]  | mod[10]r[001]rm[110] | 8E  |
| r[c]rm[mdi+disp32]  | r[c]rm[m15+disp32]  | mod[10]r[001]rm[111] | 8F  |
| r[d]rm[ma+disp32]   | r[d]rm[m8+disp32]   | mod[10]r[010]rm[000] | 90  |
| r[d]rm[mc+disp32]   | r[d]rm[m9+disp32]   | mod[10]r[010]rm[001] | 91  |
| r[d]rm[md+disp32]   | r[d]rm[m10+disp32]  | mod[10]r[010]rm[010] | 92  |
| r[d]rm[mb+disp32]   | r[d]rm[m11+disp32]  | mod[10]r[010]rm[011] | 93  |
| r[d]rm[sib+disp32]  | r[d]rm[sib+disp32]  | mod[10]r[010]rm[100] | 94  |
| r[d]rm[mbp+disp32]  | r[d]rm[m13+disp32]  | mod[10]r[010]rm[101] | 95  |
| r[d]rm[msi+disp32]  | r[d]rm[m14+disp32]  | mod[10]r[010]rm[110] | 96  |
| r[d]rm[mdi+disp32]  | r[d]rm[m15+disp32]  | mod[10]r[010]rm[111] | 97  |
| r[b]rm[ma+disp32]   | r[b]rm[m8+disp32]   | mod[10]r[011]rm[000] | 98  |
| r[b]rm[mc+disp32]   | r[b]rm[m9+disp32]   | mod[10]r[011]rm[001] | 99  |
| r[b]rm[md+disp32]   | r[b]rm[m10+disp32]  | mod[10]r[011]rm[010] | 9A  |
| r[b]rm[mb+disp32]   | r[b]rm[m11+disp32]  | mod[10]r[011]rm[011] | 9B  |
| r[b]rm[sib+disp32]  | r[b]rm[sib+disp32]  | mod[10]r[011]rm[100] | 9C  |
| r[b]rm[mbp+disp32]  | r[b]rm[m13+disp32]  | mod[10]r[011]rm[101] | 9D  |
| r[b]rm[msi+disp32]  | r[b]rm[m14+disp32]  | mod[10]r[011]rm[110] | 9E  |
| r[b]rm[mdi+disp32]  | r[b]rm[m15+disp32]  | mod[10]r[011]rm[111] | 9F  |
| r[sp]rm[ma+disp32]  | r[sp]rm[m8+disp32]  | mod[10]r[100]rm[000] | A0  |
| r[sp]rm[mc+disp32]  | r[sp]rm[m9+disp32]  | mod[10]r[100]rm[001] | A1  |
| r[sp]rm[md+disp32]  | r[sp]rm[m10+disp32] | mod[10]r[100]rm[010] | A2  |
| r[sp]rm[mb+disp32]  | r[sp]rm[m11+disp32] | mod[10]r[100]rm[011] | A3  |
| r[sp]rm[sib+disp32] | r[sp]rm[sib+disp32] | mod[10]r[100]rm[100] | A4  |
| r[sp]rm[mbp+disp32] | r[sp]rm[m13+disp32] | mod[10]r[100]rm[101] | A5  |
| r[sp]rm[msi+disp32] | r[sp]rm[m14+disp32] | mod[10]r[100]rm[110] | A6  |
| r[sp]rm[mdi+disp32] | r[sp]rm[m15+disp32] | mod[10]r[100]rm[111] | A7  |
| r[bp]rm[ma+disp32]  | r[bp]rm[m8+disp32]  | mod[10]r[101]rm[000] | A8  |
| r[bp]rm[mc+disp32]  | r[bp]rm[m9+disp32]  | mod[10]r[101]rm[001] | A9  |
| r[bp]rm[md+disp32]  | r[bp]rm[m10+disp32] | mod[10]r[101]rm[010] | AA  |
| r[bp]rm[mb+disp32]  | r[bp]rm[m11+disp32] | mod[10]r[101]rm[011] | AB  |
| r[bp]rm[sib+disp32] | r[bp]rm[sib+disp32] | mod[10]r[101]rm[100] | AC  |
| r[bp]rm[mbp+disp32] | r[bp]rm[m13+disp32] | mod[10]r[101]rm[101] | AD  |
| r[bp]rm[msi+disp32] | r[bp]rm[m14+disp32] | mod[10]r[101]rm[110] | AE  |
| r[bp]rm[mdi+disp32] | r[bp]rm[m15+disp32] | mod[10]r[101]rm[111] | AF  |
| r[si]rm[ma+disp32]  | r[si]rm[m8+disp32]  | mod[10]r[110]rm[000] | B0  |
| r[si]rm[mc+disp32]  | r[si]rm[m9+disp32]  | mod[10]r[110]rm[001] | B1  |
| r[si]rm[md+disp32]  | r[si]rm[m10+disp32] | mod[10]r[110]rm[010] | B2  |
| r[si]rm[mb+disp32]  | r[si]rm[m11+disp32] | mod[10]r[110]rm[011] | B3  |
| r[si]rm[sib+disp32] | r[si]rm[sib+disp32] | mod[10]r[110]rm[100] | B4  |
| r[si]rm[mbp+disp32] | r[si]rm[m13+disp32] | mod[10]r[110]rm[101] | B5  |
| r[si]rm[msi+disp32] | r[si]rm[m14+disp32] | mod[10]r[110]rm[110] | B6  |
| r[si]rm[mdi+disp32] | r[si]rm[m15+disp32] | mod[10]r[110]rm[111] | B7  |
| r[di]rm[ma+disp32]  | r[di]rm[m8+disp32]  | mod[10]r[111]rm[000] | B8  |
| r[di]rm[mc+disp32]  | r[di]rm[m9+disp32]  | mod[10]r[111]rm[001] | B9  |
| r[di]rm[md+disp32]  | r[di]rm[m10+disp32] | mod[10]r[111]rm[010] | BA  |
| r[di]rm[mb+disp32]  | r[di]rm[m11+disp32] | mod[10]r[111]rm[011] | BB  |
| r[di]rm[sib+disp32] | r[di]rm[sib+disp32] | mod[10]r[111]rm[100] | BC  |
| r[di]rm[mbp+disp32] | r[di]rm[m13+disp32] | mod[10]r[111]rm[101] | BD  |
| r[di]rm[msi+disp32] | r[di]rm[m14+disp32] | mod[10]r[111]rm[110] | BE  |
| r[di]rm[mdi+disp32] | r[di]rm[m15+disp32] | mod[10]r[111]rm[111] | BF  |
| r[a]rm[a]           | r[a]rm[8]           | mod[11]r[000]rm[000] | C0  |
| r[a]rm[c]           | r[a]rm[9]           | mod[11]r[000]rm[001] | C1  |
| r[a]rm[d]           | r[a]rm[10]          | mod[11]r[000]rm[010] | C2  |
| r[a]rm[b]           | r[a]rm[11]          | mod[11]r[000]rm[011] | C3  |
| r[a]rm[sp]          | r[a]rm[12]          | mod[11]r[000]rm[100] | C4  |
| r[a]rm[bp]          | r[a]rm[13]          | mod[11]r[000]rm[101] | C5  |
| r[a]rm[si]          | r[a]rm[14]          | mod[11]r[000]rm[110] | C6  |
| r[a]rm[di]          | r[a]rm[15]          | mod[11]r[000]rm[111] | C7  |
| r[c]rm[a]           | r[c]rm[8]           | mod[11]r[001]rm[000] | C8  |
| r[c]rm[c]           | r[c]rm[9]           | mod[11]r[001]rm[001] | C9  |
| r[c]rm[d]           | r[c]rm[10]          | mod[11]r[001]rm[010] | CA  |
| r[c]rm[b]           | r[c]rm[11]          | mod[11]r[001]rm[011] | CB  |
| r[c]rm[sp]          | r[c]rm[12]          | mod[11]r[001]rm[100] | CC  |
| r[c]rm[bp]          | r[c]rm[13]          | mod[11]r[001]rm[101] | CD  |
| r[c]rm[si]          | r[c]rm[14]          | mod[11]r[001]rm[110] | CE  |
| r[c]rm[di]          | r[c]rm[15]          | mod[11]r[001]rm[111] | CF  |
| r[d]rm[a]           | r[d]rm[8]           | mod[11]r[010]rm[000] | D0  |
| r[d]rm[c]           | r[d]rm[9]           | mod[11]r[010]rm[001] | D1  |
| r[d]rm[d]           | r[d]rm[10]          | mod[11]r[010]rm[010] | D2  |
| r[d]rm[b]           | r[d]rm[11]          | mod[11]r[010]rm[011] | D3  |
| r[d]rm[sp]          | r[d]rm[12]          | mod[11]r[010]rm[100] | D4  |
| r[d]rm[bp]          | r[d]rm[13]          | mod[11]r[010]rm[101] | D5  |
| r[d]rm[si]          | r[d]rm[14]          | mod[11]r[010]rm[110] | D6  |
| r[d]rm[di]          | r[d]rm[15]          | mod[11]r[010]rm[111] | D7  |
| r[b]rm[a]           | r[b]rm[8]           | mod[11]r[011]rm[000] | D8  |
| r[b]rm[c]           | r[b]rm[9]           | mod[11]r[011]rm[001] | D9  |
| r[b]rm[d]           | r[b]rm[10]          | mod[11]r[011]rm[010] | DA  |
| r[b]rm[b]           | r[b]rm[11]          | mod[11]r[011]rm[011] | DB  |
| r[b]rm[sp]          | r[b]rm[12]          | mod[11]r[011]rm[100] | DC  |
| r[b]rm[bp]          | r[b]rm[13]          | mod[11]r[011]rm[101] | DD  |
| r[b]rm[si]          | r[b]rm[14]          | mod[11]r[011]rm[110] | DE  |
| r[b]rm[di]          | r[b]rm[15]          | mod[11]r[011]rm[111] | DF  |
| r[sp]rm[a]          | r[sp]rm[8]          | mod[11]r[100]rm[000] | E0  |
| r[sp]rm[c]          | r[sp]rm[9]          | mod[11]r[100]rm[001] | E1  |
| r[sp]rm[d]          | r[sp]rm[10]         | mod[11]r[100]rm[010] | E2  |
| r[sp]rm[b]          | r[sp]rm[11]         | mod[11]r[100]rm[011] | E3  |
| r[sp]rm[sp]         | r[sp]rm[12]         | mod[11]r[100]rm[100] | E4  |
| r[sp]rm[bp]         | r[sp]rm[13]         | mod[11]r[100]rm[101] | E5  |
| r[sp]rm[si]         | r[sp]rm[14]         | mod[11]r[100]rm[110] | E6  |
| r[sp]rm[di]         | r[sp]rm[15]         | mod[11]r[100]rm[111] | E7  |
| r[bp]rm[a]          | r[bp]rm[8]          | mod[11]r[101]rm[000] | E8  |
| r[bp]rm[c]          | r[bp]rm[9]          | mod[11]r[101]rm[001] | E9  |
| r[bp]rm[d]          | r[bp]rm[10]         | mod[11]r[101]rm[010] | EA  |
| r[bp]rm[b]          | r[bp]rm[11]         | mod[11]r[101]rm[011] | EB  |
| r[bp]rm[sp]         | r[bp]rm[12]         | mod[11]r[101]rm[100] | EC  |
| r[bp]rm[bp]         | r[bp]rm[13]         | mod[11]r[101]rm[101] | ED  |
| r[bp]rm[si]         | r[bp]rm[14]         | mod[11]r[101]rm[110] | EE  |
| r[bp]rm[di]         | r[bp]rm[15]         | mod[11]r[101]rm[111] | EF  |
| r[si]rm[a]          | r[si]rm[8]          | mod[11]r[110]rm[000] | F0  |
| r[si]rm[c]          | r[si]rm[9]          | mod[11]r[110]rm[001] | F1  |
| r[si]rm[d]          | r[si]rm[10]         | mod[11]r[110]rm[010] | F2  |
| r[si]rm[b]          | r[si]rm[11]         | mod[11]r[110]rm[011] | F3  |
| r[si]rm[sp]         | r[si]rm[12]         | mod[11]r[110]rm[100] | F4  |
| r[si]rm[bp]         | r[si]rm[13]         | mod[11]r[110]rm[101] | F5  |
| r[si]rm[si]         | r[si]rm[14]         | mod[11]r[110]rm[110] | F6  |
| r[si]rm[di]         | r[si]rm[15]         | mod[11]r[110]rm[111] | F7  |
| r[di]rm[a]          | r[di]rm[8]          | mod[11]r[111]rm[000] | F8  |
| r[di]rm[c]          | r[di]rm[9]          | mod[11]r[111]rm[001] | F9  |
| r[di]rm[d]          | r[di]rm[10]         | mod[11]r[111]rm[010] | FA  |
| r[di]rm[b]          | r[di]rm[11]         | mod[11]r[111]rm[011] | FB  |
| r[di]rm[sp]         | r[di]rm[12]         | mod[11]r[111]rm[100] | FC  |
| r[di]rm[bp]         | r[di]rm[13]         | mod[11]r[111]rm[101] | FD  |
| r[di]rm[si]         | r[di]rm[14]         | mod[11]r[111]rm[110] | FE  |
| r[di]rm[di]         | r[di]rm[15]         | mod[11]r[111]rm[111] | FF  |