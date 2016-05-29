# Home Lab

## Supermicro 5018D-FN4T
* Xeon D 8 core processor
* 128GB Memory
* 1u short depth case

### Thoughts
I've had this box since July 2015 and its been extremely stable.

* Low power consumption so can leave running 24x7
* Runs ESXi 6 without having to inject VIBs into the installer.
  * ESXi is booted from a USB stick
  * Support was finally added in ESXi for the 10Gb base-t ports. See: [VMware](http://www.vmware.com/resources/compatibility/detail.php?deviceCategory=io&productid=39968)
* IPMI / remote console works well. No need to plug in monitor / keyboard to set the box up.
* Supermicro makes you jump through hoops to licence the remote BIOS upgrade feature.
  * Remotely upgrading the board management firmware is supported out of the box and is painless.
  * Once licenced, remote upgrade of the BIOS is also painless.
    * To licence the BIOS update feature, I had to request a trial of the Supermicro Update Manager software and was provided with a key to enable the feature as part of the trial.
* I made a mistake ordering the 1u version as it's annoyingly loud for a home office environment. 
  * Attempting to swap the fan out for a quieter noctua model was a failure as the board overheated as soon as I did anything remotely processor intensive (like booting a VM).
  * I should have purchased the tower model 5028D-TN4T instead.
  * Will likely purchase the mini tower case and swap the board in the future for the sake of my hearing / sanity.
* Using a Samsung evo 850 for local storage with remote storage pool provided by my NAS.
* This thing runs Cisco VIRL like a champ. I have the 20 node licence and have dedicated 32GB and 6 cores to VIRL.