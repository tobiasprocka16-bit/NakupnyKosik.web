OBCHOD – nasadenie na Render

1. Rozbaľte tento ZIP.
2. Nahrajte obsah priečinka do nového GitHub repozitára.
3. Na Render zvoľte New + -> Web Service a pripojte tento repozitár.
4. Ak Render načíta render.yaml, potvrďte nastavenia. Inak nastavte:
   Build Command: pip install -r requirements.txt
   Start Command: uvicorn main2:app --host 0.0.0.0 --port $PORT
5. Vytvorte službu (Deploy).

Stránka obchodu: /
Administrácia skladu: /admin
Admin heslo podľa pôvodného kódu: trubicky

Poznámka: Sklad a košík sú momentálne uložené iba v pamäti procesu.
Po reštarte alebo novom nasadení sa resetujú. Pre trvalé dáta je potrebná
databáza (napr. PostgreSQL).
