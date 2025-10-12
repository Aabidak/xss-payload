##recon
find files/ -type f | while read file; do ./dec.sh "$file"; done



##key
1.mmls KH.img 
2.fls -r -o 40960 KH.img 
3.icat -o 40960 KH.img 18 >flag.txt 

##doube
1.grep -aob '%pdf ' filename.png
2.dd if=filename.png of=extracted.pdf bs=1 skip=(number found in above command)


##pixels

1.zsteg -a -v chall.png
2.zsteg -a -v chall.png |grep "CTF"

##doube

1.cpio -i < archive.cpio
2.
