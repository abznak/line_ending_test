# crlf test

This repositiory is for testing things that affect line endings.

```
$ hexdump -C linux.txt 
00000000  42 42 42 20 74 68 69 73  20 66 69 6c 65 20 41 41  |BBB this file AA|
00000010  41 0a 42 42 42 20 75 73  65 73 20 6c 69 6e 75 78  |A.BBB uses linux|
00000020  20 41 41 41 0a 42 42 42  20 6c 69 6e 65 20 65 6e  | AAA.BBB line en|
00000030  64 69 6e 67 73 20 41 41  41 0a                    |dings AAA.|
0000003a
$ hexdump -C mac.txt 
00000000  42 42 42 20 74 68 69 73  20 66 69 6c 65 20 41 41  |BBB this file AA|
00000010  41 0d 42 42 42 20 75 73  65 73 20 6c 69 6e 75 78  |A.BBB uses linux|
00000020  20 41 41 41 0d 42 42 42  20 6c 69 6e 65 20 65 6e  | AAA.BBB line en|
00000030  64 69 6e 67 73 20 41 41  41 0d                    |dings AAA.|
0000003a
$ hexdump -C dos.txt 
00000000  42 42 42 20 74 68 69 73  20 66 69 6c 65 20 41 41  |BBB this file AA|
00000010  41 0d 0a 42 42 42 20 75  73 65 73 20 64 6f 73 20  |A..BBB uses dos |
00000020  41 41 41 0d 0a 42 42 42  20 6c 69 6e 65 20 65 6e  |AAA..BBB line en|
00000030  64 69 6e 67 73 20 41 41  41 0d 0a                 |dings AAA..|
0000003b
```
