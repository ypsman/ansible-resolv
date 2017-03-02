base Packages
=============
[![Build Status](https://travis-ci.org/ypsman/ansible-resolv.svg?branch=master)](https://travis-ci.org/ypsman/ansible-resolv)

config resolv.conf, DNS Nameserver and Domain.

Example Playbook
----------------

    - hosts: all
      roles:
        - role: ypsman.resolv
          resolv_dns_domain: 'mydomain.org'
          resolv_searchpath: ['mydomain.local', 'mydomain.org']
          resolv_dns_server:
          - 8.8.8.8
          - 8.8.4.4
