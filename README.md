# Sport Progression Systems

This is an *attempt* to provide a formal specification of progression systems for different sports.

## Motivation

Progression systems in sports are usually specified in textual documents, frequently in the language of the governing sport association.
The apparent drawback is that such documents are not machine-readable.
However, machine-readable specifications can be used to visualize and validate progression systems, perform automatic progression, and other purposes.
This project tries to provide a general specification that is able to cover a large variety of sports using a JSON schema.
While being machine-readable such schemas are still human-readable (to some extent).
This project also includes specifications of progression systems from some sports.

## Disclaimer

The progression systems provided in this project are unofficial, if not stated otherwise.

## Nomenclature

The nomenclature used in the JSON schema resembles the general scheme used for multisports events plus some custom terms:

* Competitors are the participants of a sports event, like individuals or teams.
* A range contains the progresion system for a number of competitors.
* A phase is a stage during a particular sport event.
  There might be a qualification and a racing phase, or rounds like heats leading to semifinals and finally to finals.
* Within a phase, units are held to rank competitors.
  Units are individual heats (one particular heat or semifinal) or matches.
  Competitors progress to these units from other units or phases following certain rules.
* A subunit might be used determine a ranking within a unit.

## Rules

The specification of what rule are referring to is intentionally left open.
The specification resembles a simple JSON representation of DML criteria ("WHERE" statements), but the interpretation of what is selected (see schema) may depend on the sport or the system that uses the progression system.
Nevertheless, a progression system following the provided JSON schema should try to be both machine- and human-readable.

## Technical Background

The JSON schema follows [JSON Schema Draft-07](https://json-schema.org/specification-links.html#draft-7) as it appears to be widely supported.

## Licence

This work is licensed under CC BY-SA 4.0. To view a copy of this license, visit http://creativecommons.org/licenses/by-sa/4.0/.
See AUTHORS file for a list of authors.
