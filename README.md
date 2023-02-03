# Control-de-bombeo-LABVIEW

## Explicación - problemática

Se requiere sistema de bombeo de agua potable, el cual cuenta con tres bombas. Dos bombas son las principales y la tercera es de respaldo en caso de que una se dañe o se deshabilite por mantenimiento. Cada bomba tiene su pulsador de marcha y paro, así como también su selector de habilitado o deshabilitada. El sistema tendrá funcionamiento manual y automático comandado por la señal enviada por un selector. 
*	Modo manual: Cada bomba se activará presionando su respectivo pulsador de encendido, el cual deberá enclavarse (mantenerse en 1 aún después de haber sido soltada la botonera). Y de la misma forma, cada bomba tendrá su botón de apagado. Debido a que en el cálculo de carga no se consideraron las tres bombas encendidas al mismo tiempo, esto no debe ocurrir bajo ningún concepto, por lo que se debe garantizar que solo se enciendan máximo dos a la vez (puede realizarse con paridad par), y en caso de presionar el botón de encendido de una tercera bomba, esta no arrancará. 
*	Modo automático: En este modo se deben encender las bombas cuando la presión de la línea sea menor a 1.6 bar y como máximo 2.5 bar, lo cual garantiza el suministro de agua potable a los habitantes del sector con la misma presión. Las bombas primaria y secundaria serán aquellas que se enciendan cuando todo funciona normalmente, pero en caso de que una de ellas presente una falla o se encuentre deshabilitada se deberá enviar una señal de ALARMA(LED), mientras tanto se deberá utilizar la tercera bomba. 
En cualquier modo de operación, se puede presionar el pulsador de paro de emergencia, el cual deshabilitará las bombas inmediatamente mientras permanezca activo, al desactivarse, podrán funcionar normalmente. 
Cuando funcione en un modo de operación, no tomará en cuenta nada del proceso que sigue el otro modo. Considere que no se pueden deshabilitar dos bombas a la vez y que siempre se encenderán en pares.

## Panel de control (HMI):

![image](https://user-images.githubusercontent.com/69557269/216710432-8f8d5eb6-79d8-4ecc-9c7e-81cb66c6097e.png)

## Progamación modo automático:

![image](https://user-images.githubusercontent.com/69557269/216710618-4a3c993c-51b6-42bf-bf63-46aec458ba75.png)

## Progamación modo manual:

![image](https://user-images.githubusercontent.com/69557269/216710648-81f45646-054a-4dd2-8c70-7efbe5a44d6d.png)

## Autores ✒

* **Daniel Alvarado Pelaéz** 
* **Rios Andy Santiagoo** 

