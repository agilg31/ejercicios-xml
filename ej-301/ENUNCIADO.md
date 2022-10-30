# Ejercicio 301

Los siguientes documentos XML no son válidos. Modificarlos, lo mínimo posible, para que lo sean. La DTD no debe modificarse.

## Apartado a)

```xml
<?xml version="1.0" encoding="UTF-8"?>
<!DOCTYPE numeros [
    <!ELEMENT numeros (#PCDATA)>
]>
<numeros>
    <numero>25</numero>
</numeros>
```

## Apartado b)

```xml
<?xml version="1.0" encoding="UTF-8"?>
<!DOCTYPE letras [
    <!ELEMENT letras (letra)>
        <!ELEMENT letra (#PCDATA)>
]>
<letras>
    <letra>m</letra>
    <letra>uve doble</letra>
</letras>
```

## Apartado c)

```xml
<?xml version="1.0" encoding="UTF-8"?>
<!DOCTYPE colores [
    <!ELEMENT colores (color*)>
        <!ELEMENT color (#PCDATA)>
]>
<colores>
    <color>azul marino</color>
    negro
    <color>amarillo</color>
</colores>
```

## Apartado d)

```xml
<?xml version="1.0" encoding="UTF-8"?>
<!DOCTYPE flores [
    <!ELEMENT flores (flor+)>
        <!ELEMENT flor (#PCDATA)>
]>
<flores>
</flores>
```

## Apartado e)

```xml
<?xml version="1.0" encoding="UTF-8"?>
<!DOCTYPE animales [
    <!ELEMENT animales (animal*)>
        <!ELEMENT animal (#PCDATA)>
]>
<animales>
    <perro>Caniche</perro>
    <gato>Siamés</gato>
</animales>
```

## Apartado f)

```xml
<?xml version="1.0" encoding="UTF-8"?>
<!DOCTYPE escritores [
    <!ELEMENT escritores (escritor*)>
        <!ELEMENT escritor (nombre, nacimiento)>
            <!ELEMENT nombre (#PCDATA)>
            <!ELEMENT nacimiento (#PCDATA)>
]>
<escritores>
    <escritor>
        <nombre>Mario Vargas Llosa</nombre>
        <nacimiento>28 de marzo de 1936</nacimiento>
    </escritor>
    <escritor>
        <nacimiento>1 de abril de 1929</nacimiento>
        <nombre>Milan Kundera</nombre>
    </escritor>
</escritores>
```

## Apartado g)

```xml
<?xml version="1.0" encoding="UTF-8"?>
<!DOCTYPE musicos [
    <!ELEMENT musicos (musico*)>
        <!ELEMENT musico ((nombre|apodo), fechaNacimiento)>
            <!ELEMENT nombre (#PCDATA)>
            <!ELEMENT apodo (#PCDATA)>
            <!ELEMENT fechaNacimiento (#PCDATA)>
]>
<musicos>
    <musico>
        <nombre>Antonio Vivaldi</nombre>
        <apodo>El cura pelirrojillo</apodo>
        <fechaNacimiento>4 de marzo de 1678</fechaNacimiento>
    </musico>
    <musico>
        <nombre>Johann Sebastian Bach</nombre>
        <apodo>El viejo peluca</apodo>
        <fechaNacimiento>21 de marzo de 1685</fechaNacimiento>
    </musico>
</musicos>
```

## Apartado h)

```xml
<?xml version="1.0" encoding="UTF-8"?>
<!DOCTYPE agenda [
    <!ELEMENT agenda (contacto*)>
        <!ELEMENT contacto (nombre, telefonoFijo*, telefonoMovil+)>
            <!ELEMENT nombre (#PCDATA)>
            <!ELEMENT telefonoFijo (#PCDATA)>
            <!ELEMENT telefonoMovil (#PCDATA)>
]>
<agenda>
    <contacto>
        <nombre>Ayuntamiento</nombre>
        <telefonoFijo>010</telefonoFijo>
    </contacto>
    <contacto>
        <nombre>Emergencias</nombre>
        <telefonoFijo>112 (Unión Europea)</telefonoFijo>
        <telefonoMovil>Desconocido</telefonoMovil>
        <telefonoFijo>911 (Estados Unidos)</telefonoFijo>
    </contacto>
</agenda>
```

## Apartado i)

```xml
<?xml version="1.0" encoding="UTF-8"?>
<!DOCTYPE sistemaSolar [
    <!ELEMENT sistemaSolar (cuerpo*)>
        <!ELEMENT cuerpo (planeta|satelite|asteroide)>
            <!ELEMENT planeta (#PCDATA)>
            <!ELEMENT satelite (#PCDATA)>
            <!ELEMENT asteroide (#PCDATA)>
]>
<sistemaSolar>
    <cuerpo>
        <planeta>Tierra</planeta>
        <satelite>Luna</satelite>
    </cuerpo>
    <asteroide>Ceres</asteroide>
</sistemaSolar>
```
