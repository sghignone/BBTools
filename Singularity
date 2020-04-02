Bootstrap: docker
From: anapsix/alpine-java:latest


%labels
	author Stefano Ghignone
	maintainer sghignone
	name BBTools
	version v38.79 (released 2020-02-19) 
	bbmap 38.79
%post
	apk update && apk upgrade \
	&& apk add --no-cache sudo build-base wget

	#download and unpack bbtools from Sourgeforge
	wget -c https://downloads.sourceforge.net/project/bbmap/BBMap_38.79.tar.gz -P /opt/
	tar -xvzf /opt/BBMap_38.79.tar.gz -C /opt/
	rm /opt/BBMap_38.79.tar.gz

%environment
	export PATH=/opt/bbmap:$PATH
