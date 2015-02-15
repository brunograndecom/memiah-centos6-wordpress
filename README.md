# centos 6.5 wordpress 4.1 powered by ansible and vagrant

Builds httpd, mysql, php and wordpress on to an existing centos 6.5 vagrant box.
Httpd is configured with a self signed certificate.

## Requirements

* vagrant 1.7.x+ [vagrant 1.7.x+](https://www.vagrantup.com/ "Vagrant")
* a centos 6.5 vagrant box (named centos6.5) installed into vagrant
* ansible 1.8.x+

## Usage

Be sure to change the user and ssh related items in setup.yml at the bottom -
under 'Add user' and 'Add public key to authorized_keys' respectively.

In the project root type:

    vagrant up

Then in your favourite browser visit:

    http://192.168.50.51 (which will fail as port 80 is blocked)
    http://192.168.50.51 (which will send you to Wordpress setup)

If you like run:

    vagrant halt

to shutdown the machine.

Run:

    vagrant up

again to start it back up and see if everything is running as expected.

## License

The MIT License (MIT)

Copyright (c) [2015]

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
