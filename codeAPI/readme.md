# code API

> Attention : il n'y a pour le moment pas de véritable "API", ce qui est décrit ici sont l'usage de lien permettant de faire executer des actions par le serveur. En cas de besoins particulier, préférez me contacter (discord, mail, ...) plutôt que de traffiquer les morceaux de code proposer ci-dessous

## Partie publique

---

**fetch main data**  
`GET https://cta.loulou123546.fr/API/fetch`  

**entry :**  
*No entry*  

**result : JSON object**  
|key|description|example|
|:---:|:---:|:---:|
|inter|array of object, where object look like the example|`WIP`|
|vhc|array of object, where object look like the example|`WIP`|
|chat|array of string, where each string is a message|`"chat":["Hello Marc", "Hi, how are you ?", "Fine"]`| 

---

**Send a message**  
`POST https://cta.loulou123546.fr/API/newMSG`  

**entry : JSON object**  
|key|description|example|
|:---:|:---:|:---:|
|user|string with name of author|`"loulou123546"`|
|msg|string with msg content|`"Hey, I'm really happy today"`|

**result : JSON object**  
200 : `JSON :   { "ok" : true }`  
400 : `JSON :   { "error" : true }`  
