# COMMANDO.IO CLI
The Commando.io command-line interface.

````
Usage:
    commando auth
    commando unauth
    commando servers [<server-id>]
    commando groups [<group-id>]
    commando recipes [<recipe-id>]
    commando execute <recipe-id> (--server=<server-id> | --groups=<group-id>,<group-id>,...)
    commando execution-queue <execution-queue-id>
    commando executions <execution-id>
    commando (version | --version)
    commando (help | --help)
````

Requirements
------------
*  bash *(with sed, grep, mktemp)*
*  curl

Installation
------------
````
cd "$HOME"
git clone https://github.com/commando/commando-cli.git
chmod +x commando-cli/commando
````

Optionally, you may create a symbolic link in `/usr/local/bin`:

````
ln -s "$HOME"/commando-cli/commando /usr/local/bin
````

Authentication
--------------

````
➜ ./commando auth
Enter your account alias: demo
Provide a valid API token secret key: %
````

Unauthentication
-----------------

````
➜ ./commando unauth
````

Run An Execution
-----------------

```
➜ ./commando execute rec_3Fc5q540e480b672d38Ig --groups=grp_2Xk7x540e481bcb9c775d
{
    "id": "55500796179db98dd24ac149",
    "url": "/v1/execution-queue/55500796179db98dd24ac149",
    "status": "QUEUED",
    "recipe": "rec_3Fc5q540e480b672d38Ig",
    "groups": [
        "grp_2Xk7x540e481bcb9c775d"
    ],
    "halt_on_stderr": false,
    "notes": null,
    "created": "2015-05-11T01:36:22Z",
    "created_by": {
        "id": "usr_9ukjE540e4870aace5VFr",
        "ip_address": "198.199.100.1",
        "geo_ip": "San Francisco, California, United States",
        "user_agent": "Commando-Cli/1.1 demo curl 7.37.1 (x86_64-apple-darwin14.0) libcurl/7.37.1 SecureTransport zlib/1.2.5"
    },
    "events": [
        {
            "status": "QUEUED",
            "date": "2015-05-11T01:36:22Z",
            "meta": {
                "queue": {
                    "ids": [
                        6147421832739411593
                    ],
                    "msg": "Messages put on queue.",
                    "id": 6147421832739411593
                }
            }
        }
    ]
}
```

Current Version
---------------

https://github.com/commando/commando-cli/blob/master/VERSION

Changelog
---------

https://github.com/commando/commando-cli/blob/master/CHANGELOG.md

Support, Bugs, And Feature Requests
-----------------------------------

Create issues here in GitHub (https://github.com/commando/commando-cli/issues).

License & Legal
---------------

Copyright 2017 NodeSocket, LLC.

Licensed under the Apache License, Version 2.0 (the "License"); you may not use this work except in compliance with the License. You may obtain a copy of the License in the LICENSE file, or at:

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the specific language governing permissions and limitations under the License.
