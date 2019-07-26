tomcat-install
===

Currently this role only download the require tomcat version for ACS 6.1.

Future projects will make this role reuseable for other versions of tomcat require by different ACS versions.

Role Variables:
---

Installation directory for tomcat
    tomcat_install_folder: /opt/tomcat

User that will own the tomcat_install_folder recursively
    tomcat_user: tomcat