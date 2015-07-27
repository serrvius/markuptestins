### apGDrivePlugin

#### It is a plugin for [symfony 1.4] (http://symfony.com/legacy) working with Google Drive.

Plugin connects to Google Drive and scans a map of new files if they are detected they are converted to .pdf format and downloaded to the local machine (if needed, converted files can be 
stored on Google Drive in separate folder)

#### Main components 

| Config file           |   config/gdrive.yml                           |
| Google API library    |   plugin/apGdrivePlugin/lib/vendor/google-api |


Config file: 

> config/gdrive.yml

```yml
    client_secret_code: <google application secret code>
    client_id: <google application client id>

    source_folder_name: folder-1/folder-1.1/folder-1.1.1 # / - is directory delimiter
    destination_folder_name: folder-2/folder-2.1/folder-2.1.1 # / - is directory delimiter

    #root path from storage is: web/uploads
    local_store_reports: /AdWords/%customerId%/%year%/%month%/ #  %customerId% , %year% and %month% - it's a system tokens
```




