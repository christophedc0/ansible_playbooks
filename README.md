# ansible_playbooks

## plex.yml
This playbook runs plex_master.yml and afterwards play_slave.yml.

### purpose:
#### plex_master.yml
* Update plex
* Stop plex service
* Compress media library
* Copy library over scp to a backup plex instance
* Start plex service
* Clean up the mess we made

#### plex_slave.yml
* Update plex
* Stop plex service
* Save plex preferences
* Remove current media library
* Decompress media library
* Restore plex preferences
* Start plex service
* Clean up the mess we made
