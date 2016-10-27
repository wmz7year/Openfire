FROM lwieske/java-8:server-jre-8u112-slim
MAINTAINER "wmz7year"

RUN mkdir /openfire

ADD 	/target/openfire/bin/ 			/openfire/bin
ADD 	/target/openfire/conf/ 			/openfire/conf
ADD 	/target/openfire/lib/ 			/openfire/lib
ADD 	/target/openfire/logs/ 			/openfire/logs
ADD 	/target/openfire/plugins/ 		/openfire/plugins
ADD 	/target/openfire/resources/ 	/openfire/resources

EXPOSE 5222/tcp 5223/tcp 5229/tcp 7070/tcp 7443/tcp 7777/tcp 9090/tcp 9091/tcp

ENTRYPOINT ["/openfire/bin/openfire.sh"]