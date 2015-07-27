### apGDrivePlugin

#### It is a plugin for [symfony 1.4] (http://symfony.com/legacy) working with Google Drive.

Plugin connects to Google Drive and scans a map of new files if they are detected they are converted to .pdf format and downloaded to the local machine (if needed, converted files can be 
stored on Google Drive in separate folder)

#### Main components

###### Config file 
```yml
    client_secret_code: OWbNz5JbYwsrDjE9kR4tjAC-
    client_id: 747384071922-r5dn694mfkp5eu88i9m3kccgeh705uu8.apps.googleusercontent.com

    source_folder_name: App/AutoPlanning/Source # / - is dorectory delimiter
    destination_folder_name: App/AutoPlanning/Destination # / - is dorectory delimiter

    #root path from storage is: web/uploads
    local_store_reports: /AdWords/%customerId%/%year%/%month%/ #  %customerId% , %year% and %month% - it's a system tokens
```


