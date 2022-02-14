# Lightweight HTTP server v jazyku C

Server preložíte pomocou pribaleného makefilu.

## Špecifikácia

Jedná sa o lightweight server, ktorý má minimum závislostí.
Server prijíma GET requesty na zadanom porte, ktorý sa píše do argumentu pri spustení programu.
Prijíma GET requesty: 
* /hostname (získa doménové meno)
* /cpu-name (získa informácie o procesore)
* /load     (získa aktuálnu záťaž procesora)

### Inštalácia

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
## Výstup
```
merlin.fit.vutbr.cz
Intel(R) Xeon(R) CPU E5-2640 0 @ 2.50GHz
65%
```
