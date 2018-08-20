# Downloading and updating databases

## ftp download of uniprot
`ftp ftp.uniprot.org`

You'll see:
```
Connected to ftp.uniprot.org (141.161.180.197).
220 Welcome to UniProt FTP service.
Name (ftp.uniprot.org:ewilbanks):
```

Enter username `anonymous` and just hit enter for password.

navigate to correct folder using `cd` and grab files you want using `get

```
ftp> cd /pub/databases/uniprot/current_release/knowledgebase/complete/
ftp> get README
ftp> get reldate.txt
ftp> get uniprot_trembl.fasta.gz

