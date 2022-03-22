# pfsense-filebeat
PFSENSE 2.6.0-RELEASE (amd64)
based on https://github.com/Noebas/pfsense-filebeat
just updated beat link


ELK_PfSense Run from command line to install:
curl --create-dirs -o /root/scripts/install.sh https://raw.githubusercontent.com/Silureth/pfsense-filebeat/main/install.sh

rename filebeats.yml_new in /usr/local/etc/beats/ -> filebeats.yml

Optional add menu item by add this to the service section of /cf/conf/config.xml
filebeat filebeat filebeat 

 	

><service>
	<name>filebeat</name>
	<rcfile>filebeat</rcfile>
	<executable>filebeat</executable>
	<description><![CDATA[Filebeat service]]></description>
</service>
