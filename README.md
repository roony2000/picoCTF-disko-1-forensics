# picoCTF-disko-1-forensics
Solution for the picoCTF Disko-1 challenge. Used gunzip, strings, and grep to extract a hidden flag from a compressed disk image. Includes original files, screenshots, and a clear step-by-step README.

# picoCTF 202X - Disko 1 Forensics Challenge

## Challenge Description
A disk image file (`disko-1.dd.gz`) was provided. The goal was to find a hidden flag inside the disk image using basic forensic tools.

---

## Tools Used
- Kali Linux
- `gunzip` to decompress the file
- `strings` to extract readable strings
- `grep` to filter for the flag

---

## Steps Taken

### 1. Decompress the disk image
```bash
gunzip disko-1.dd.gz

2. Extract readable strings and search for the flag

strings disko-1.dd > output.txt
grep "picoCTF" output.txt

3. Flag Found
picoCTF{1t5_ju5t_4_5tr1n9_be6031da}




![Decompress](https://github.com/roony2000/picoCTF-disko-1-forensics/raw/main/images/decompress.png)



![Flag Found](https://github.com/roony2000/picoCTF-disko-1-forensics/raw/main/images/flag_found.png)



Conclusion
This challenge demonstrates how to extract hidden information from a disk image using simple command-line tools, a fundamental forensic skill.


Files included
disko-1.dd.gz : Original compressed disk image

disko-1.dd : Decompressed disk image

output.txt : Extracted strings output

images/ : Screenshots showing the steps
