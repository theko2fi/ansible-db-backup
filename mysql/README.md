## Restore

```bash
./azcopy copy "SAS" --from-to BlobPipe | gunzip | mysql -u USERNAME -p[pass]
```
or 

```bash
./azcopy copy "SAS" "./backupfile.sql.gz" 
gunzip ./backupfile.sql.gz
mysql -u root -p < ./backupfile.sql
```

