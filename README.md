# brewmaster-frontend

[![Build Status](https://travis-ci.org/brewmajsters/ansible-role-brewmaster-frontend.svg?branch=master)](https://travis-ci.org/brewmajsters/ansible-role-brewmaster-frontend)

Download and install brewmajsters/brewmaster-frontend with setup systemd service for nodejs frontend.

## Requirements

None

## Role Variables

    repo:
      dest: <str, absolute or relative path of github repo destination directory>
      version: <str, branch name or commit to clone>
    npm:
      run_script: <str, target npm script to run in systemd service (defaults to 'dev')>

## Dependencies

None

## Example Playbook

    - hosts: servers
      roles: ansible-role-brewmaster-frontend

## License

None

## Author Information

Tomas Bellus
