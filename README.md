dh-dyndns
====

This script uses your dreamhost api key (assuming it has dns access), to
<br>either check, delete, list, or update your ip address for a given record
<br>in dreamhost. Makes dynamic dns possible with dreamhost except for the
<br>four hour time to live (ttl). If you need a faster dynamic dns service,
<br>try DynDNS.


Usage
----

<pre><code>Usage : dh-dyndns [option] &lt;value&gt; &lt;action&gt;
  Options:
    -h | --help   | help        shows this message
    -d | --domain | domain      domain which will be used (ex.: foo.bar.baz)
    -k | --key    | key         dreamhost api key
    -o | --option | option      actions to perform. listed below

  Actions:
    check           this checks whether existing ip is same as new.
    delete          this will delete record.
    exist           this will show you the existing ip address in record.
    list            shows you existing record according to domain.
    new             this will show you the new ip.
    update          this performs update of ip address according to whatever is
                    grabbed by check in script.

Sample Usage:
  update record: dh-dyndns -k ################ -d foo.bar.baz -o update

  check record : dh-dyndns -k ################ -d foo.bar.baz -o check

  update record: dh-dyndns -k ################ -d foo.bar.baz -o update

  help         : dh-dyndns -h</code></pre>

Requirements
----

- Wget (http://www.gnu.org/software/wget/)
- Bash (http://tiswww.case.edu/php/chet/bash/bashtop.html)

Todo
----


License and Author
----

Author:: Cesar Bodden (cesar@pissedoffadmins.com)

Copyright:: 2013, Pissedoffadmins.com

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program.  If not, see <http://www.gnu.org/licenses/>.
