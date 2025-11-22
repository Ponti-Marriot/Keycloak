# Cómo ejecutar Keycloak en Windows y Linux

Este documento explica cómo iniciar **Keycloak** en modo desarrollo
(**start-dev**) usando un puerto personalizado (ej.: `9000`) en
**Windows** y **Linux**.

------------------------------------------------------------------------

## Requisitos previos

1.  **Java 17 o superior** instalado\
2.  Ubicarse dentro del directorio principal de Keycloak

------------------------------------------------------------------------

# Linux

1.  Abre la terminal\
2.  Entra al directorio donde está Keycloak:

``` bash
cd ./keycloak-26.3.3
```

3.  Ejecuta Keycloak:

``` bash
./bin/kc.sh --verbose start-dev --http-port 9000
```

4.  Accede al panel de administración:

```{=html}
<!-- -->
```
    http://localhost:9000

------------------------------------------------------------------------

# Windows (PowerShell o CMD)

1.  Abre **PowerShell** o **CMD**
2.  Entra al directorio donde está Keycloak:

``` powershell
cd .\keycloak-26.3.3\
```

3.  Ejecuta Keycloak:

``` powershell
.\bin\kc.bat start-dev --http-port 9000 --verbose
```

4.  Accede al panel:

```{=html}
<!-- -->
```
    http://localhost:9000

------------------------------------------------------------------------

## Notas importantes

-   `start-dev` es **solo para desarrollo**, no para producción.\
-   `--http-port` cambia el puerto donde se ejecuta Keycloak.\
-   `--verbose` ayuda a ver más información útil para depuración.
