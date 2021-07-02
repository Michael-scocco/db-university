## DIPARTIMENTO

    - descrizione: TESTO; NON NULLABILE
    - sede: VARCHAR(128) ; NON NULLABILE
    - contatti: VARCHAR(128) ; NON NULLABILE
    - direttore: VARCHAR(64) ; NON NULLABILE
    - piano_annuale_ricerche: VARCHAR(128) ; PREDEFINITA(0)
    - contratti_convenzioni: VARCHAR(128) ; PREDEFINITA(0)

## CORSO DI LAUREA

    - tipologia_laurea: VARCHAR(128) ; NON NULLABILE
    - frequenza_minima_ore: TINYINT ; PREDEFINITA(0)
    - sede: VARCHAR(128) ; NON NULLABILE
    - numero_max_ammessioni: INT ; NON NULLABILE
    - materiale_didattico: TESTO ; NON NULLABILE

## CORSO

    - durata_corso: VARCHAR(128) ; NON NULLABILE
    - giorni_lezioni: VARCHAR(128) ; NON NULLABILE
    - programma_corso: TESTO ; NON NULLABILE
    - frequenza_minima_ore: TINYINT ; PREDEFINITA(0)
    - ore_totali_corso: TINYINT ; NON NULLABILE
    - media_voti_minima: TINYINT ; PREDEFINITA(0)

## INSEGNANTE

    - nome: VARCHAR(64) ; NON NULLABILE
    - cognome: VARCHAR(64) ; NON NULLABILE
    - indirizzo: VARCHAR ; NON NULLABILE
    - n_tel: VARCHAR(32) ; NULLABILE
    - data_nascita: DATA ; NON NULLABILE
    - luogo_nascita: VARCHAR(64) ; NON NULLABILE
    - cfr: VARCHAR(64) ; NON NULLABILE ; UNICO
    - genere: VARCHAR(16) ; NON NULLABILE
    - data_assunzione: DATA ; NON NULLABILE
    - turno: VARCHAR(128) ; NULLABILE
    - ruolo: VARCHAR(32) ; NON NULLABILE
    - stipendio: INT ; NON NULLABILE
    - tipo_contratto: VARCHAR(64) ; NON NULLABILE
    - e-mail: VARCHAR(128) ; NON NULLABILE ; UNICO
    - foto: VARCHAR ; NON NULLABILE
    - materia: VARCHAR(32) ; NON NULLABILE
    - corsi_attivi: TINYINT ; PREDEFINITA(0)

## APPELLO

    - id_studente: INT; NON NULLABILE
    - data_appello: DATA ; NON NULLABILE
    - materia_appello: VARCHAR(64) ; NON NULLABILE
    - voto_minimo: TINYINT ; NON NULLABILE
    - voto_massimo: TINYINT ; NON NULLABILE
    - tipologia_appello: VARCHAR(128) ; NON NULLABILE

## STUDENTE

    - id_studente: INT; NON NULLABILE
    - nome: VARCHAR(64) ; NON NULLABILE
    - cognome: VARCHAR(64) ; NON NULLABILE
    - indirizzo: VARCHAR ; NON NULLABILE
    - n_tel: VARCHAR(32) ; NULLABILE
    - data_nascita: DATA ; NON NULLABILE
    - luogo_nascita: VARCHAR(64) ; NON NULLABILE
    - cfr: VARCHAR(64) ; NON NULLABILE ; UNICO
    - genere: VARCHAR(16) ; NON NULLABILE
    - tipo_documento: VARCHAR(16) ; NON NULLABILE
    - n_documento: VARCHAR(32) ; NON NULLABILE ; UNICO
    - e-mail: VARCHAR(128) ; NON NULLABILE ; UNICO

## ESITO

    - totale_esami_sostenuti: TINYINT ; NON NULLABILE
    - totale_esami_non_sostenuti: TINYINT ; NON NULLABILE
    - totale_presenza_ore_corso: TINYINT ; NON NULLABILE
    - totale_assenze: TINYINT ; NON NULLABILE
    - media_voto: TINYINT ; NON NULLABILE
    - laurea_conseguita: VARCHAR(10) ; NON NULLABILE