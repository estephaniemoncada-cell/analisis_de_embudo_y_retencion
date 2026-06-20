# Título: Analisis de embudo y retención | Mercado Libre
# Objetivo: 
</p>
Usar SQL para mapear el embudo de conversión completo, identificar los principales puntos de fuga y evaluar la retención de usuarios por cohortes, por ultimo proponer mejoras accionables basadas en los datos.
 </p>

# Datos: 
</p>
Se utilizaron dos tablas disponibles:
* <p align="justify"> mercadolibre_funnel (user_id, session_id, event_name, event_time, country, device_category, platform, product_cat, price, currency, referral_source, event, date, year)
 * <p align="justify"> mercadolibre_retention (user_id, signup_date, signup_datetime, country, device_category, platform, day_after_signup, activity_date, active, prob_active)
 </p>
 El año analizado fue 2025, verificando la tasa de retención en D7, D14, D21 y D28 por pais </p>
 
# Proceso: 
* <p align="justify"> Exploración de eventos para confirmar la secuencia del embudo, despues de agruparon las conversiones del embudo por país, se calcularon las conversiones como % para detectar en que etapa del funnel se pierden más usuarios.</p>
 * <p align="justify"> Analicé las cohortes mensuales (YYY-MM), para calcular el % de usuarios activos al día 7, 14, 21 y 28 desde su registro
 
</p>
Las herramientas utilizadas fueron: SQL y Google Sheets </p>

# Entregable:

🔗 **Notebook del proyecto:**

[Ver análisis completo en Jupyter Notebook](https://github.com/estephaniemoncada-cell/analisis_de_embudo_y_retencion/blob/main/Proyecto%204_%20An%C3%A1lisis%20de%20embudo%20y%20retenci%C3%B3n%20para%20MercadoLibre%20-%20Resumen%20ejecutivo.pdf)

# Insights 
* <p align="justify">Analizamos el funnel general de compras de Mercado Libre por pais y por el periodo de tiempo entre el 01-01-2025 y el 08-31-2025, para saber la tasa de conversion entre cada etapa	"El 65.89% de los usuarios abandona el proceso entre seleccionar el producto y agregarlo al carrito. El pais con mayor porcentaje de abandono es Bolivia con un 70.97%, por otro lado Uruguay tiene el menor porcentaje de abandono con un 59.09%"
* <p align="justify">Se analizo la retencion de los usuarios por 7 dias, 14 dias, 21 dias y 28 dias los cuales se registaron entre el periodo del 01-01-2025 y el 06-01-2025, de igual forma se analizo la retencion por pais	"Se observa que la mayor retencion de usuarios se tiene entre el dia 7 y el dia 14 con un promedio de 32.57% de retencion de los usuarios.El pais con mayor retencion de usuarios al final del periodo es México y el pais con menor retencion de usuarios a lo largo del periodo estipulado es Bolivia"

# Recomendación:
* <p align="justify"> Mejoraria la etapa de seleccionar el producto, muchas veces se puede deber a que la fotorafia no es muy atractiva o no muestra los detalles necesarios. Tambien incentivaria a los usuarios a colocar opiniones sobre el producto, ya que esto da mayor confianza al futuro comprador		
