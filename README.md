# AutoritatCertificacio

Creació i gestió d'una Autoritat de Certificació amb OpenSSL

Creació de l'estructura de l'AC:

1. Crear estructura de carpetes AC Arrel i Ac Intermèdia, amb els seus fitxers de BD: ac_init
2. Crear certificat AC Arrel: ac_crear_acA
3. Crear certificat AC Intermèdia: ac_crear_acI
4. Crear arxiu amb cadena de certificació: ac_crear_cacert

Gestió de l'AC:

5. Crear certificat final d'usuari: ca_crear_usuari <fitxer_certificat>
6. Crear certificat final SSL: ca_crear_ssl <fitxer_certificat>
7. Revocar certificat final: ac_revocar_cert <fitxer_certificat>
8. Generació de la CRL: ac_crear_crl
9. Exportar fitxer PFX: ac_exportar_p12 <fitxer_certificat>

Altres utilitats:

· Mostrar un certificat qualsevol: ac_mostrar_cert <fitxer>
· Llistar certificats emesos: ac_llistar_certs
· Eliminar tota la informació de l'AC: ac_rm
