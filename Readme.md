# Lightweight HTTP server v jazyku C

Server preložíte pomocou pribaleného makefilu.

## Špecifikácia

Jedná sa o lightweight server, ktorý má minimum závislostí.
Server prijíma GET requesty na zadanom porte, ktorý sa píše do argumentu pri spustení programu.
Prijíma GET requesty: 
* /hostname (získa doménové meno)
* /cpu-name (získa informácie o procesore)
* /load     (získa aktuálnu záťaž procesora)

### Installation

A step by step guide that will tell you how to get the development environment up and running.

```
$ make
```

## Použitie

```
$ ./hinfosvc PORT
```

## Príklady použitia

```
$ make
$ ./hinfosvc 12345 &
```
```
$ curl http://localhost:12345/hostname
$ curl http://localhost:12345/cpu-name
$ curl http://localhost:12345/load
```

