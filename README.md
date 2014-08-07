Role Name
========

Run Java fatjar as a service on your Ubuntu server.

Role Variables
--------------

- ```service_name```: service artifactId
- ```service_version```: service version
- ```service_port```: service port provided as PORT env variable
- ```dist_dir```: directory where to find fatJar, default `.`

Transfers file `{{ dist_dir }}/{{ service_name }}-{{ service_version }}.jar` to your server and runs it as supervisor service.


Example Playbook
-------------------------

See `test.yml`

You can run it in Vagrant. Just do:

```
vagrant up
```

and `curl http://localhost:8080/`

License
-------

**fatjar** role is published under [Apache License 2.0](http://www.apache.org/licenses/LICENSE-2.0).
