Debian-PredictionIo
===================

PredictionIO is an open source machine learning server for software developers to create predictive features, such as personalization, recommendation and content discovery.

Requirements
------------

This role requires a debian compliant system such as ubuntu.

Role Variables
--------------

predictionio:
    version: "0.8.0"

Dependencies
------------

None

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: cowops.debian-predictionio, predictionio.version: "0.8.0" }

Tasks
-----

  - Install [PredictionIO](http://prediction.io/) server
  - Register service
Notes
-----
Once installed, do not forget to execute
`/usr/local/sbin/PredictionIO-{$VERSION}/bin/users`
in order to create admin and users accounts

License
-------

BSD
