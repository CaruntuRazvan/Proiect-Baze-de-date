#  Database project
Database for a professional football club

##  Database Diagram

The schema includes the following entities and their relationships:
- Stadion: Stores information about stadiums, including idStadion (PK), nume, locatie, and tip_iarba.
- Impresar: Contains details of agents, with idImpresar (PK), nume, prenume, telefon.
- Meci: Represents matches, with idMeci (PK), idStadion (FK), adversar, data_meci, and ora.
- Performanta_Jucator: Tracks player performances, with idMeci (FK), idJuator (FK), goluri, pase_decisive, cartonas_galben, cartonas_rosu, nota, postie_juator, and numar_titbu.
- Jucator: Holds player information, with idJuator (PK), idContract (FK), nume, prenume, varsta, nationalitate, inaltime, and telefon.
- Contract: Stores contract details, with idContract (PK), durata and salariu.
- Performanta_Arbitru: Records referee performances, with idMeci (FK) and idArbitru (FK).
- Arbitru: Contains referee details, with idArbitru (PK), nume, prenume, varsta, nationalitate, and rol.
- Performanta_Antrenament: Tracks training performance, with idJuator (FK) and idAntrenament (FK).
- Antrenament: Stores training session details, with idAntrenament (PK) and randament.
- Tip_Antrenament: Defines training types, with idTipAntrenament (PK), durata, and intensitate.
- Baza_Antrenament: Holds training facility information, with idBaza (PK), locatie, and tip_iarba.

![Diagram](./diagrama.png)
