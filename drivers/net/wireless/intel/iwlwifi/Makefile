# common
obj-$(CONFIG_IWLWIFI)	+= iwlwifi.o
iwlwifi-objs		+= iwl-io.o
iwlwifi-objs		+= iwl-drv.o
iwlwifi-objs		+= iwl-debug.o
iwlwifi-objs		+= iwl-notif-wait.o
iwlwifi-objs		+= iwl-eeprom-read.o iwl-eeprom-parse.o
iwlwifi-objs		+= iwl-phy-db.o iwl-nvm-parse.o
iwlwifi-objs		+= pcie/drv.o pcie/rx.o pcie/tx.o pcie/trans.o
iwlwifi-objs		+= pcie/ctxt-info.o pcie/trans-gen2.o
iwlwifi-$(CONFIG_IWLDVM) += iwl-1000.o iwl-2000.o iwl-5000.o iwl-6000.o
iwlwifi-$(CONFIG_IWLMVM) += iwl-7000.o iwl-8000.o iwl-9000.o iwl-a000.o
iwlwifi-objs		+= iwl-trans.o

iwlwifi-objs += $(iwlwifi-m)

iwlwifi-$(CONFIG_IWLWIFI_DEVICE_TRACING) += iwl-devtrace.o

ccflags-y += -I$(src)

obj-$(CONFIG_IWLDVM)	+= dvm/
obj-$(CONFIG_IWLMVM)	+= mvm/

CFLAGS_iwl-devtrace.o := -I$(src)
