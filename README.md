Inspired by GMER.
Windows driver including couple different techniques for file removal when regular operation isn't possible.

Description
===========
Details about each techniqu you can find in the following blog post:
https://translate.google.com/translate?sl=pl&tl=en&js=y&prev=_t&hl=en&ie=UTF-8&u=http%3A%2F%2Fwww.icewall.pl%2F%3Fp%3D349&edit-text=
(only automatic translation available, sorry , old post)

Techniques
===========
1. Setting FILE_SHARE_DELATE via:
	FILE_OBJECT : DeleteAccess and ImageSectionObject imporant for executable files.
2. Closing opened handles from all processes.
3. Attaching to our driver to the bottom of file system devices stack and hooking NTFS IRP handles. 
   Technique omits malware hooks made on higher level. Eficient method to remove e.g Bagle rootkit.
	

