# Vagrantfile(s)

These are my base Vagrantfiles files for

- CentOS 7
- CentOS 8 (CentOS Linux 8 is End Of Life (EOL) as of December 31st 2021.)
- Debian 9
- Debian 10
- Ubuntu 18.04
- Ubuntu 20.04
- RockyLinux 8

These use the vagrant VMs produced by [Jeff Geerling](https://app.vagrantup.com/geerlingguy/).

If no vm names are specified vagrant will deploy one vm of each OS type.

## Network Configuration

The VM is configure with 2 network adapters.

- Adapter 1 is a nat interface.
- Adapter 2 is a host-only adapter. This is configured with a 192.168.60.x address.

## Shared Storage

The /vagrant filesystem is disabled.

## CentOS 8 Repositories

Due to CentOS Linux 8 going End Of Life (EOL) as of December 31st 2021, You will need to run the below commands on the VM to allow the yum command to work as expected.

- `cd /etc/yum.repos.d/`
- `sed -i 's/mirrorlist/#mirrorlist/g' /etc/yum.repos.d/CentOS-*`
- `sed -i 's|#baseurl=http://mirror.centos.org|baseurl=http://vault.centos.org|g' /etc/yum.repos.d/CentOS-*`
- `yum check-update`

## License

MIT

## Author Information

Created in 2020 by Graham Lillico.
