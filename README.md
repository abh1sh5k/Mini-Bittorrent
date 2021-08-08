# Mini-Bittorrent
### Requirement-
`sudo apt install openssl libssl-dev`

### Running the Project
* Run `make` in *tracker.cpp* directory and *client.cpp* directory.
* Run the following command to activate tracker server
 ``` 
 ./tracker <my_tracker_ip>:<my_tracker_port> <other_tracker_ip>:<other_tracker_port>  <seederlist_file>
 ```
* Run the following command to activate client server in client directory.
 ```
 ./client <CLIENT_IP>:<UPLOAD_PORT> <TRACKER_IP_1>:<TRACKER_PORT_1> <TRACKER_IP_2>:<TRACKER_PORT_2>
 ```
  
#### Functions on Client side
###### Share
* It share the file over the network and can be accessible through mtorrent file.
```
share <local_file_path> <filename>.<file_extension>.mtorrent
```
###### Download
* It downloads the file mentioned in mtorrent from available seeder.
```
 get <path_to_.mtorrent_file> <destination_path>
```
###### Downloads Status
* Check which files are Downloaded.
```
show_downloads
```
###### Remove user from Seederlist
```
remove <filename.mtorrent>
```
###### Closing the client
```
close
```
#### Summary
[![Torrent-diagram.jpg](https://i.postimg.cc/T1nYXCCh/Torrent-diagram.jpg)](https://postimg.cc/MfK87bk8)
