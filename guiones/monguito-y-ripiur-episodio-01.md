# MONGUITO Y RIPIUR — Episodio 01
## "La Patrulla Perdida en la Cordillera"

Formato: video narrado tipo "explorador" (estructura de Leo, El Explorador: descubrimiento → obstáculo → resolución → moraleja), adaptado a comedia militar familiar.
Duración objetivo: **25-28 minutos**
Personajes: **Monguito** (Fuerza Aérea Argentina) y **Ripiur** (Ejército Argentino)
Estilo visual: **Caricatura 2D**, basada en la ficha de referencia subida por el usuario.

---

## 0. NOTA DE PRODUCCIÓN (leer antes de generar)

Un video de 25 minutos no se hace con 200 clips de video generados — ningún modelo (Seedance 2.0 incluido) sostiene eso en costo/tiempo. La forma en que canales de este estilo llegan a 20-30 min es:

1. **Base = imágenes fijas en Higgsfield** (una por escena o por "beat" de guion), animadas en edición con paneos/zooms lentos (efecto Ken Burns) mientras suena la narración y los diálogos.
2. **Seedance 2.0 solo para los "momentos de acción"**: 3 a 5 clips animados de 8-10 segundos por escena, en los golpes de humor o movimiento fuerte (una caída, un salto, el cóndor pasando, la ventisca). El resto se cubre con la imagen fija + narración.
3. Esto da ritmo real de "documental-aventura" y reduce el trabajo a **~40 imágenes + ~15-18 videos cortos**, perfectamente viable.

Cada escena de abajo trae: guion (narración + diálogos), **1 prompt de imagen para Higgsfield** (toma clave de la escena) y **1-2 prompts de video para Seedance 2.0** (para los momentos de acción de esa escena).

### Prompt base de consistencia (pegar SIEMPRE al final de cada prompt de imagen)

```
estilo caricatura cómica argentina 2D, contorno grueso negro tipo cómic,
colores planos (cel-shading), proporciones exageradas, cabezas grandes,
narices redondas y prominentes, ojos pequeños y expresivos, sonrisas
amplias, iluminación plana de historieta, sin fotorrealismo, línea limpia
tipo ilustración editorial de humor gráfico
```

> Tip: en Higgsfield, subí la imagen de referencia que ya tenés (Monguito y Ripiur riendo en la montaña) como **elemento/referencia de personaje** ("reference element", no Soul, porque son 2 personajes en la misma toma) y usala en cada generación para mantener la cara, el uniforme y las proporciones idénticas escena a escena.

### Elemento de referencia ya creado (prueba de consistencia)

Se generó la ficha de personajes con `nano_banana_pro` y se guardó como **Reference Element** en Higgsfield:

- **Nombre:** `Monguito-y-Ripiur`
- **element_id:** `25eb2005-20af-4a4f-8436-1423db4c9ad8`
- **Ficha base:** https://d8j0ntlcm91z4.cloudfront.net/user_3GxEMiqnR2zWOQRKDIe0jXd0pRt/hf_20260727_135601_33a5bac9-fd61-43fb-b844-25ad5a88522c.png

Para reusar la identidad en cualquier prompt de imagen, insertá `<<<25eb2005-20af-4a4f-8436-1423db4c9ad8>>>` dentro del texto del prompt (Higgsfield lo reemplaza automáticamente por la referencia visual). Se probó con 2 escenas del episodio 1 y el resultado mantiene cara, uniforme y proporciones:

- Escena 8 (cóndor): https://d8j0ntlcm91z4.cloudfront.net/user_3GxEMiqnR2zWOQRKDIe0jXd0pRt/hf_20260727_135651_b2dea7a8-c071-4eea-b12a-6f84e410454a.png
- Escena 10 (rescate): https://d8j0ntlcm91z4.cloudfront.net/user_3GxEMiqnR2zWOQRKDIe0jXd0pRt/hf_20260727_135653_f066ec6f-205a-4b1d-a0b1-c94d0dd815c3.png

Modelo usado: `nano_banana_pro` (resuelve internamente a `nano_banana_2`), 2 créditos por imagen a resolución 1k.

---

## 1. FICHA DE PERSONAJES

### MONGUITO — Fuerza Aérea Argentina
- Calvo, cabeza redonda y brillante, nariz grande y roja/redondeada, cachetes rosados.
- Sonrisa enorme con dientes cuadrados, ojos casi cerrados cuando ríe.
- Uniforme de fajina camuflado, parche de bandera argentina en el hombro.
- Distintivo de Fuerza Aérea: gorra/boina gris-azulada con alitas bordadas, o auriculares de radio colgando del cuello; a veces lentes de aviador sobre la frente.
- Carga un bolso/rollo de dormir enorme atado a la mochila (siempre un poco desbordado, gag visual recurrente).
- Personalidad: optimista, torpe, hace bromas todo el tiempo, le tiene miedo a las alturas (irónico para Fuerza Aérea) pero es un genio con la radio y la tecnología.

### RIPIUR — Ejército Argentino
- Casco de combate M1 con red de camuflaje, cabeza más angosta, nariz grande también (familia visual con Monguito).
- Uniforme de fajina camuflado, parche de bandera argentina en el hombro.
- Físico más fornido, postura firme, pero igual de payaso que Monguito apenas se relaja.
- Personalidad: work-in-progress "duro y disciplinado" que se derrite de risa fácil; conoce la montaña como la palma de la mano, es el guía de la patrulla.

### Prompt de imagen — Ficha de personajes (para generar la referencia base en Higgsfield)

```
Dos soldados argentinos de caricatura 2D parados uno al lado del otro,
de cuerpo entero, sobre fondo blanco liso para usar como ficha de
personaje (character sheet). A la izquierda "Monguito": calvo, nariz
grande y redonda, sonrisa enorme, uniforme de fajina camuflado del
Ejército Argentino con detalle de boina gris azulada de Fuerza Aérea
Argentina con alitas bordadas, mochila con rollo de dormir desbordado,
pulgar arriba. A la derecha "Ripiur": casco M1 con red de camuflaje,
uniforme de fajina camuflado del Ejército Argentino, parche de bandera
argentina en el hombro, postura firme pero sonriendo, pulgar arriba.
Ambos con expresión de alegría exagerada tipo carcajada.
estilo caricatura cómica argentina 2D, contorno grueso negro tipo cómic,
colores planos (cel-shading), proporciones exageradas, cabezas grandes,
narices redondas y prominentes, ojos pequeños y expresivos, sonrisas
amplias, iluminación plana de historieta, sin fotorrealismo, línea limpia
tipo ilustración editorial de humor gráfico
```

---

## 2. GUION POR ESCENAS

---

### ESCENA 1 — Cold Open / Gancho (0:00–1:00)

**NARRADOR (voz en off, tono entusiasta tipo "explorador"):**
"¡Bienvenidos, exploradores! Hoy los vamos a llevar a una misión que nadie en la Cordillera de los Andes va a olvidar. ¿Están listos para conocer a la patrulla más... particular... de las Fuerzas Armadas Argentinas?"

*(Corte rápido: Monguito resbalando en la nieve, Ripiur atajándolo de la mochila justo antes de caer a un pozo de nieve. Los dos quedan colgando, muertos de risa.)*

**MONGUITO:** "¡Ripiur, esto no estaba en el plan de vuelo!"
**RIPIUR:** "¡Acá no hay plan de vuelo, Monguito, esto es TIERRA!"

*(Título del episodio en pantalla: "MONGUITO Y RIPIUR: La Patrulla Perdida en la Cordillera")*

**Prompt imagen (Higgsfield):**
```
Dos soldados de caricatura argentina colgando de un borde nevado,
uno sosteniendo al otro de la mochila, ambos riendo a carcajadas,
fondo de cordillera nevada con picos filosos, cielo celeste con nubes,
cámara en ángulo bajo dramático tipo toma de acción,
[+ prompt base de consistencia]
```

**Prompt video (Seedance 2.0), ~8s:**
```
Imagen a video. El soldado calvo (Monguito) resbala y cae hacia el
borde nevado agitando los brazos; el otro soldado (Ripiur) lo agarra
firme de la correa de la mochila justo a tiempo, tirón brusco hacia
arriba, nieve salpicando en cámara lenta al final, ambos quedan
riéndose colgados. Cámara: leve shake al inicio, estabiliza al final.
Loop de risa en bucle los últimos 2 segundos.
```

---

### ESCENA 2 — Presentación de la Base (1:00–3:30)

**NARRADOR:** "Todo empezó horas antes, en la Base Conjunta Cóndor Blanco, al pie de la Cordillera..."

*(Plano general de una base militar estilizada, banderas argentinas, hangar de Fuerza Aérea de un lado, carpas y vehículos del Ejército del otro.)*

**NARRADOR:** "Monguito llevaba tres años en Fuerza Aérea reparando radios... y evitando subirse a cualquier cosa más alta que una escalera."
**NARRADOR:** "Ripiur, en cambio, era el mejor guía de montaña del Ejército Argentino. El problema es que los dos NUNCA habían trabajado juntos."

*(Los dos se cruzan por primera vez en el patio, chocan mochilas, se miran raro, después se ríen.)*

**Prompt imagen (Higgsfield):**
```
Vista general de una base militar de caricatura al pie de una cordillera
nevada, banderas argentinas flameando, un hangar de Fuerza Aérea a la
izquierda con un avión Hércules estilizado, carpas y camiones verdes
del Ejército a la derecha, cielo despejado, estilo ilustración editorial,
composición amplia tipo establishing shot,
[+ prompt base de consistencia]
```

**Prompt video (Seedance 2.0), ~8s:**
```
Imagen a video, toma de establecimiento: cámara hace un paneo lento de
izquierda a derecha sobre la base militar, banderas argentinas ondeando
con viento suave, una hélice del avión Hércules gira lentamente al fondo,
soldados diminutos caminando en el patio. Movimiento de cámara suave,
sin cortes bruscos, ideal para narración superpuesta.
```

---

### ESCENA 3 — La Misión (3:30–6:00)

*(Interior de una carpa de comando. Un mapa gigante de la cordillera sobre la mesa.)*

**CAPITÁN (personaje secundario, voz grave pero cómica):** "Muchachos, un sensor meteorológico de la Fuerza Aérea cayó en la zona alta hace dos días. Sin ese dato, no podemos avisar si viene una tormenta grande. Necesito que un piloto de radio... y un guía de montaña... vayan a buscarlo. Juntos."

**MONGUITO:** "¿Juntos? Capitán, yo con las alturas tengo un problema..."
**RIPIUR:** "¿Y yo con las radios qué se supone que hago? ¿Le grito más fuerte a la montaña?"
**CAPITÁN:** "Por eso mismo. Se necesitan el uno al otro. ¡Andando, patrulla!"

**Prompt imagen (Higgsfield):**
```
Interior de una carpa de comando militar de caricatura, un capitán con
bigote grande señalando un mapa gigante de una cordillera sobre una
mesa de madera, Monguito y Ripiur parados en posición de firmes pero
con caras de duda cómica, linterna colgante iluminando la escena,
[+ prompt base de consistencia]
```

**Prompt video (Seedance 2.0), ~8s:**
```
Imagen a video. El capitán golpea el mapa con el dedo índice mientras
habla (boca animada sutil), Monguito y Ripiur se miran de reojo el uno
al otro con cara de "¿en serio?", cámara fija tipo diálogo de historieta,
leve movimiento de zoom-in lento hacia el mapa al final.
```

---

### ESCENA 4 — Preparativos Cómicos (6:00–8:30)

**NARRADOR:** "Antes de subir, había que preparar el equipo... y ahí empezaron los problemas."

*(Montaje: Monguito empacando de todo menos lo necesario —una radio gigante, un termo de mate del tamaño de un tambor, medialunas—. Ripiur revisando cuerdas, piolet, carpa, poniendo los ojos en blanco.)*

**RIPIUR:** "Monguito, ¿para qué llevás el mate más grande de la Patagonia?"
**MONGUITO:** "¡La supervivencia empieza con la cabeza fría y el mate caliente, Ripiur!"

**Prompt imagen (Higgsfield):**
```
Interior de un depósito militar de caricatura, Monguito cargando una
mochila gigante desbordada con un termo enorme de mate, una radio
antigua y medialunas asomando, Ripiur al lado con mochila prolija de
montaña (piolet, cuerdas, carpa) mirándolo con cara de resignación
cómica, estantes de equipo militar de fondo,
[+ prompt base de consistencia]
```

**Prompt video (Seedance 2.0), ~9s:**
```
Imagen a video, montaje cómico: Monguito mete objetos absurdos uno
tras otro en la mochila que ya no cierra, rebotando cada vez que
intenta cerrarla; Ripiur niega con la cabeza en primer plano, corte
final con la mochila explotando y las medialunas volando por el aire.
Ritmo rápido tipo comedia física, cámara fija.
```

---

### ESCENA 5 — Viaje al pie de la Cordillera (8:30–10:30)

**NARRADOR:** "Un camión militar los llevó hasta el último puesto antes de la montaña. A partir de ahí, todo era a pie."

*(Toma del camión subiendo un camino de montaña sinuoso, Monguito con cara de mareado, Ripiur canturreando una marcha militar desafinada.)*

**Prompt imagen (Higgsfield):**
```
Camión militar verde de caricatura subiendo un camino sinuoso de
montaña con precipicio de un lado, Monguito asomado por la ventanilla
con cara de mareado, Ripiur al volante cantando con la boca abierta,
polvo detrás del camión, picos nevados de fondo,
[+ prompt base de consistencia]
```

**Prompt video (Seedance 2.0), ~8s:**
```
Imagen a video. El camión avanza traqueteando por el camino de montaña,
cámara lateral siguiendo el vehículo (tracking shot), polvo levantándose
de las ruedas, leve rebote de la carrocería en los pozos del camino,
Monguito se agarra con fuerza cada vez que el camión pega un salto.
```

---

### ESCENA 6 — Primer Obstáculo: el viento y la nieve (10:30–13:00)

**NARRADOR:** "A los pocos kilómetros de caminata, la cordillera les mostró los dientes."

*(Ventisca fuerte, casi no se ven, se agarran de una cuerda entre los dos.)*

**RIPIUR:** "¡Agarrate de la cuerda y no sueltes, pase lo que pase!"
**MONGUITO:** "¡Ripiur, no veo nada, esto es peor que la niebla en la pista de aterrizaje!"

*(Un golpe de viento hace volar la gorra de Monguito. Corren cómicamente detrás de ella.)*

**Prompt imagen (Higgsfield):**
```
Dos soldados de caricatura atados por una cuerda caminando encorvados
contra una ventisca fuerte, nieve horizontal cruzando la escena,
visibilidad baja, tonos blanco-azulados, la gorra de uno de ellos
volando por el aire, expresiones de esfuerzo exagerado,
[+ prompt base de consistencia]
```

**Prompt video (Seedance 2.0), ~10s:**
```
Imagen a video. Ventisca fuerte cruzando la pantalla de derecha a
izquierda, los dos personajes avanzan inclinados hacia adelante
luchando contra el viento, la gorra sale volando de la cabeza de
Monguito, él suelta la cuerda un instante y corre torpemente tras
ella mientras Ripiur lo tira de nuevo hacia la cuerda. Cámara con
temblor sutil simulando ráfagas de viento.
```

---

### ESCENA 7 — Se pierden (13:00–15:00)

**NARRADOR:** "Y como toda buena aventura... en algún momento, alguien se perdió."

*(Discusión cómica mirando un mapa al revés.)*

**MONGUITO:** "Yo digo que el sensor está para allá."
**RIPIUR:** "Monguito, tenés el mapa al revés."
**MONGUITO:** "...Eso explica muchas cosas."

**Prompt imagen (Higgsfield):**
```
Monguito sosteniendo un mapa de papel al revés con cara de total
confianza, Ripiur señalando el mapa con cara de incredulidad,
parados sobre una roca con vista panorámica de la cordillera nevada
detrás, luz de atardecer dorada,
[+ prompt base de consistencia]
```

**Prompt video (Seedance 2.0), ~7s:**
```
Imagen a video. Ripiur estira la mano y gira el mapa 180 grados en
las manos de Monguito; la cara de Monguito pasa de confianza a
sorpresa cómica, Ripiur se lleva la mano a la cara (facepalm),
cámara fija con leve zoom-in al mapa girando.
```

---

### ESCENA 8 — Encuentro con un cóndor (15:00–17:30)

**NARRADOR:** "La Cordillera también tiene sus propios guardianes..."

*(Un cóndor andino gigante sobrevuela bajo, los asusta, Monguito se tira al piso, Ripiur se queda mirando fascinado.)*

**RIPIUR:** "Tranquilo, es un cóndor, es el dueño de esta montaña."
**MONGUITO:** "¡Bueno, que sea dueño desde más arriba, por favor!"

**Prompt imagen (Higgsfield):**
```
Un cóndor andino gigante de caricatura volando bajo y cerca de cámara
con las alas extendidas, Monguito tirado boca abajo en la nieve
cubriéndose la cabeza con las manos, Ripiur de pie mirando hacia
arriba con admiración, picos nevados de fondo, luz de atardecer,
[+ prompt base de consistencia]
```

**Prompt video (Seedance 2.0), ~9s:**
```
Imagen a video. El cóndor desciende en picada hacia cámara y luego
vira hacia arriba pasando muy cerca (efecto de sobrevuelo), su sombra
cruza rápido sobre los personajes, Monguito se agacha y cubre su
cabeza de forma exagerada, Ripiur sigue con la mirada el vuelo del
cóndor sin inmutarse. Cámara con leve movimiento ascendente siguiendo
al ave.
```

---

### ESCENA 9 — Encuentran el sensor... en un lugar peligroso (17:30–20:00)

**NARRADOR:** "Finalmente, lo encontraron. Pero, como era de esperar, no iba a ser tan fácil."

*(El sensor meteorológico está enganchado en una saliente de un acantilado, sobre una grieta.)*

**MONGUITO:** "Ahí está... justo en el peor lugar posible."
**RIPIUR:** "Tranquilo. Para esto entrené toda mi vida. Vos sos mis ojos por radio, yo bajo."

**Prompt imagen (Higgsfield):**
```
Un sensor meteorológico metálico con antena, enganchado en una saliente
rocosa sobre una grieta profunda nevada, Ripiur asomado al borde
mirando hacia abajo con una cuerda preparada, Monguito sosteniendo la
cuerda desde arriba con cara de tensión, luz fría de atardecer en la
montaña,
[+ prompt base de consistencia]
```

**Prompt video (Seedance 2.0), ~10s:**
```
Imagen a video. Ripiur se asegura la cuerda a la cintura y comienza a
descender por el borde del acantilado en rappel, pequeñas piedras
caen al vacío, Monguito sostiene la cuerda con las dos manos y la
cara tensa, mirando hacia abajo cada tanto y hacia el cielo (rezando
en broma). Cámara desde arriba mirando hacia el descenso (POV alto).
```

---

### ESCENA 10 — El rescate en equipo (Clímax) (20:00–22:30)

**NARRADOR:** "Este era el momento. El de Fuerza Aérea y el del Ejército, cada uno usando lo que mejor sabía hacer."

*(Ripiur baja y alcanza el sensor, pero una piedra se suelta y por poco lo golpea. Monguito, desde arriba, usa la radio para guiarlo por una ruta segura que solo se ve desde el aire/desde su ángulo.)*

**MONGUITO (por radio):** "¡Ripiur, dos metros a tu izquierda, la piedra de tu derecha no aguanta! ¡Confiá en mí!"
**RIPIUR:** "¡Copiado! ¡Vos guiá, que yo trepo!"

*(Ripiur logra asegurar el sensor y sube. Los dos gritan de alegría y chocan los cascos/gorras.)*

**Prompt imagen (Higgsfield):**
```
Ripiur trepando de vuelta el acantilado con el sensor meteorológico
asegurado en la espalda, roca suelta cayendo al vacío detrás suyo,
Monguito arriba con la radio en la mano gritando indicaciones con
gesto de brazo señalando una dirección, luz dorada de atardecer,
tensión y acción,
[+ prompt base de consistencia]
```

**Prompt video (Seedance 2.0), ~10s:**
```
Imagen a video. Una piedra se desprende cerca de Ripiur, él se corre
justo a tiempo hacia la izquierda siguiendo el grito de Monguito,
sigue trepando con impulso decidido hasta salir por el borde del
acantilado; al llegar arriba, ambos chocan cascos/gorras y saltan de
alegría. Cámara sigue el ascenso de abajo hacia arriba y termina en
plano general de festejo.
```

---

### ESCENA 11 — La tormenta que se acerca (22:30–24:30)

**NARRADOR:** "Pero la montaña no da tregua tan fácil..."

*(El cielo se oscurece de golpe, empieza a nevar fuerte. Deben correr a un refugio de emergencia que arman entre los dos, trabajando en perfecta sincronía por primera vez.)*

**Prompt imagen (Higgsfield):**
```
Cielo oscureciéndose con nubes de tormenta acercándose sobre la
cordillera, Monguito y Ripiur armando juntos una carpa de emergencia
naranja entre ráfagas de nieve, trabajando en equipo, uno sosteniendo
las varillas y el otro clavando las estacas, urgencia en sus caras,
[+ prompt base de consistencia]
```

**Prompt video (Seedance 2.0), ~9s:**
```
Imagen a video. Los dos personajes arman la carpa de emergencia con
movimientos rápidos y coordinados mientras la nieve empieza a caer
con fuerza, se meten adentro justo cuando arrecia la ventisca, la
carpa se sacude por el viento pero aguanta. Cámara fija con nieve
cayendo en primer plano (efecto de profundidad).
```

---

### ESCENA 12 — Adentro del refugio: la charla de amistad (24:30–26:00)

**NARRADOR:** "Y ahí, apretados en una carpa de dos por dos, pasó algo que ninguno esperaba: se hicieron amigos de verdad."

**RIPIUR:** "Che, Monguito... para ser de Fuerza Aérea, no estuviste nada mal hoy."
**MONGUITO:** "Y vos para ser del Ejército, casi me hacés sentir seguro en la montaña. Casi."
*(Se ríen, comparten el mate del termo gigante que tanto se había burlado Ripiur.)*
**RIPIUR:** "Este mate... la verdad que vino bien."
**MONGUITO:** "Te lo dije. La supervivencia empieza con la cabeza fría y el mate caliente."

**Prompt imagen (Higgsfield):**
```
Interior de una carpa de emergencia pequeña de noche, Monguito y
Ripiur sentados uno frente al otro compartiendo un mate de un termo
gigante, linterna colgando iluminando la escena con luz cálida,
afuera se ve la ventisca a través de la tela de la carpa, ambiente
acogedor y de amistad,
[+ prompt base de consistencia]
```

**Prompt video (Seedance 2.0), ~8s:**
```
Imagen a video. Monguito ceba el mate y se lo pasa a Ripiur, quien
lo toma y asiente con aprobación, ambos sonríen y chocan los puños,
la luz de la linterna parpadea suavemente, afuera se ve la sombra de
la nieve cayendo sobre la tela de la carpa. Cámara fija, plano medio.
```

---

### ESCENA 13 — Regreso a la base (26:00–27:30)

**NARRADOR:** "Con la tormenta pasada y el sensor a salvo, era hora de volver."

*(Caminata de regreso al amanecer, ahora sincronizados, bromeando como viejos amigos. Llegan a la base, el Capitán los recibe.)*

**CAPITÁN:** "¿Y el sensor?"
**RIPIUR:** "Entregado, mi Capitán. Con la ayuda de mi... compañero de Fuerza Aérea."
**MONGUITO:** "Compañero de patrulla, para toda la vida."

**Prompt imagen (Higgsfield):**
```
Amanecer sobre la cordillera, Monguito y Ripiur caminando de regreso
hacia la base militar a lo lejos, luz cálida de sol naciente, sombras
largas, caminando al mismo ritmo y sonriendo, sensor meteorológico
visible en la mochila de Ripiur,
[+ prompt base de consistencia]
```

**Prompt video (Seedance 2.0), ~8s:**
```
Imagen a video, toma panorámica: los dos personajes caminan hacia la
cámara con la base militar de fondo iluminada por el amanecer, el sol
sale lentamente detrás de los picos nevados, leve destello de luz
(lens flare), cámara estática con foco en la silueta caminando.
```

---

### ESCENA 14 — Cierre y moraleja (27:30–28:30)

**NARRADOR:** "Y así, la Fuerza Aérea y el Ejército Argentino nos enseñaron algo importante: no importa el uniforme que lleves puesto, en equipo se llega más lejos... y con un buen mate, cualquier tormenta se aguanta."

*(Los dos posan para una foto grupal con el resto de la base, todos riendo, bandera argentina de fondo. Gag final: la mochila de Monguito explota y llueven medialunas sobre todos.)*

**NARRADOR:** "¿Querés ver la próxima misión de Monguito y Ripiur? ¡Suscribite y activá la campanita, que la Cordillera todavía tiene muchas sorpresas guardadas!"

**Prompt imagen (Higgsfield):**
```
Foto grupal de caricatura frente a la base militar, Monguito y Ripiur
al centro con los brazos sobre los hombros del otro, soldados
secundarios alrededor riendo, bandera argentina gigante de fondo,
medialunas cayendo desde arriba en el aire (gag cómico), luz de día
brillante,
[+ prompt base de consistencia]
```

**Prompt video (Seedance 2.0), ~8s:**
```
Imagen a video. Todo el grupo posa sonriendo para la foto, de repente
la mochila de Monguito explota desde atrás y las medialunas salen
disparadas hacia arriba en cámara lenta, todos miran hacia arriba
riendo, la bandera argentina ondea de fondo. Cierre con freeze-frame
en el último fotograma tipo "foto final".
```

---

## 3. CHECKLIST DE PRODUCCIÓN

- [ ] Generar ficha de personajes (Escena 1 del bloque de fichas) primero y usarla como referencia en TODAS las imágenes siguientes.
- [ ] Generar las ~14 imágenes clave (una por escena) en Higgsfield.
- [ ] Generar los ~15-18 clips de Seedance 2.0 indicados (los momentos de acción).
- [ ] Grabar narración en off (tono entusiasta, ritmo "explorador de aventuras").
- [ ] Grabar/generar voces de Monguito (más aguda, alegre) y Ripiur (más grave, firme pero risueña) — se puede usar clonación de voz o TTS con personalidad.
- [ ] Editar: imágenes fijas con paneo/zoom lento + clips animados en los golpes de humor/acción + narración y diálogos + música de fondo tipo aventura/folclore liviano.
- [ ] Duración final objetivo: 25-28 minutos.
