# ansible-role-copy_etc_issue

These are my base Vagrantfile files for

- CentOS 7
- CentOS 8
- Debian 10

These use the vagrant VMs produced by [Jeff Geerling](https://app.vagrantup.com/geerlingguy/).

If no vm names are specified vagrant will deploy one vm of each OS type.

## Network Configuration

The VM is configure with 2 network adapters.

- Adapter 1 is a nat interface.
- Adapter 2 is a host-only adapter. This is configured with a 192.168.60.x address.

## Shared Storage

The /vagrant filesystem is disabled. 

## License

MIT

## Author Information

Created in 2020 by Graham Lillico.
