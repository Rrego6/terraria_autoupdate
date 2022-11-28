# terraria_autoupdate

terrariad is a simple script to daemonize the terraria server. It handles starting, stopping, and updating the server. terrariad spawns a named tmux session

## usage
./terrariad start
./terrariad update
./terrariad stop
./terrariad warn

These commands should work well with a systemd service and timer to automatically start,stop, and update the terraria server.

## setup
- tmux,curl, and unzip must be available in the path
- kill any running terraria server, as terrariad will manage spawning it.
- when running for the first time, use ./terrariad update. This will download and then spawn the insance.

in terrariad:
- config_path must be set to a valid terraria config file. 
- terraria_dir_path must be set to a valid location



