## python
request like requests.get("localhost:1080") won't work as you need to include the protocol scheme, without http:// part, requests has no idea how to connect to the remote server. The correct way to request is like the example below:
	requests.get("http://localhost:1080")

## react and axios
	remember to pass http for domain name

## npm
### encountered when "npm install fabric-client" on mac
### xcode-select: error: tool 'xcodebuild' requires Xcode, but active developer directory '/Library/Developer/CommandLineTools' is a command line tools instance
	$ sudo xcode-select -s /Applications/Xcode.app/Contents/Developer

## docker
如果碰到docker启动马上退出的情况，很有可能是给docker分配的本地磁盘满了，使用docker volume prune就可以清除
