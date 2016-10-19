EPIC Ansible AWS role
=====================
This Ansible role manages the tags, snapshots and alarms in AWS.

Role Variables
--------------

* `aws_enable_statuscheck_alarm` (bool) enable/disable setting the alarm for the status check
* `aws_alarms_actions` (array) define the actions exectued when the alarm triggers
* `aws_tags` (dict) the tags to use when tagging the instance, volume, snapshots and eni
* `aws_enable_snapshots` (bool) enable/disable taking snapshots
* `aws_snapshots_nr_to_keep`: (int) the number of snapshots to keep in history

See [defaults/main.yml](defaults/main.yml) for the default values.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: enrise.ansible-aws-role }

License
-------

MIT
