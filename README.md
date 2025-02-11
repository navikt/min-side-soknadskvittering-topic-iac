# min-side-soknadskvittering-topic-iac

Repo med configurasjon for hvem som kan produsere til soknadskvittering-topic

## Topics og hensikt

- `aapen-soknadskvittering-v1` meld om hendelser for soknad som samles av appen tms-soknadskvittering.

## Hvordan få tilgang til topic?

**For skrivetilgang**

```
        - team: myTeam
          application: myApplication
          access: write 
```
**For lesetilgang**

```
        - team: myTeam
          application: myApplication
          access: read 
```

## Sletting av topic?
1. Ved å sette `removeDataWhenResourceIsDeleted` til `true` kan vi slette topic og all data som ligger på den.

    ```
      annotations:
            kafka.nais.io/removeDataWhenResourceIsDeleted: "true"
    ```
2. Deploy topic
3. Slett filen

# Henvendelser

Spørsmål knyttet til koden eller prosjektet kan rettes mot https://github.com/orgs/navikt/teams/min-side


## For NAV-ansatte

Interne henvendelser kan sendes via Slack i kanalen #team-personbruker.
