# unraid_arc_g2
compiled unraid kernel images to get intel arc dg2 working

this was compiled from https://github.com/thor2002ro/unraid_kernel (rc5)

for me dhcp was broken un this RC so you may have to set a static ip if that happens to you as well

changes:
bzmodules & bzimages:
CONFIG_INTEL_MEI=m 
CONFIG_INTEL_MEI_ME=m 
CONFIG_INTEL_MEI_TXE=m 
CONFIG_INTEL_MEI_GSC=m 
CONFIG_INTEL_MEI_HDCP=m 
CONFIG_INTEL_MEI_PXP=m 
CONFIG_INTEL_MEI_WDT=m

bzfirmware:
files from https://git.kernel.org/pub/scm/linux/kernel/git/firmware/linux-firmware.git/tree/i915
dg2_huc_gsc.bin
dg2_dmc_ver2_08.bin
