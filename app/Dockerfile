# lamp stack built with puppet

FROM braucher/php
MAINTAINER Jeff Braucher <jeff@braucher.net>

# You change /puppet/php.yaml and re-apply puppet like this
# RUN /puppet-apply

COPY ./app* /
ENTRYPOINT ["/app"]
CMD ["start"]

