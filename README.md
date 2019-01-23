# Procedura

Si descrive il caso di un server CentOS 7.x

- Imposta utente e gruppo centos sulla folder Wildfly ``` sudo chown -R centos:centos /opt/wildfly-12.0.0.Final/ ```

- Crea ``` sudo vim /etc/systemd/system/multi-user.target.wants/wildfly.service ```

- Imposta i permessi ``` sudo chmod 664 /etc/systemd/system/multi-user.target.wants/wildfly.service ```

- Abilita il servizio ``` sudo systemctl enable wildfly ```

- Avvia il servizio ``` sudo systemctl start wildfly ```
