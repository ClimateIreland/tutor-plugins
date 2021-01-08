Collection of plugin for `Tutor <https://docs.tutor.overhang.io>`_
==================================================================
Collection of plugins for `Tutor <https://docs.tutor.overhang.io>`_ to customise settings and environmentl variables.


Plugins List
------------

- default-course-mode-honor.yml  
- enable-account-retirement.yml  
- disable-course-browsable.yml   
- enable-course-prerequisites.yml  
- disable-course-discovery.yml   
- googleanalytics.yml  
- disable-discussion.yml  
- disable-wiki.yml  

Installation
------------

Once the plugin has been developed and save in plugins root folder ($ tutor plugins printroot), it should be listed in the plugins list with:: 

    tutor plugins list 

It if it has not already enabled, enable it with::

    tutor plugins enable myplugin 

Or disable it with::

    tutor plugins disable myplugin 

If config settings are being changed the settings need to be saved, you can make changes to the settings even on a running instance::

    tutor config save 

Restart your platform for config to take effect::

    tutor local quickstart 

If only lms settings have been changed instead of above can simply restart the LMS with::

    tutor local exec lms reload-gunicorn 
