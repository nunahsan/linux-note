### SSH Config
1. nano ~/.ssh/config

2. create new line using following syntax
```
		Host <connection_name>
		HostName <target_machine_ip_address>
		User <username>
		IdentityFile <private_key_file>
		Port <target_machine_port_number>
```

3. example :
```
		Host myserver
		HostName 123.123.123.123
		User root
		IdentityFile ~/.ssh/private.pem
		Port 22
```

4. save the file

5. ssh to target machine as below
`
ssh myserver
`

6. additional note :
private.pem file must be changed mode to 400
`
chmod 400 ~/.ssh/private.pem
`
