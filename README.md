# brewmaster-frontend

[![Build Status](https://travis-ci.org/brewmajsters/ansible-role-brewmaster-frontend.svg?branch=master)](https://travis-ci.org/brewmajsters/ansible-role-brewmaster-frontend)

Download and install brewmajsters/brewmaster-frontend with setup systemd service for nodejs frontend.

## Requirements

None

## Role Variables

    frontend_repo:
      dest: <str, absolute or relative path of github repo destination directory>
      version: <str, branch name or commit to clone>
    frontend_npm:
      run_script: <str, target npm script to run in systemd service (defaults to 'dev')>
    frontend_nodejs_archive_url: <str, nodejs binary archive url>
    frontend_nodejs_archive_root_path: <str, download path of nodejs archive>
    frontend_npm_users: <list, users to run npm and node binaries>

## Dependencies

None

## Example Playbook

    - hosts: servers
      roles: ansible-role-brewmaster-frontend

## License

None

## Author Information

Tomas Bellus
