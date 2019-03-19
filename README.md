# Ansible role for Siege
Ansible role for Siege 4.0.2, an http/https regression testing and benchmarking utility.

## What's inside?
- Siege 4.0.2
- Default configuration:
    ```
    version:                        4.0.2
    verbose:                        true
    color:                          true
    quiet:                          false
    debug:                          false
    protocol:                       HTTP/1.1
    HTML parser:                    enabled
    get method:                     HEAD
    connection:                     close
    concurrent users:               25
    time to run:                    n/a
    repetitions:                    n/a
    socket timeout:                 30
    accept-encoding:                gzip;deflate
    delay:                          0.500 sec
    internet simulation:            false
    benchmark mode:                 false
    failures until abort:           1024
    named URL:                      none
    URLs file:                      /etc/siege/urls.txt
    thread limit:                   255
    logging:                        false
    log file:                       /home/vagrant/siege.log
    resource file:                  /home/vagrant/.siege/siege.conf
    timestamped output:             false
    comma separated output:         false
    allow redirects:                true
    allow zero byte data:           true
    allow chunked encoding:         true
    upload unique files:            true
    no-follow:
     - ad.doubleclick.net
     - pagead2.googlesyndication.com
     - ads.pubsqrd.com
     - ib.adnxs.com
    ```
## Usage examples


## Tested on
- Virtual Box 6.0.4, Vagrant 2.2.3, Ansible 2.7.6, ContOS 7 build 1812.01

## Installation
1. Navigate to Ansible's roles folder
2. Add the repo to git modules
    ```
    git submodule add https://github.com/budnerp/ansible_role_siege.git ansible_role_siege
    ```
3. Add the role to Ansible's playbook file
    ```    
    roles:
    [...]
        - ansible_role_siege
    [...]
    ```
   
## Other links
- Joe Dog Software Siege Manual [https://www.joedog.org/siege-manual/#]()
- Load testing with Siege [https://www.stephenrlang.com/2016/02/load-testing-with-siege/]()
- Speed testing your website with Siege: Part One [https://www.euperia.com/website-performance-2/speed-testing-your-website-with-siege-part-one/720]()
- Speed testing your website with Siege: Part two [https://www.euperia.com/website-performance-2/speed-testing-your-website-with-siege-part-two/771]()

## TO DO
-[ ] add dependencies

## License
Copyright (c) We Are Interactive under the MIT license.