.. The contents of this file may be included in multiple topics.
.. This file should not be changed in a way that hinders its ability to appear in multiple documentation sets.

|chef private| is now installed on your server, but is not configured for use. To configure it for a Standalone installation, simply run:

.. code-block:: bash

   $ private-chef-ctl reconfigure

This command may take several minutes to run, during which the output of the |chef| run that is configuring your new |chef private| installation is shown. When it is complete, you will see:

.. code-block:: bash

   Chef Server Reconfigured!

.. note:: |chef private| is composed of many different services, which work together to create a functioning system. One outcome is that it can take a few minutes for the system to finish starting up. One way to tell that the system is fully ready is to use the top command. You will notice high CPU utilization for several |ruby| processes while the system is starting up. When that utilization drops off, the system is ready.