### apGDrivePlugin

#### It is a plugin for [symfony 1.4] (http://symfony.com/legacy) working with Google Drive.

Plugin connects to Google Drive and scans a map of new files if they are detected they are converted to .pdf format and downloaded to the local machine (if needed, converted files can be 
stored on Google Drive in separate folder)

#### Main components 

| Component type                    |  Description                                  |
|-----------------------------------|:----------------------------------------------|
| Config file path                  |   config/gdrive.yml                           |
| Google API submodule library path |   plugin/apGdrivePlugin/lib/vendor/google-api |
| File name validate pattern        |   CR Pack Visi ([\w]+-[\d]+) ([\d]+) [\S ]+   |
| Plugin module name                |   ap_gdrive                                   |
| Processing task:action name       |   `gdrive:processing`                         |

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

configuration parameters description:  

|   Param name                |  Description        |
|-----------------------------|:--------------------|
|   `client_secret_code`      |     [Google application] (https://console.developers.google.com/project) OAuth credentials client secret    |
|   `client_id`               |     [Google application] (https://console.developers.google.com/project) OAuth credentials client id    |
|   `source_folder_name`      |     Google Drive folder tray where is sored files               |
|   `destination_folder_name` |     Google Drive folder tray where make a converted file copy   |
|   `local_store_reports`     |     Local folder tree for store converted files                 |



