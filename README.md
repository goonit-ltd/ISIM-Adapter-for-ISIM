# ISIM-Adapter-for-ISIM
This adapter for IBM Security Identity Manager allows you to provision from an ISIM Supplier environment to an ISIM Consumer environment. This adapter works like any other and the Consumer Person entries will appear as ISIM accounts in the Supplier.

The adapter has been written using IBM Tivoli Directory Integrator 7.0 and testing performed using IBM Tivoli Directory 7.1.1 RMI service.

Adapter has been tested on ITIM 5.1 only at this time, may need small changes for ISIM 6.0.

The adapter uses LDAP for reconciliation of Person entries and connects to ITIM/ISIM using DSML2 over JNDI.

TDI ALs are in itimadapter.xml

To create the profile to import in ITIM/ISIM: -

	jar -cvf ITIMAdapterProfile.jar ITIMAdapterProfile/

Adapter implements standard Person object (inetOrgPerson). Update the schema.dsml file with any/all custom attributes required for custom Person objectclasses and add them to the eritimadapteraccount objectclass.







