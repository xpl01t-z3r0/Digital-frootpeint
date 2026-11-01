
# Task 1

<img width="2164" height="1370" alt="image" src="https://github.com/user-attachments/assets/065ffc66-1fc7-4441-bbac-161da097c05e" />


```
┌──(root㉿kali)-[~/Desktop/tryhackme/osint]
└─# exiftool edited-house-1763031553617.jpg                                    
ExifTool Version Number         : 13.36
File Name                       : edited-house-1763031553617.jpg
Directory                       : .
File Size                       : 793 kB
File Modification Date/Time     : 2026:10:06 13:37:20-04:00
File Access Date/Time           : 2026:10:06 13:37:50-04:00
File Inode Change Date/Time     : 2026:10:06 13:37:27-04:00
File Permissions                : -rw-r--r--
File Type                       : JPEG
File Type Extension             : jpg
MIME Type                       : image/jpeg
Exif Byte Order                 : Big-endian (Motorola, MM)
GPS Latitude                    : 26 deg 12' 14.76"
GPS Longitude                   : 28 deg 2' 50.28"
JFIF Version                    : 1.01
Resolution Unit                 : None
X Resolution                    : 1
Y Resolution                    : 1
Image Width                     : 1306
Image Height                    : 837
Encoding Process                : Baseline DCT, Huffman coding
Bits Per Sample                 : 8
Color Components                : 3
Y Cb Cr Sub Sampling            : YCbCr4:4:4 (1 1)
Image Size                      : 1306x837
Megapixels                      : 1.1
GPS Position                    : 26 deg 12' 14.76", 28 deg 2' 50.28"

```

![[Pasted image 20261006235414.png]]



![[Pasted image 20261006235836.png]]

flag = THM{Johannesburg}

# Task 2

![[Pasted image 20261007001216.png]]

![[Pasted image 20261007001250.png]]

flag = THM{20160210224602}

# Task 3

 ![[landmark-1763035881792.jpg]]

![[Pasted image 20261007002653.png]]


![[Pasted image 20261007002557.png]]


![[Pasted image 20261007003023.png]]

flag = THM{General Post Office}

# Task 4

![[Pasted image 20261007010647.png]]

```
┌──(root㉿kali)-[~/Desktop/tryhackme/osint]
└─# exiftool internal-docs-1769695301727.odt 
ExifTool Version Number         : 13.36
File Name                       : internal-docs-1769695301727.odt
Directory                       : .
File Size                       : 15 kB
File Modification Date/Time     : 2026:10:06 15:00:29-04:00
File Access Date/Time           : 2026:10:06 15:02:48-04:00
File Inode Change Date/Time     : 2026:10:06 15:02:43-04:00
File Permissions                : -rw-r--r--
File Type                       : ODT
File Type Extension             : odt
MIME Type                       : application/vnd.oasis.opendocument.text
Creation-date                   : 2026:01:29 14:59:44
Description                     : Just remember Robin, don't publish this externally!
Language                        : en-US
Date                            : 2026:01:29 15:50:57.170215644
Editing-cycles                  : 4
Subject                         : Key Updates
Title                           : Internal Document
Editing-duration                : PT29M54S
Generator                       : LibreOffice/25.8.4.2$Linux_X86_64 LibreOffice_project/580$Build-2
Document-statistic Table-count  : 0
Document-statistic Image-count  : 0
Document-statistic Object-count : 0
Document-statistic Page-count   : 1
Document-statistic Paragraph-count: 7
Document-statistic Word-count   : 73
Document-statistic Character-count: 449
Document-statistic Non-whitespace-character-count: 380
User-defined Name               : Internal username
User-defined                    : markwilliams7243
Preview PNG                     : (Binary data 6403 bytes, use -b option to extract)

```

![[Pasted image 20261007010938.png]]

![[Pasted image 20261007010957.png]]

flag = THM{Y0u_f0und_7h3_fin4l_fl4g!}

