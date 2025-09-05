#SECCION DE COMENTARIOS

#Registro en el link: https://earthdatahub.destine.eu/getting-started
#Seccion:
#How to obtain an Earth Data Hub personal access token
#To obtain a personal access token you first need to register to the DestinE platform.
#Then you can go to *#Earth Data Hub account settings#* where you can find your default personal access tokens or create others.

#OJO: Usar correo de trabajo (profesional/institucional).
#El Gmail solo sería aceptado si no cuentas con uno institucional, pero no es lo recomendado.

#Email:jllamocca@senamhi.gob.pe
#user:jllamocca
#pass: Senamhi2025*


#Autentificacion
#Ingresar: https://earthdatahub.destine.eu/account-settings

#Tea asignan un ID
#Your user UID is 63203c1e-f1c5-451a-a7ec-48aec91b1ac0

#Cuota
#El límite mensual es de 500 000 solicitudes/mes

#En el mismo lugar
#My personal access tokens
#TOKEN: edh_pat_cfdba8b50c493e84dfc676f5f1efed1794dde11c40cd21237e54c21da72c2f9378c792defeb8e2ca4638ac478df26ab8



#En caso tengas un HPC
# Guardar tu token en el archivo .netrc
with open("$HOME/.netrc", "w") as f:
    f.write("machine data.earthdatahub.destine.eu\n")
    f.write("  password edh_pat_cfdba8b50c493e84dfc676f5f1efed1794dde11c40cd21237e54c21da72c2f9378c792defeb8e2ca4638ac478df26ab8\n")

!chmod 600 $HOME/.netrc


#Se va a Catalogos para el elegir la base de datos: https://earthdatahub.destine.eu/catalogue
