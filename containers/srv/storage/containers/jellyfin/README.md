# Primo avvio del container
1. creare le cartelle `config` e `cache` 
   ```
   sudo mkdir {config,cache}
   ```
2. cambiargli il proprietario
   ```
   sudo chown utente:gruppo {config,cache}
   ```
   dove utente e gruppo vanno sostituiti con quelli dell'utente normale (si possono verificare digitando: `id $user` come utente normale)
3. testare la configurazione `docker-compose.yml` digitando:
   ```
   sudo docker-compose --env-file ../general_parameters.env config
   ```
4. se è tutto a posto si può lanciare il container con:
   ```
   sudo docker-compose --env-file ../general_parameters.env up -d
   ```
