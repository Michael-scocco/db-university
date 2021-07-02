## DIPARTIMENTO

    - descrizione: TESTO; NOT NULLABLE
    - sede: VARCHAR(128) ; NOT NULLABLE
    - contatti: VARCHAR(128) ; NOT NULLABLE
    - direttore: VARCHAR(64) ; NOT NULLABLE
    - piano_annuale_ricerche: VARCHAR(128) ; DEFAULT(0)
    - contratti_convenzioni: VARCHAR(128) ; DEFAULT(0)

## CORSO DI LAUREA

    - tipologia_laurea: VARCHAR(128) ; NOT NULLABLE
    - frequenza_minima_ore: TINYINT ; DEFAULT(0)
    - sede: VARCHAR(128) ; NOT NULLABLE
    - numero_max_ammessioni: INT ; NOT NULLABLE
    - materiale_didattico: TESTO ; NOT NULLABLE

## CORSO

    - durata_corso: VARCHAR(128) ; NOT NULLABLE
    - giorni_lezioni: VARCHAR(128) ; NOT NULLABLE
    - programma_corso: TESTO ; NOT NULLABLE
    - frequenza_minima_ore: TINYINT ; DEFAULT(0)
    - ore_totali_corso: TINYINT ; NOT NULLABLE
    - media_voti_minima: TINYINT ; DEFAULT(0)

## INSEGNANTE

    - nome: VARCHAR(64) ; NOT NULLABLE
    - cognome: VARCHAR(64) ; NOT NULLABLE
    - indirizzo: VARCHAR ; NOT NULLABLE
    - n_tel: VARCHAR(32) ; NOT NULLABLE
    - data_nascita: DATA ; NOT NULLABLE
    - luogo_nascita: VARCHAR(64) ; NOT NULLABLE
    - cfr: VARCHAR(64) ; NOT NULLABLE ; UNIQUE
    - genere: VARCHAR(16) ; NOT NULLABLE
    - data_assunzione: DATA ; NOT NULLABLE
    - turno: VARCHAR(128) ; NULLABLE
    - ruolo: VARCHAR(32) ; NOT NULLABLE
    - salario: INT ; NOT NULLABLE
    - tipo_contratto: VARCHAR(64) ; NOT NULLABLE
    - e-mail: VARCHAR(128) ; NOT NULLABLE ; UNIQUE
    - foto: VARCHAR ; NOT NULLABLE
    - materia: VARCHAR(32) ; NOT NULLABLE
    - corsi_attivi: TINYINT ; DEFAULT(0)

## APPELLO

    - id_studente: INT; NOT NULLABLE
    - data_appello: DATA ; NOT NULLABLE
    - materia_appello: VARCHAR(64) ; NOT NULLABLE
    - voto_minimo: TINYINT ; NOT NULLABLE
    - voto_massimo: TINYINT ; NOT NULLABLE
    - tipologia_appello: VARCHAR(128) ; NOT NULLABLE

## STUDENTE

    - id_studente: INT; NOT NULLABLE
    - nome: VARCHAR(64) ; NOT NULLABLE
    - cognome: VARCHAR(64) ; NOT NULLABLE
    - indirizzo: VARCHAR ; NOT NULLABLE
    - n_tel: VARCHAR(32) ; NULLABILE
    - data_nascita: DATA ; NOT NULLABLE
    - luogo_nascita: VARCHAR(64) ; NOT NULLABLE
    - cfr: VARCHAR(64) ; NOT NULLABLE ; UNIQUE
    - genere: VARCHAR(16) ; NOT NULLABLE
    - tipo_documento: VARCHAR(16) ; NOT NULLABLE
    - n_documento: VARCHAR(32) ; NOT NULLABLE ; UNIQUE
    - e-mail: VARCHAR(128) ; NOT NULLABLE ; UNIQUE

## ESITO

    - totale_esami_sostenuti: TINYINT ; NOT NULLABLE
    - totale_esami_non_sostenuti: TINYINT ; NOT NULLABLE
    - totale_presenza_ore_corso: TINYINT ; NOT NULLABLE
    - totale_assenze: TINYINT ; NOT NULLABLE
    - media_voto: TINYINT ; NOT NULLABLE
    - laurea_conseguita: VARCHAR(10) ; NOT NULLABLE