# Original from envoyproject/envoy:examples/front-proxy/Dockerfile-frontenvoy
FROM envoyproxy/envoy

EXPOSE 5050 9901

ADD envoy-gateway.yml /etc/envoy-gateway.yaml
ADD ./start-gateway.sh /usr/local/bin/start-gateway.sh
RUN chmod u+x /usr/local/bin/start-gateway.sh

ENTRYPOINT /usr/local/bin/start-gateway.sh
