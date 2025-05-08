# 6_FROST_StaticData
Script that creates the json payload for the creation of static STA entities via API 

#### Generazione dei JSON statici per la creazione delle entità su FROST  

Gli script generano i file JSON statici, utilizzabili con **POSTMAN**, per la creazione delle entità di base su **FROST** dei vari pilot del progetto.  

#### Entità di base da creare (una tantum):  
- **Things**  
- **Locations**  
- **Feature of Interest (FOI)**  
- **Observed Properties**  
- **Datastreams**  

#### Procedura di esecuzione  
Gli script si basano su file **Excel**, quindi prima di eseguirli è necessario:  
1. **Avviare un'istanza di Jupyter Notebook.**  
2. **Eseguire il run di ogni cella dello script.**  
3. **Specificare nelle celle i percorsi corretti** dei file Excel compilati inizialmente da ogni pilot.  

#### Differenze tra i pilot  
- **Siviglia**: la geometria delle **location** è rappresentata da una **MultiLineString**.  
- **Vilnius**: la geometria può essere di tipo **Point** o **Polygon**, a seconda dei casi.  

#### Personalizzazioni e modifiche  
- È possibile **modificare i nomi dei file di output**.  
- Potrebbe essere necessario **aggiornare gli ID univoci**, ad esempio cambiando `"THI.FE.001"` in `"THI.ZG.001"`.  
- È importante **aggiornare i counter** per mantenere la coerenza dei dati.  
