# ================================================================
# SECCIÓN DE COMENTARIOS – EARTH DATA HUB (DestinE)
# ================================================================

# Registro en el portal:
#   https://earthdatahub.destine.eu/getting-started
#
# Sección de interés:
#   "How to obtain an Earth Data Hub personal access token"
#
# Pasos:
#   1. Registrarse en la plataforma DestinE.
#   2. Ingresar a *Earth Data Hub account settings*.
#   3. Allí encontrarás tu token personal por defecto o la opción
#      de generar nuevos.

# OJO:
#   - Usar correo de trabajo (profesional/institucional).
#   - Gmail solo en caso de no disponer de uno institucional (NO recomendado).

# Ejemplo de credenciales personales:
#   Email: jllamocca@senamhi.gob.pe
#   User : jllamocca
#   Pass : Senamhi2025*

# Autenticación:
#   Ingresar a: https://earthdatahub.destine.eu/account-settings
#   UID de usuario (ejemplo): 63203c1e-f1c5-451a-a7ec-48aec91b1ac0

# Cuota:
#   Límite mensual: 500,000 solicitudes

# Token personal (ejemplo):
#   edh_pat_cfdba8b50c493e84dfc676f5f1efed1794dde11c40cd21237e54c21da72c2f9378c792defeb8e2ca4638ac478df26ab8

# ================================================================
# AUTENTICACIÓN EN HPC
# Guardar el token en el archivo ~/.netrc
# ================================================================

with open("$HOME/.netrc", "w") as f:
    f.write("machine data.earthdatahub.destine.eu\n")
    f.write("  password edh_pat_cfdba8b50c493e84dfc676f5f1efed1794dde11c40cd21237e54c21da72c2f9378c792defeb8e2ca4638ac478df26ab8\n")

!chmod 600 $HOME/.netrc

# ================================================================
# CATÁLOGOS
# Selección de base de datos:
#   https://earthdatahub.destine.eu/catalogue
# ================================================================

