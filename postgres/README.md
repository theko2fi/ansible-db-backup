## Restore

```bash
./azcopy copy "SAS" --from-to BlobPipe | gunzip | psql postgres
```
or 

```bash
./azcopy copy "SAS" "./backupfile.pgdump.gz" 
gunzip ./backupfile.pgdump.gz
psql -f ./backupfile.pgdump postgres
```
