.. _install-multiteam-embedded-database:


.. role:: custom-color-primary-bold
   :class: sd-text-primary sd-font-weight-bold

   
.. role:: custom-color-primary-link
   :class: sd-text-primary sd-text-decoration-line-underline
   

#############################################################################################################################################
Install SimpleELN :custom-color-primary-bold:`MultiTeam Edition` as Web Server with Embedded Database
#############################################################################################################################################

The SimpleELN **MultiTeam Edition** is preconfigured with an embedded database, ideal for testing purposes. For production usage, kindly refer to the instructions outlined in :ref:`Install SimpleELN MultiTeam Edition with an External Database <install-multiteam-external-database>` for integrating with external databases such as MySQL, SQL Server, or Oracle. Please adhere to the outlined steps below to test its functionalities:

1. Download the application zip file (SimpleELN-MultiTeam-Server-{platform}-{arch}-{version}.zip) for the target platform from the official website or a trusted source.
#. Rename the downloaded zip file to **simpleeln-multiteam.zip** for convenient identification.
#. Open a terminal window
    
    - On Windows, you can press :code:`Win + R` and type ``cmd`` to open a command prompt.
    - On macOS or Linux, you can open a terminal from the Applications menu or use the Spotlight search (\ |apple clover| + Space).
    
#. Navigate to the directory where the **simpleeln-multiteam.zip** file is extracted.
      
      .. code-block:: sh
        :linenos:
        
        # Navigate to the directory where the simpleeln-multiteam.zip file is located and extract the zip file.
        unzip simpleeln-multiteam.zip
        # Navigate to the directory where the simpleeln-multiteam.zip file has been extracted.
        cd simpleeln-multiteam
        
#. Modify the web server settings. (Create the application.properties file and place it in the 'config' folder if not exist)
      
    .. code-block:: cfg
       :caption: contents of the config/application.properties file 
       :linenos:
       
       # contents of the config/application.properties file
       # server.port=32780 #default
       server.port=32780
       
#. Run the application web server

    - For Windows:
      
      .. code-block:: sh
         :linenos:
         
         # run the script
         startserver.bat

    - For macOS or Linux:
      
      .. code-block:: sh
         :linenos:
         
         # Optional: modify the file permissions if necessary
         sudo chown -R $USER ..
         chmod a+x ./startserver.sh
         # run the script
         ./startserver.sh

#. Use a web browser to access the web server

    1. Start the web server.
    #. Open a web browser in the local or remote computer (such as Google Chrome, Mozilla Firefox, Microsoft Edge, etc.).
    #. Navigate to :custom-color-primary-link:`http://<host_ip>:<port>`, making sure to replace <host_ip> with the IP address of your server host machine and <port> with the designated port number. For example, replace the <port> with the server.port number specified in the **application.properties** file: 32780
    #. If the connection is successful, you will be able to access the SimpleELN interface, similar to the following screenshot. 
        
        .. image:: ../images/localhost_cmdline-screenshot-homepage.png
            :align: center
            :width: 80%
            :class: sd-mb-4
            :alt: SimpleELN Homepage
            

.. |apple clover|  unicode:: U+2318 .. REGISTERED SIGN

