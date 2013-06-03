# To rebuild:
# lxc-docker build .
# lxc-docker tag <IMAGEID> nemaload/concat
# lxc-docker push nemaload/concat

FROM nemaload/base
MAINTAINER Petr Baudis "pasky@ucw.cz"

# INSERT would be natural here, but it's not supported in Docker yet
RUN sh -c '/bin/echo -e "#!/bin/sh\ncat \"\$1\" \"\$2\" >\"\$3\"" >/srv/computation/concat.sh'
RUN chmod +x /srv/computation/concat.sh
