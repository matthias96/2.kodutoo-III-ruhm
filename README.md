# 2. kodutoo (III r�hm)

## Kirjeldus

1. V�imalda oma lehel kasutajat luua ja kontrollida sisselogimist (kui on �ige tr�ki kasutaja id )
  * Abi saad 4. tunnit��st
1. **OLULINE! �RA POSTITA GITHUBI GREENY MYSQL PAROOLE.** Selleks toimi j�rgmiselt:
  * loo eraldi fail `config.php`. Lisa sinna kasutaja ja parool ning t�sta see enda koduse t�� kaustast �he taseme v�rra v�ljapoole
  ```PHP
  $servername = "localhost";
  $username = "username";
  $password = "password";
  ```
  * Andmebaasi nimi lisa aga kindlasti enda faili ja `require_once` k�suga k�si parool ja kasutajanimi `config.php` failist, siis saan kodust t��d lihtsamini kontrollida
  ```PHP
  // �henduse loomiseks kasuta
  require_once("../config.php");
  $database = "database";
  $mysqli = new mysqli($servername, $username, $password, $database);
  ```