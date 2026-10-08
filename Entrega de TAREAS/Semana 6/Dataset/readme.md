Link Dataset
https://archive.ics.uci.edu/dataset/222/bank+marketing

# Variables de entrada
## datos del cliente bancario
1 - age - edad (numérico) 

2 - job - trabajo: tipo de trabajo (categórico: "administrativo", "desconocido", "desempleado", "gerencia", "empleado doméstico", "emprendedor", "estudiante", "obrero", "autónomo", "jubilado", "técnico", "servicios") 

3 - marital - estado civil: estado civil (categórico: "casado", "divorciado", "soltero"; nota: "divorciado" significa divorciado o viudo) 

4 - education - educación (categórico: "desconocido", "secundario", "primario", "terciario") 

5 - default - impago: ¿tiene crédito en mora? (binario: "sí", "no") 

6 - balance - saldo: saldo anual promedio, en euros (numérico) 

7 - houding - vivienda: ¿tiene préstamo hipotecario? (binario: "sí", "no") 

8 - loan - préstamo: ¿tiene préstamo personal? (binario: "sí","no") 

## relacionado con el último contacto de la campaña actual 
9 - contact - contacto: tipo de comunicación del contacto (categórico: "desconocido","teléfono","celular") 

10 - day - día: último día del mes del contacto (numérico) 

11 - month - mes: último mes del año del contacto (categórico: "ene", "feb", "mar", ..., "nov", "dic") 

12 - duration - duración: duración del último contacto, en segundos (numérico) 

## otros atributos 
13 - campaign - campaña: número de contactos realizados durante esta campaña y para este cliente (numérico, incluye el último contacto) 

14 - pdays - días anteriores: número de días transcurridos desde el último contacto con el cliente en una campaña anterior (numérico, -1 significa que el cliente no fue contactado previamente) 

15 - previous - anterior: número de contactos realizados antes de esta campaña y para este cliente (numérico) 

16 - poutcome - resultado: resultado de la campaña de marketing anterior (categórico: "desconocido","otro","fracaso","éxito") 

# Variable de salida (objetivo deseado)
17 - y - tiene el cliente ¿Ha contratado un depósito a plazo fijo? (binario: "sí","no")
