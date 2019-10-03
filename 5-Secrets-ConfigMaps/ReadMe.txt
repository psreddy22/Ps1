Secrets:
 	Consuming: Consuming Secrets either by ENV Variables or by mounting as secret volumes.	

ConfigMaps:
	Consuming: Consuming configmaps either by ENV Variables or by mounting as configmaps.

=========================================
Q1. Difference B/w Secrets & ConfigMaps ?
=========================================

Both Secrets & ConfigMaps are same except one property;

Secrets uses internally an encryption and decreption algoritham (base64)
Configmaps uses directly plain text as given in manifest file / in-put files.

