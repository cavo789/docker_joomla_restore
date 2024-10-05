# Restore a Joomla backup using Docker

Set of files for restoring a JPA Joomla archive using Docker. At the end, your site has been restored locally.

Please read the full article on [https://www.avonture.be/blog/docker-joomla-restore-jpa].

To download this repository, please run something like this:

```bash
mkdir /tmp/joomla_restore && cd $_
curl -LOJ --silent https://github.com/cavo789/docker_joomla_restore.git/archive/refs/tags/1.0.0.tar.gz
tar -xzvf docker_joomla_restore-1.0.0.tar.gz --strip-components 1 && rm -f docker_joomla_restore-1.0.0.tar.gz
```

Then, once downloaded:

```bash
make import
```

The Joomla site will be available on `http://127.0.0.1:8080\kickstart.php`.