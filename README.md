## sftp2blob (Azure)
- Fetches names of collections on sftp (Each directory in root is a collection).
- Creates a container in storage account (noted in config.js) for each collection if it doesn't already exist.
- Compares files in blobs with files in sftp collection.
- New files in sftp are downloaded to local / or mounted cloud and then uploaded to blob.

### Install
- Clone repo and cd into project
- Run `cp config-sample.js config.js; mkdir data`
- Add ssh and Azure blob storage credentials
- Run npm install
- Run node main.js
