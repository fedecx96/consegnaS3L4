L'esperimento ci fa notare come con BurpSuite sia possibile intercettare username e password del pannello di controllo di DVWA.

Una volta inserite username e password nel form di login di DVWA, possiamo leggere in chiaro user e password inserite nel form, dato che la pagina non utilizza HTTPS ma HTTP.

Sempre su BurpSuite, possiamo modificare user e password prima che i dati vengano elaborati dal sito.

Alterando user e password, ovviamente, il login fallirà.

Nota: per modificare il file php.ini e cambiare l'impostazione allow_url_include, ho dovuto aprire il file da terminale come root con il comando 'sudo mousepad php.ini' (mousepad è l'editor di file di testo). 
Se si apre il file senza permessi di root, non si potrà salvare il file in quanto è in sola lettura.
