## Getting Started ##
---------------

To initialize your local repository using the OMNIROM trees to build MultiROM, use a command like this:

    repo init -u git://github.com/sub77/platform_manifest_twrp_omni.git -b mr-6.0
    
To initialize a shallow clone, which will save even more space, use a command like this:

    repo init --depth=1 -u git://github.com/sub77/platform_manifest_twrp_omni.git -b mr-6.0

Then to sync up:

    repo sync

Then to build:

     cd <source-dir>; . build/envsetup.sh; lunch omni_<device>-eng; mka recoveryimage; mka multirom_zip
