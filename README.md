# COMMANDO.IO CLI
The Commando.io command line interface.

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
    commando version
````

Installation
------------
````
git clone https://github.com/commando/commando-cli.git
chmod +x commando
````

Authentication
--------------

````
➜  ./commando auth
Enter your account alias: demo
Provide a valid API token secret key for demo.commando.io: %
````

Unauthentication
-----------------

````
➜  ./commando unauth
````

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

Copyright 2015 NodeSocket, LLC.

Licensed under the Apache License, Version 2.0 (the "License"); you may not use this work except in compliance with the License. You may obtain a copy of the License in the LICENSE file, or at:

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the specific language governing permissions and limitations under the License.
