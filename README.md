# AED — Entrega Individual 3: `compactar` con PositionList
**Autor:** Luis Bravo  
**Curso:** 2017–2018 — Algoritmos y Estructuras de Datos (UPM)

Proyecto **Maven** con separación nítida de código y tests para la práctica de `compactar(PositionList<E>)`.

## Estructura
```
src/
  main/java/aed/individual3/
    OperacionCompactar.java   # tu implementación (sin modificar)
    MainCompactar.java        # main de ejemplo
  test/java/aed/individual3/
    Tester.java               # pruebas de la práctica (sin modificar)
    BuildSmokeTest.java       # test  JUnit
docs/guia.pdf                
```

## Uso
```bash
# 1) Copia positionList.jar a la carpeta libs/
# 2) Compilar y lanzar tests
mvn -q -DskipTests=false test

# Ejecutar un main de ejemplo
mvn -q -Dexec.mainClass=aed.individual3.MainCompactar exec:java
```

> Especificación resumida (ver *docs/guia.pdf*): implementar `compactar` que
> - devuelve **nueva** `PositionList<E>` con **una sola aparición** por cada **bloque de consecutivos iguales**,
> - acepta elementos `null`,
> - lanza `IllegalArgumentException` si `lista == null`,
> - la longitud de la salida no puede superar la número de elementos tras compactar.  
> (*Guía de la entrega, págs. 4–7*).

— *Luis Bravo*
