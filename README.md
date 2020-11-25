# brewmaster-frontend

[![Build Status](https://travis-ci.org/brewmajsters/ansible-role-brewmaster-frontend.svg?branch=master)](https://travis-ci.org/brewmajsters/ansible-role-brewmaster-frontend)

Download and install brewmajsters/brewmaster-frontend with setup systemd service for nodejs frontend.

## Requirements

None

## Role Variables

    frontend_repo_dest: <str, absolute or relative path of github repo destination directory>
    frontend_repo_version: <str, branch name or commit to clone>
    frontend_repo_url: <str, url to public frontend repository>
    frontend_npm:
      run_script: <str, target npm script to run in systemd service (defaults to 'dev')>
    frontend_nodejs_archive_url: <str, nodejs binary archive url>
    frontend_nodejs_archive_root_path: <str, download path of nodejs archive>
    frontend_npm_users_home: <list, home dir paths of users to run npm and node binaries>
    frontend_environments: <dict, environment variables to be modified in '.env' file>
    frontend_listen_address: <str, listen IP address>

## Dependencies

None

## Example Playbook

    - hosts: servers
      roles: ansible-role-brewmaster-frontend

## License

None

## Author Information

Tomas Bellus
