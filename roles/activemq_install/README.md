activemq_install
=========
Downloads and installs activemq. Will create a user named activemq which should be used to run the activemq script.

ActiveMQ requires Java be installed and JAVA_HOME configured. 

This role will verify if Java is installed using yum. 
- If this is true, no further action is required and JAVA_HOME does not need to be configued.
- If this is false, java is download into the activemq_install_dir/java, extracted, and then the default activemq script updated with JAVA_HOME=activemq_install_dir/java


Role Variables
--------------

The follow variables are used to define the version of activemq downloaded:
activemq_major_version 
activemq_minor_version
activemq_hotfix_version

The following variable should not need to be modified as they a constructed using the above three version related variables:
activemq_version
activemq_file_name
activemq_download_url: "https://archive.apache.org/dist/activemq/{{ activemq_version }}/{{ activemq_file_name }}"

The location where activemq is installed:
activemq_install_dir

The username created and configured to own the installation
activemq_user

License
-------

Free
