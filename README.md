# Calculadora Solitarios Medici en español

v1.4.2

El script libre para plegar Solitarios Medici.

He visto otras implementaciones, pero no he encontrado ninguna en código abierto. El tipo que escribió la calculadora de SM en Windows a principios de siglo, que yo sepa, no hizo publico el código. Me imaginé que tenía sentido programar tal cosa en TypeScript, al no existir ningún cálculo complicado, por lo que las velocidades de los motores JS son aceptables, además de que es barato, simple y popular.

La librería básica es [MediciSolitaireCalculator.ts](https://github.com/assador/medici/blob/master/src/components/MediciSolitaireCalculator/MediciSolitaireCalculator.ts). Todo lo demás es una implementación específica de trabajo en Vue.js, que puede obviarse al utilizar la biblioteca en cualquier otro entorno.

## Instalación

1. Clonar repositorio
2. Una vez clonado: `npm install` y `seguidamente npm run build`
2. O simplemente toma el archivo [MediciSolitaireCalculator.ts](https://github.com/assador/medici/blob/master/src/components/MediciSolitaireCalculator/MediciSolitaireCalculator.ts) y úsalo como consideres (bajo los términos de la GPLv3)

## Vue.js descripción de la aplicación

A continuación se describe cómo funciona la implementación en Vue.js. Puede ejecutarse libremente en <https://sof14dh.github.io/medici> o en el sitio oficial <https://assador.github.io/medici> (en ruso).

### El apartado "Bloque de Trabajo"

Este bloque mostrará una baraja desplegada. Establezca las condiciones iniciales; por ejemplo, cartas predeterminadas en los lugares correctos. A continuación, haga clic en el botón "Plegar".

### El bloque “Presstablecer Cartas”

Selecciona las cartas que permanecerán en las posiciones indicadas (el número debajo de la carta) al calcular el plegado de la baraja. Para predeterminar una carta, primero haz clic en la carta deseada en este bloque y, a continuación, en la carta del bloque de trabajo en cuya posición (indicada por el número situado debajo de la carta)s deseas que aparezca la carta que ha seleccionado.

Debajo de este bloque en forma de baraja ordenada, se muestran las cartas que ya ha predeterminado. Para eliminar una carta preestablecida, haga clic sobre ella en este bloque.

### "Lista de mazos guardados"

Este bloque mostrará una lista de las barajas plegadas guardadas. Para guardar un mazo apilado, haga clic en el botón «Añadir a la lista», que aparece después de Plegar el "Bloque de Trabajo". El mazo apilado activo, que se muestra en el "Bloque de Trabajo", aparece resaltado en esta lista. Puede seleccionar cualquier mazo previamente guardado en la misma. Cuando realice cambios en el "Bloque de Trabajo", por ejemplo, añadiendo Cartas Preestablecidas seguidas de un nuevo plegado y vuelva a pulsar el botón «Añadir a la lista», ¡el nuevo mazo calculado sobreescribirá en la lista al mazo resaltado! Si quiere guardar un nuevo cálculo en la lista, haga click en el botón «Nuevo» que se encuentra un poco antes. En este caso ninguno de ellos aparecerá resaltado en la lista de mazos guardados. 

### Importar y Exportar

Puede guardar sus resultados en un archivo y volver a cargarlos desde el archivo almacenado previamente. Para guardar, haga clic en el botón "Exportar". Se le pedirá que guarde el archivo en formato JSON en algún sitio. Para cargar desde un archivo, haga clic en el botón "Importar". Exportación a archivo e importación desde archivo hacia el bloque de trabajo y la lista de mazos guardados.

***
Si de repente te entrase el insensato impulso de hacer una donación, desinteresada o caprichosa, puedes hacerlo aquí: <https://www.paypal.me/niaouveas>. En caso de que tengas alguna duda particular, puedes escribirme un correo a [assador@gmail.com](mailto:assador@gmail.com). (Ambos enlaces son los oficiales del creador del aplicativo).

Se trata de un software libre publicado bajo licencia GNU GPL v3 (véase el archivo LICENSE).


***

# Medici Solitaire Calculator

v1.4.2

Свободный скрипт для складывания пасьянса Медичи.

Другие реализации видел, но открытого кода не находил. Тот чувак, что писал виндовый ПМ-калькулятор в начале века, насколько знаю, код не открывал. Решил, что такую штуку имеет смысл писать на TypeScript — замороченных вычислений не будет, так что скорости JS-движков приемлемы, зато дёшево, сердито, просто и популярно. 

Основная библиотека — [MediciSolitaireCalculator.ts](https://github.com/assador/medici/blob/master/src/components/MediciSolitaireCalculator/MediciSolitaireCalculator.ts). Всё остальное — конкретная рабочая реализация на Vue.js, которой можно пренебречь при использовании этой библиотеки где бы то ни было ещё.

## Установка

1. Склонировать репозиторий
2. В склонированном каталоге: `npm install && npm run build`
2. Или просто берёте файл [MediciSolitaireCalculator.ts](https://github.com/assador/medici/blob/master/src/components/MediciSolitaireCalculator/MediciSolitaireCalculator.ts) и делаете с ним всё, что заблагорассудится (в рамках GPLv3)

## Описание работы реализации на Vue.js

Ниже описана работа готовой сборки скрипта на Vue.js. Ею можно пользоваться свободно по адресу: <https://assador.github.io/medici>.

### Блок «Рабочая колода»

В этом блоке будет выводиться складывающаяся колода. Задайте начальные условия; например, предопределённые на нужных местах карты. Затем нажмите на кнопку «Сложить».

### Блок «Предопределение карт»

Выбор карт, которые при расчёте складывающейся колоды будут оставаться на указанных вами местах (число под картой). Для предопределения карты нажмите сначала на нужную карту в этом блоке, потом на ту карту в блоке рабочей колоды, на позиции которой (указывается номером под картой) вы хотите видеть выбранную вами.

Под этим блоком с упорядоченной колодой, ниже, показываются уже предопределённые вами карты. Для того, чтобы убрать предопределение какой-либо карты, нажмите на неё в этом блоке.

### «Список сохранённых колод»

В этом блоке будет выводиться список сохранённых вами в памяти сложенных колод. Для сохранения сложенный колоды нажмите кнопку «Добавить в список», которая появляется после расчёта сложенной колоды. Активная сложенная «рабочая» колода, показываемая в основной области, в этом списке выделена фоном. Вы можете выбрать в этом списке любую сохранённую ранее колоду. При этом она появится также в блоке «Рабочая колода». При внесении изменений в эту рабочую колоду, например, при добавлении зарезервированных (предопределённых) карт с последующим новым расчётом и новом клике по кнопке «Добавить в список» новая рассчитанная колода будет сохранена вместо этой выделенной, рассчитанной прежде! Если вы хотите сохранить в списке новый расклад, перед ним нажмите на кнопку «Новая». При этом, в списке сохранённых колод ни одна из них не будет выделена.

### Импорт и экспорт

Вы можете сохранять результаты работы в файл и загружать ранее сохранённые из файла. Для сохранения нажмите на кнопку «Сохранить». Вам будет предложено сохранить куда-нибудь файл в формате JSON. Для загрузки из файла нажмите на кнопку «Импортировать». Экспортируются в файл и импортируются из файла: рабочая колода и список сохранённых колод.

***
Если у вас вдруг возникло глупое желание пожертвовать мне денежку, бескорыстно или нет, вы можете сделать это здесь: <https://www.paypal.me/niaouveas>. Бескорыстное желание, если таковое имеется, можно выразить, написав письмо на [assador@gmail.com](mailto:assador@gmail.com).

Это свободное программное обеспечение, опубликованное под GNU GPL v3 (см. файл LICENSE).

***
## And one more time by English…

The free script for Medici solitaire folding. I’ve seen other implementations, but I haven’t found any open source code. The guy who wrote the Windows PM Calculator at the beginning of the century, as far as I know, did not open source. I figured that it makes sense to write such a thing in TypeScript — there won’t be any complicated calculations, so JS engines speeds are acceptable, but it is cheap, simple and popular.

Basic library is [MediciSolitaireCalculator.ts](https://github.com/assador/medici/blob/master/src/components/MediciSolitaireCalculator/MediciSolitaireCalculator.ts). Everything else is a specific working implementation in Vue.js, which can be neglected when using the library anywhere else.

## Installation

1. Clone repository
2. Inside cloned: `npm install && npm run build`
2. Or just take [MediciSolitaireCalculator.ts](https://github.com/assador/medici/blob/master/src/components/MediciSolitaireCalculator/MediciSolitaireCalculator.ts) file and do what you want to (under the terms of GPLv3)

## Vue.js implementation description

Below is a description of how the Vue.js implementation works. It can be used freely at <https://assador.github.io/medici>.

### The “Working deck” block

This block will display a folded deck. Set the initial conditions; for example, predetermined cards at the right places. Then click on the “Fold“ button.

### The “Card Predetermination” block

Select the cards that will remain in the locations you specify (the number below the card) when calculating the folding deck. To predetermine a card, click first on the card you want in this block, then on the card in the working deck block whose position (indicated by the number below the card) you want to see the card you selected.

Below this ordered deck block, the cards you have already predetermined are shown. To remove a predetermined card, click on it in this block.

### “Saved Deck List”

This block will display a list of your saved folded decks. To save the folded deck, press the “Save to list” button that appears after the calculation of the folded deck. The active “working” folded deck, shown in the main area, is highlighted in the background in this list. You can select any previously saved deck in this list. It will also appear in the “Working deck“ block. When you make changes to this working deck, such as adding reserved (predetermined) cards followed by a new calculation and clicking the “Save to list” button again, the new calculated deck will be saved instead of this previously calculated selected one! If you want to save a new deck to the list, click the “New” button before it. In this case, in the list of saved decks, none of them will be highlighted.

### Import and export

You can save your results to a file and load previously saved from the file. To save, click the “Save” button. You will be prompted to save the file in JSON format somewhere. To load from a file, click on the “Import” button. Exporting to file and importing from file: the working deck and the list of saved decks.

***
If you suddenly have a foolish desire to donate, disinterestedly or selfishly, you can do it here: <https://www.paypal.me/niaouveas>. Self-interest, if any, can be expressed by writing a letter to [assador@gmail.com](mailto:assador@gmail.com).

This is a free software published under GNU GPL v3 (see LICENSE file).
