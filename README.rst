
ElectrumX Banner Updater
------------------------

This script can be used to update the ElectrumX banner file to contain information about memory pool and fees.

ElectrumX server: 
    https://github.com/kyuupichan/electrumx
    
Bitcoin Core daemon:
    https://github.com/bitcoin/bitcoin


Getting Started
---------------

The first time you run this script your original banner file will be copied to ``${BANNER}.template``.

On each subsequent run ``${BANNER}.template`` will be used as the top portion of the new banner.

If you wish to change your banner you should edit ``${BANNER}.template``.


Edit update-electrumx-banner:
*****************************

- Adjust the ``BITCOIN_DATADIR`` environment to specify where to find your bitcoin data directory.

- Adjust the ``BITCOIN_CLI`` environment to specify where to find bitcoin-cli.

- Adjust the ``BANNER`` environment to specify the your electrumx banner file.


Scheduled Update:
*****************

Run ``crontab -e`` and add a cron job to update the banner every 2 minutes.

::

    */2 * * * *  /path/to/update-electrumx-banner


Versions
--------

This script is working with the following software versions::

 Operating System:   Ubuntu 16.04
 ElectrumX:          1.18.12
 Bitcoin Core:       0.17.0
 Bitcoin ABC:        0.18.4
 Bitcoin SV:         0.10.0
 
Live Example
------------

You can see an example here: 
    http://vps.hsmiths.com:49001/banner


=======================================================

**Samuel Smith**  shsmith@socal.rr.com   https://github.com/shsmith
