JOSÉ RECARGAS — VERIFICACIÓN DE FREE FIRE + FOTO

IMPORTANTE:
- La verificación NO funciona abriendo index.html directamente desde C:/...
- Debés usar la URL desplegada en Vercel, porque la página necesita /api/verificar.
- La API Key debe estar en Vercel como variable de entorno; no la pongas en index.html.

Vercel → Settings → Environment Variables:
FREEFIRE_API_KEY = TU_API_KEY

Opcional:
FREEFIRE_API_BASE = http://siambhau69.eu.cc/freefireinfo/bhau
FREEFIRE_REGIONS = SAC,BR,BD,IND,PK,SG,ID,TH,VN,TW,US,NA,ME,RU,CIS,EUROPE

Después de guardar la variable, hacé Redeploy.

La página:
- verifica el UID automáticamente;
- encuentra la región;
- muestra nombre y UID;
- muestra la imagen/banner de perfil cuando la API la entrega;
- habilita los productos solamente después de verificar.

Si al probar en Vercel aparece 403:
la API Key está rechazada o vencida.

Si aparece 504:
el servicio de Free Fire está tardando demasiado.

Si aparece 404:
el UID no fue encontrado en las regiones consultadas.
