# Analyse-Trafic-Reseau-Wireshark

Lors de ce TP, nous avons utilisé Wireshark pour analyser le trafic réseau généré par un navigateur web.

Dans le cas de HTTP, les paquets capturés montrent clairement les requêtes et les réponses échangées entre le client et le serveur. On peut lire directement les informations comme la méthode GET, l’URL demandée ou encore les champs Host et User-Agent. Cela montre que HTTP transmet les données en clair, sans chiffrement.

Dans le cas de HTTPS, les paquets capturés utilisent le protocole TLS. On observe des messages comme Client Hello et Server Hello, qui correspondent à la phase d’établissement de la connexion sécurisée. Ensuite, les données apparaissent comme Application Data, mais leur contenu est chiffré et donc illisible dans Wireshark.

Ainsi, ce TP montre la différence principale entre les deux protocoles :
    •    HTTP : communication non chiffrée, contenu lisible.
    •    HTTPS : communication chiffrée via TLS, contenu protégé et non lisible.

Cela explique pourquoi HTTPS est utilisé aujourd’hui pour sécuriser les communications sur Internet.