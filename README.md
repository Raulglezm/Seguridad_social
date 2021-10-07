# Seguridad_social


![image](https://user-images.githubusercontent.com/91153605/136469429-153c3bc7-99cb-4a85-971b-a253861b6d47.png)



```bash
<?xml version="1.0" encoding="iso-8859-15" standalone="yes"?>

<!DOCTYPE afiliado [
<!ELEMENT afiliado (DNI_NIE, nombre, apellidos, fechadenacimiento, situacionlaboral, listadodebajas, prestacionesCobradas)>
<!ELEMENT DNI_NIE (#PCDATA)>
<!ELEMENT nombre (#PCDATA)>
<!ELEMENT apellidos (#PCDATA)>
<!ELEMENT fechaNacimiento(#PCDATA)>
<!ELEMENT situacionLaboral (en_paro, en_activo, jubilado, edad_no_laboral)>
     <!ELEMENT en_paro (#PCDATA)>
     <!ELEMENT en_activo (#PCDATA)>
     <!ELEMENT jubilado (#PCDATA)>
     <!ELEMENT edad_no_laboral (#PCDATA)>
<!ELEMENT listadoBajas (Causa, fecha_inicio,fecha_final)>
     <!ELEMENT Causa (#PCDATA)>
     <!ELEMENT fecha_inicio (#PCDATA)>
     <!ELEMENT fecha_final (#PCDATA)
<!ELEMENT prestacionesCobradas(catidad_percibida, fecha_inicio, fecha_final)>
     <!ELEMENT catidad(#PCDATA)>
     <!ELEMENT (#PCDATA)>
     <!ELEMENT (#PCDATA)>
]

<afiliado>

    <DNI_NIE>43384356A</DNI_NIE>
    <nombre>Juan</nombre>
    <apellidos>Luis Flores</apellidos>
    <fechaNacimiento>14/04/2005</fechaNacimiento>
    <situacionLaboral>edad_no_laboral</situacionLaboral>
    <listadoBajas> </listadoBajas>
    <prestacionesCobradas> </prestacionesCobradas>

</afiliado>

<afiliado>

    <DNI_NIE>42789356A</DNI_NIE>
    <nombre>Julian</nombre>
    <apellidos>Martín Perez</apellidos>
    <fechaNacimiento>10/10/1997</fechaNacimiento>
    <situacionLaboral>En_activo</situacionLaboral>
    <listadoBajas>
   	 <causa> Caida </causa>
   	 <fecha_inicio> 07/09/2021 </fecha_inicio>
   	 <fecha_final> 09/10/2021 </fecha_final>
     </listadoBajas>
    <prestacionesCobradas>
   	 <cantidad> 600 <cantidad/>
   	 <fecha_inicio> 07/09/2021 </fecha_inicio>
   	 <fecha_final> 09/10/2021 </fecha_final>
    </prestacionesCobradas>
</afiliado>
```
#
# Procedimiento: 
Lo primero fue dividir las distintas etiquetas y sus caracteristicas, para posteriormente crear el DTD y por último el perfil de lo afiliados, donde uno de ellos no tiene la edad apta para trabajar, y por ello los datos como <listadobajas> y <prestacionesCobradas> queda vacias. 

