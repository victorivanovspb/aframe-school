<!-- Title slide. -->
<!-- .slide: data-background="media/img/aframe.jpg" -->

<div class="talk-title">
  <h1>Школа A-Frame</h1>
  <h3>Интерактивный курс по WebVR</h3>
  <p class="talk-info">
    <b><a href="https://aframe.io">aframe.io</a></b>
  </p>
</div>

------

## Пролог

<!-- .slide: data-background="media/img/aframe.jpg" -->

> С помощью [Glitch](https://glitch.com) в школе вам даются упражнения «шаг за шагом»,
> чтобы помочь вам погрузиться в мир [WebVR](https://webvr.rocks)! В школе перемещение
> по разделам осуществляется &larr; and &rarr, а перемещение между подразделами **&uarr; and
> &darr;**:

<img class="stretch" data-src="media/img/navigation.jpg">

**Навигация &darr;**

---

### Полезные ресурсы во время вашего путешествия

1. [Просмотрите Документацию и Часто задаваемые вопросы](https://aframe.io/docs/)
2. [Обратитесь за помощь на Slack](https://aframe.io/community/#slack)
3. [Задайте вопрос на Stack Overflow](http://stackoverflow.com/questions/ask/?tags=aframe)
4. Если вы участвуете в семинаре , то поднимите свою руку, если у вас есть вопрос!

**Навигация &rarr;**


<!-- Lessons start below. -->


------

## Glitch &mdash; введение

> Школа использует [Glitch](https://glitch.com) в качестве среды обучения
> и разработки для A-Frame

<img class="stretch" data-src="media/img/glitch.jpg">

- Glitch запускает ваш код в браузере без необходимости дополнительноустанавливать
что-нибудь ещё
- Glitch позволяет **переделывать** проекты с использованием существующих проектов A-Frame
  в качестве отправной точки
- Glitch мгновенно публикует и хранит ваш сайт с URL-адресом (например,
  `https://aframe.glitch.me`)
- Glitch обновляет ваш сайт с A-Frame в реальном времени при каждом изменении кода
- Glitch позволяет нескольким людям работать с кодом в одном проекте

*Если вы заинтересованы в установке локального окружения для разработки, пропустите шаг &darr;*

---

## Glitch &mdash; переделывание существующего проекта

> Glitch позволяет переделать (или сделать ответвление) существующий проект и использовать это в качестве основы для вашего
> нового проекта. Перед тем как начать, мы рекомендуем связать аккаунт в Glitch с вашим [аккаунтом в GitHub
> ](https://github.com/). Glitch предоставит вам имя проекта и его URL-адрес,
> сгенерированные случайным образом, которые вы можете изменить.

<img class="stretch" data-src="media/img/glitch2.jpg">

<a href="https://glitch.com/~aframe/" target="_blank">Переделать заготовленные проекты A-Frame в Glitch</a>  <!-- .element: class="cta-button glitch" -->

---

## Glitch &mdash; редактирование кода

> После того, как вы [переделали заготовку A-Frame в Glitch](https://glitch.com/~aframe/),
> проверьте, где вы будете редактировать свой код. Осмотритесь вокруг и убедитесь, что вы можете
> редактировать код серверной части, загружать ассеты, создавать новые файлы, или приглашать 
> других, чтобы редактировать с вами!

<img class="stretch" data-src="media/img/glitch3.jpg">

---

## Glitch &mdash; просмотр вашего проекта

> После того как вы поработали в редакторе, посмотрите ваш проект в действии.

<img class="stretch" data-src="media/img/glitch4.jpg">

---

## Glitch &mdash; экспортирование вашего проекта

> В любой момент времени, если вы захотите скачать свой проект или экспортировать его на GitHub, можете
> обратиться к пункту меню *Дополнительные опции*. Скачивание даст вам файл с расширением `.tgz`, который вы сможете
> распаковать. В проектах A-Frame, от вас потребуется работать с тем, что находится в директории `public/`,
> а код серверной части игнорировать.

<img class="stretch" data-src="media/img/glitch5.jpg">

Если вы скачиваете проект, вам
может быть интересно узнать про создание окружения для веб-разработки в следующем
разделе **&darr;**. В противном случае, жмите **&rarr;** для того, чтобы приступить к изучению A-Frame!

---

## [Дополнительно] Установка окружения web-разработки

> Вы можете установить полноценное окружение web-разработки на вашей локальной машине,
> а не использовать онлайн-среду web-разработки Glitch.

<img class="stretch" data-src="media/img/webdevenv1.jpg">

1. **Получите текстовый редактор:** [Atom](https://atom.io) хороший вариант для начала
2. **Установите локальный сервер:** Скачайте и запустите [Mongoose
Server](https://www.cesanta.com/products/binary) или запустите `python -m
SimpleHTTPServer` в консоли
3. **Создайте файл `index.html`** и скопируйте код A-Frame из представленных в Glitch примеров
4. **Запустите локальный сервер** в той же директории, что и файл HTML
5. **Откройте URL-адрес локального сервера** в вашем браузере (например, `http://localhost:8000`)
6. **Внесите изменения** в ваш HTML файл и перезагрузите браузер, чтобы увидеть их
7. Дополнительно: попробуйте [ngrok](https://ngrok.io) для того, чтобы любое устройство в любой
сети имело доступ к вашему локальному серверу

---

## [Дополнительно] Установка окружения web-разработки &mdash; получите текстовый редактор

> [Atom](https://atom.io) — хороший текстовый редактор для начала, если у вас нет ничего другого.
> Другими популярными вариантами являются: [Notepad++](https://notepad-plus-plus.org/),
> [Sublime](https://www.sublimetext.com/), [Brackets](http://brackets.io/) или
> [vim](http://www.vim.org/download.php).

<img class="stretch" data-src="media/img/webdevenv2.jpg">

---

## [Дополнительно] Установка окружения web-разработки &mdash; установите локальный сервер

> Вам будет нужен локальный HTTP-сервер, чтобы обслуживать ваши файлы в браузере.

<div class="captioned-image-row small">
  <div>
    <img data-src="https://cloud.githubusercontent.com/assets/8731271/24021623/10654d22-0a5f-11e7-9769-63cdff91637c.png">
    <a href="https://www.cesanta.com/products/binary">Mongoose Binary</a>
  </div>
  <div>
    <img data-src="https://www.python.org/static/opengraph-icon-200x200.png">
    <code>python -m SimpleHTTPServer 8080</code>
  </div>
  <div>
    <img data-src="https://www.echosteg.com/images/blog/standard/nodejs_logo.png">
    <a href="https://docs.npmjs.com/getting-started/installing-node">Node + npm + live-server</a>
  </div>
</div>

---

## [Дополнительно] Установка окружения web-разработки &mdash; используйте ngrok

> При желании вы можете использовать [ngrok](https://ngrok.com/) для того, чтобы разрабатывать свой
> A-Frame проект со смартфона без необходимости выполнять настройку доступа к локальному IP-адресу.

1. Скачайте и распакуйте [ngrok](https://ngrok.com/download/) в любое место
2. Запустите ngrok, предоставив ему номер порта вашего локального сервера (`./ngrok http 8080`)
3. ngrok предоставит вам URL-адрес, состоящий из набора букв и цифр (e.g., `https://abcdef123456.ngrok.io`)
4. Откройте этот URL-адрес с другого устройства в любой сети (таком как смартфон или другой компьютер)

<img class="stretch" data-src="media/img/webdevenv3.jpg">

------

## Попробуйте примеры A-Frame

> Поработайте с примерами в вашем десктопе или смартфоне [на странице
> A-Frame](https://aframe.io), [в блоге A-Frame](https://aframe.io/blog/), или
> [awesome-aframe](https://github.com/aframevr/awesome-aframe). Посмотрите
> [webvr.rocks](https://webvr.rocks) для получения информации о настройке WebVR with с
> гарнитурой, если она у вас есть.

<img data-src="media/img/examples.gif">

------

## Начните с *Привет, WebVR*

> A-Frame предоставляет простые в использовании HTML элементы, называемые
[примитивами](https://aframe.io/docs/0.5.0/primitives/). В разделе ниже
мы изменим основные мэши через HTML аттрибуты (например, цвет,
положение, вращение, масштаб) и дадим почувствовать рабочий процесс.

<img data-src="media/img/hellowebvr2.jpg">

<img class="stretch" data-src="media/img/hellowebvr.jpg">

---

## Начните с *Привет, WebVR* &mdash; положение

> Положение определяет где объекты находятся в трехмерном пространстве (X, Y, Z) в метрах. Изменяйте
> `положение` объектов через атрибуты `позиции` в HTML. [Почитайте о
> положениях](https://aframe.io/docs/master/components/position.html).

<a href="https://glitch.com/~aframe-school-position" target="_blank">Переделать урок в Glitch</a>  <!-- .element: class="cta-button glitch" -->

1. Переместите цилиндр влево, чтобы *уменьшить* значение `позиции` по оси X
2. Переместите поле вверх, чтобы *увеличить* значение `позиции` по оси Y
3. Переместите сферу назад, чтобы *уменьшить* значение `позиции` по оси Z
4. **Дополнительно:** Добавьте `<a-ring>` в качестве дочернего элемента `<a-sphere>` и дайте ему возможность видеть относительные позиции

<img class="stretch" data-src="media/img/positionresult.jpg">

<a href="https://aframe-school-position.glitch.me/solution.html" target="_blank">Посмотреть результат</a>  <!-- .element: class="cta-button" -->

---

## Начните с *Привет, WebVR* &mdash; вращение

> Вращение определяет ориентацию объектов в трехмерном пространстве (по осям X, Y, Z)
> в градусах. Используйте правило правой руки, чтобы пространственно визуализировать вращение. [Почитайте о
> вращениях](https://aframe.io/docs/master/components/rotation.html).

<a href="https://glitch.com/~aframe-school-rotation" target="_blank">Переделать урок в Glitch</a>  <!-- .element: class="cta-button glitch" -->

1. Поверните цилиндр вокруг оси X так, чтобы мы увидели его дно
2. Поверните поле вокруг оси Y так, чтобы оно было обращено прямо
3. **Дополнительно:** Оберните контент сцены в `<a-entity>` (как `<div>`)
и поверните её, чтобы увидеть относительные вращения

<img class="stretch" data-src="media/img/rotationresult.jpg">

<a href="https://aframe-school-rotation.glitch.me/solution.html" target="_blank">Посмотреть результат</a>  <!-- .element: class="cta-button" -->

---

## Начните с *Привет, WebVR* &mdash; добавление примитивов

> Добавьте примитивы в сцену, включив HTML элементы внутрь `<a-scene>`.  [Почитайте
> о примитивах](https://aframe.io/docs/0.5.0/primitives/).

<a href="https://glitch.com/~aframe-school-primitives" target="_blank">Переделать урок в Glitch</a>  <!-- .element: class="cta-button glitch" -->

1. Добавьте [`<a-torus-knot>`](https://aframe.io/docs/0.5.0/primitives/a-torus-knot.html) в левую часть
2. Добавьте [`<a-dodecahedron>`](https://aframe.io/docs/0.5.0/primitives/a-dodecahedron.html) в правую часть
3. Добавьте [`<a-text>`](https://aframe.io/docs/0.5.0/primitives/a-text.html), выровненный по центру

<img class="stretch" data-src="https://cloud.githubusercontent.com/assets/674727/24266010/9c57cbe4-0fc2-11e7-968f-168f3649d109.png">

<a href="https://aframe-school-primitives.glitch.me/solution.html" target="_blank">Посмотреть результат</a>  <!-- .element: class="cta-button" -->

------

## Add Textures &mdash; Uploading Assets

> We'll be adding image textures to meshes to more appearance than a flat color.
> [Find your own images
> online](https://aframe.io/docs/0.5.0/introduction/faq.html#where-can-i-find-assets),
> and upload them through the assets section in Glitch or through the uploader on
> [cdn.aframe.io](https://cdn.aframe.io). Wherever else you may upload, make sure
> it's being served with
> [CORS](https://developer.mozilla.org/docs/Web/HTTP/Access_control_CORS) and
> over HTTPS.

<img class="stretch" data-src="media/img/glitchasset.jpg">

In the Glitch below **&darr;**, some assets will already be provided in the
assets section (pictured above).

---

## Add Textures &mdash; Image Textures

> Fill in the `src` HTML attributes with image URLs. [Read about applying an
> image texture](https://aframe.io/docs/0.5.0/guides/building-a-basic-scene.html#applying-an-image-texture).

<a href="https://glitch.com/~aframe-school-textures/" target="_blank">Remix Lesson on Glitch</a>  <!-- .element: class="cta-button glitch" -->

1. Add an image texture to the ground, `<a-plane>`
2. Add image textures to `<a-box>`es
3. Add an image texture to `<a-sphere>`
4. Add an image texture to `<a-cone>`
5. Add an image texture to the background, `<a-sky>`. Find [360&deg; images from FLickr](https://www.flickr.com/groups/equirectangular/)

<img class="stretch" data-src="media/img/texture.jpg">

<a href="https://aframe-school-textures.glitch.me/solution.html" target="_blank">View Result</a>  <!-- .element: class="cta-button" -->

------

## Open the A-Frame Inspector

> Hit **`<ctrl> + <alt> + i`** on **any** A-Frame scene to pop open a visual
> editor, just like your browser's Dev Tools!  Try the Inspector on some of the
> [homepage examples](https://aframe.io/examples/). [Read about the
> Inspector](https://aframe.io/docs/master/guides/using-the-aframe-inspector.html).

<img class="stretch" data-src="media/img/inspector.gif">

---

## Open the A-Frame Inspector &mdash; Change Component Values

> Modify an entity by modifying its components on the right-hand panel. The
> Inspector knows about all A-Frame components, including community components.
>  This example includes an external [text-geometry
> component](https://www.npmjs.com/package/aframe-text-geometry-component), which
> the Inspector can modify the values of live.

<a href="https://aframe-vaporwave.glitch.me" target="_blank">Open Example on Glitch</a>  <!-- .element: class="cta-button glitch" -->

1. Select one of the entities with text in the example
2. Change the [`text-geometry` component's](https://www.npmjs.com/package/aframe-text-geometry-component) `value` property

<img class="stretch" data-src="media/img/inspectorchange.jpg">

---

## Open the A-Frame Inspector &mdash; Attach Components from the Registry

> Use [physics components](https://github.com/donmccurdy/aframe-physics-system)
> from the [Registry](https://aframe.io/registry/) to add gravity and collisions.
> The Registry is a curated collection of A-Frame components. And the Inspector
> is hooked up to the Registry so we can add components from the Registry in the
> entity panel.

<a href="https://aframe-vaporwave.glitch.me" target="_blank">Open Example on Glitch</a>  <!-- .element: class="cta-button glitch" -->

1. Add the `static-body` component to ground grid
2. Add the `dynamic-body` component to the torus knot (the purple pretzel in the back)
3. Increase the Y-position of the torus knot to make it higher up
4. Exit the Inspector

<img class="stretch" data-src="media/img/inspectorregistry.gif">

------

## Compose with Entity-Component &mdash; Break Primitives Down

> Behind the easy-to-use primitive elements, A-Frame is based on an
> entity-component architecture. Decompose the primitive elements in the
> *Hello, WebVR* example to `<a-entity>`s with their fundamental components.

<a href="https://glitch.com/~aframe-school-ecs" target="_blank">Remix Lesson on Glitch</a>  <!-- .element: class="cta-button glitch" -->

[geometry]: https://aframe.io/docs/0.5.0/components/geometry.html
[material]: https://aframe.io/docs/0.5.0/components/material.html

1. Convert `<a-box>` to `<a-entity>` with [geometry component][geometry] and [material component][material]. Configure the geometry component to be `primitive: box`
2. Convert `<a-sphere>` to `<a-entity>` with geometry component and material component. Configure the geometry component to be `primitive: sphere`
3. Convert `<a-cylinder>` to `<a-entity>` with geometry component and material component. Configure the geometry component to be `primitive: cylinder`
4. Convert `<a-plane>` to `<a-entity>` with geometry component and material component. Configure the geometry component to be `primitive: plane`
5. Convert `<a-sky>` to `<a-entity>` with geometry component and material component. Configure the geometry component to be `primitive: sphere` with a large `radius: 3000`, and configure the material component to be `shader: flat` so we don't do expensive lighting calculations when we just need a flat color

<a href="https://aframe-school-ecs.glitch.me/solution.html" target="_blank">View Result</a>  <!-- .element: class="cta-button" -->

---

## Compose with Entity-Component &mdash; Add a Light Source Sphere

> Use the entity-component pattern to add a sphere that also acts as a point
> light source. Mix together the geometry, material, and light components to
> compose this type of object.

1. Look for `<a-entity id="lightSphere">`
2. Attach the [geometry component](https://aframe.io/docs/0.5.0/components/geometry.html) configured to use `primitive: sphere` to the entity
3. Attach the [material component](https://aframe.io/docs/0.5.0/components/material.html) configured to use `color: #FFF` and `shader: flat` to the entity
4. Attach the [light component](https://aframe.io/docs/0.5.0/components/light.html) configured to use `type: point` to the entity
5. **Extra Credit:** Add the animation component from [the Registry](https://aframe.io/registry/) via a `<script>` tag. Attach the animation configured to use `property: position` and `dir: alternate` and `loop: true` and provide a position value for `to: <POSITION>`

<a href="https://glitch.com/~aframe-school-ecs-light-sphere" target="_blank">Remix Lesson on Glitch</a>  <!-- .element: class="cta-button glitch" -->

<img class="stretch" data-src="https://cloud.githubusercontent.com/assets/674727/24060160/2c53a604-0b0f-11e7-9386-f83a3a9b4cfc.gif">>

<a href="https://aframe-school-ecs-light-sphere.glitch.me/solution.html" target="_blank">View Result</a>  <!-- .element class="cta-button" -->

------

## Extend with Entity-Component &mdash; From the Registry

> [The Registry](https://aframe.io/registry/) is a great place to grab cool
> components that the community has added to A-Frame. Sort of like third-party
> plugins. Find community components from the Registry, copy their JS links,
> include them via a `<script>` tag, and use them straight from HTML.

1. Include [Particle
System](https://www.npmjs.com/package/aframe-particle-system-component). Attach
`<a-entity>`s with `particle-system` components configured to `preset: default`
and `preset: snow`. Open the Inspector to play with the values!
2. Include [Animation](https://www.npmjs.com/package/aframe-animation-component). Attach
animation to the sphere to throb its scale by configuring `animation` component
with `property: scale`, `loop: true`, and `to: 1.1 1.1 1.1`
3. Include [Outline Effect](https://www.npmjs.com/package/aframe-outline-effect). Drop in the
`<script>` and attach the `outline` component to the scene

<a href="https://glitch.com/~aframe-school-registry" target="_blank">Remix Lesson on Glitch</a>  <!-- .element: class="cta-button glitch" -->

<img class="stretch" data-src="media/img/registryexample.gif">

<a href="https://aframe-school-registry.glitch.me/solution.html" target="_blank">View Result</a>  <!-- .element class="cta-button" -->

------

## Use JavaScript

> Use JavaScript and DOM APIs to programmatically modify the scene and its
> entities. A-Frame is not just HTML; A-Frame provides access to JavaScript,
> DOM APIs, and three.js underneath for full control.  [Read about *Using
> JavaScript and DOM APIs* with
> A-Frame](https://aframe.io/docs/0.5.0/guides/using-javascript-and-dom-apis.html).

<a href="https://glitch.com/~aframe-school-js" target="_blank">Remix Lesson on Glitch</a>  <!-- .element: class="cta-button glitch" -->

<img class="stretch" data-src="media/img/js.jpg">

To see JavaScript logs, we can open the browser's development console by
right-clicking the page, clicking *Inspect* or *Inspect Element*, and then
clicking the *Console* tab. When viewing solutions, we can see the results
through the browser console.

---

## Use JavaScript &mdash; Getting Entities

> Use
> [`document.querySelector()`](https://developer.mozilla.org/docs/Web/API/Document/querySelector)
> and
> [`document.querySelectorAll()`](https://developer.mozilla.org/docs/Web/API/Document/querySelectorAll)
> to get a reference to the scene and its entities.  [Read about querying for
> entities](https://aframe.io/docs/0.5.0/guides/using-javascript-and-dom-apis.html#getting-entities-by-querying-and-traversing).

<a href="https://glitch.com/~aframe-school-js" target="_blank">Remix Lesson on Glitch</a>  <!-- .element: class="cta-button glitch" -->

1. Get a reference to the `<a-scene>` element using `var sceneEl = document.querySelector('a-scene');`
2. Get a reference to all `<a-entity>` elements using `sceneEl.querySelectorAll('a-entity');`
3. Get a reference to the box entity using `sceneEl.querySelector('#box');`
4. Get a reference to the sphere and cylinder entities in one `.querySelectorAll()` call by using multi-element selector
. Get a reference to the sphere and cylinder entities in one `.querySelectorAll()` call by adding and selecting HTML classes

<a href="https://aframe-school-js.glitch.me/solution.html" target="_blank">View Result</a>  <!-- .element: class="cta-button" -->

---

## Use JavaScript &mdash; Modifying Entities

> Use
> [`Entity.setAttribute()`](https://aframe.io/docs/0.5.0/core/entity.html#setattribute-attr-value-componentattrvalue)
> to modify entities after retrieving them from the previous exercise. [Read
> about modifying
> entities](https://aframe.io/docs/0.5.0/guides/using-javascript-and-dom-apis.html#modifying-an-entity).

<a href="https://glitch.com/~aframe-school-js" target="_blank">Remix Lesson on Glitch</a>  <!-- .element: class="cta-button glitch" -->

1. Change the box entity's `rotation` component
2. Change the cylinder entity's `geometry` component's `height` property
3. Change the sphere entity's `material` component's `metalness` property

<a href="https://aframe-school-js.glitch.me/solution2.html" target="_blank">View Result</a>  <!-- .element: class="cta-button" -->

---

## Use JavaScript &mdash; Creating Entities

> Use [`document.createElement()`](https://developer.mozilla.org/docs/Web/API/Document/createElement)
> to create entities, `.setAttribute()` to configure them, and `.appendChild()`
> to add them to the scene.  [Read about creating
> entities](https://aframe.io/docs/0.5.0/guides/using-javascript-and-dom-apis.html#creating-an-entity-with-createelement).

<a href="https://glitch.com/~aframe-school-js" target="_blank">Remix Lesson on Glitch</a>  <!-- .element: class="cta-button glitch" -->

1. In a JavaScript `for` loop, create and add 50 `<a-box>` elements with
random positions and scales (use `Math.random()`)

<a href="https://aframe-school-js.glitch.me/solution3.html" target="_blank">View Result</a>  <!-- .element: class="cta-button" -->

---

## Use JavaScript &mdash; Handling Events

> Use
> [`.addEventListener()`](https://developer.mozilla.org/docs/Web/API/EventTarget/addEventListener)
> to register a handler function that will be called when an event is emitted.
> Then manually emit that event to see that handler function execute. Later we
> can use event listeners to change the scene based on user input or other
> events. [Read about events and event listeners with
> A-Frame](https://aframe.io/docs/0.5.0/guides/using-javascript-and-dom-apis.html#events-and-event-listeners).

<a href="https://glitch.com/~aframe-school-js" target="_blank">Remix Lesson on Glitch</a>  <!-- .element: class="cta-button glitch" -->

1. Register an event listener on the box to listen to the `foo` event. In the
   handler function, change the box's color
2. Emit the `foo` event with
[`Entity.emit()`](https://aframe.io/docs/0.5.0/core/entity.html#emit-name-detail-bubbles)
and see the box change its color

<a href="https://aframe-school-js.glitch.me/solution4.html" target="_blank">View Result</a>  <!-- .element: class="cta-button" -->

------

## Add Gaze-Based Cursor Interactions &mdash; Add Cursor Entity

> Use the gaze-based [`cursor`
> component](https://aframe.io/docs/0.5.0/components/cursor.html) to provide
> the ability to interact with entities (primarily for smartphones).  [Read
> about building a 360&deg; image
> gallery](https://aframe.io/docs/0.5.0/guides/building-with-components.html).

<a href="https://glitch.com/~aframe-school-cursor" target="_blank">Remix Lesson on Glitch</a>  <!-- .element: class="cta-button glitch" -->

This lesson has all the event listeners hooked up already. We just need to add
an entity with the `cursor` component which will provide those events based on
user input.  Note these events are not provided by the browser, but through
A-Frame.

1. Add [`<a-camera>`](https://aframe.io/docs/0.5.0/components/camera.html) entity.
   Previously A-Frame was providing a default camera
2. Add [`<a-cursor>`](https://aframe.io/docs/0.5.0/components/cursor.html) entity
   as a child underneath the camera entity
3. Drag the camera around the click on the panels on desktop. On smartphones,
   stare at the panels to trigger clicks (i.e., gaze-based)

<img class="stretch" data-src="media/img/gaze.gif">

<a href="https://aframe-school-cursor.glitch.me/solution.html" target="_blank">View Result</a>  <!-- .element: class="cta-button glitch" -->

---

## Add Gaze-Based Cursor Interactions &mdash; Handle Events

> Use the `click`, `mouseenter`, `mouseleave` events provided by the gaze-based
> [`cursor` component](https://aframe.io/docs/0.5.0/components/cursor.html) to
> change the properties of an object.

The Glitch code will have the project structure set up. We can add JavaScript
code inside the `handle-events` component, marked by the code comments.

<a href="https://glitch.com/~aframe-school-cursor-handler" target="_blank">Remix Lesson on Glitch</a>  <!-- .element: class="cta-button glitch" -->

1. Attach our `controller-event-handler` to the cubes. We can attach to all of them at once through the mixin
2. Add an event listener to change the box's color on `mouseenter` event
3. Add an event listener to restore the box's color on `mouseleave` event

<img class="stretch" data-src="media/img/gazehandler.gif">

<a href="https://aframe-school-cursor-handler.glitch.me/solution.html" target="_blank">View Result</a>  <!-- .element: class="cta-button glitch" -->

------

## Add 3D Models &mdash; glTF Model

> 3D models are like the images of 3D and VR applications, although a bit
> heavier. A 3D model is created beforehand in a 3D modeling program such as
> [Blender](https://www.blender.org/) and consists of vertices, textures,
> materials. We recommend using [glTF](https://github.com/KhronosGroup/glTF), a
> relatively new 3D file format standard tailored for the Web. glTF is like the
> JPG of 3D models.

<a href="https://glitch.com/~aframe-school-gltf-model" target="_blank">Remix Lesson on Glitch</a>  <!-- .element: class="cta-button glitch" -->

1. Add the `https://cdn.aframe.io/test-models/models/virtualcity/VC.gltf` to
the `<a-asset-item id="cityModel">`'s `src` attribute to preload the model
2. Add `#cityModel` to the `<a-gltf-model>`'s `src` attribute to set and add the model

<img class="stretch" data-src="https://cloud.githubusercontent.com/assets/674727/24275925/63067074-0ff0-11e7-9440-7c855b9ea0fd.png">

<a href="https://aframe-school-gltf-model.glitch.me/solution.html" target="_blank">View Result</a>  <!-- .element: class="cta-button" -->

---

## Add 3D Models &mdash; glTF Model Animations

> Models can come with animations. The model provided above has many animations
> of ships zooming across the city. In the previous Glitch, we've provided a simple
> `play-all-model-animations` component that we can attach to our model to play
> its animations. Continue working from your current Glitch.

1. Include the `animation-mixer` component via a `<script>` in the
`<head>` after the A-Frame script. This component is currently in the Registry,
and may one day be included with A-Frame. `https://unpkg.com/aframe-extras.animation-mixer@3.4.0/dist/aframe-extras.animation-mixer.js`
2. Attach the `animation-mixer` component to the `<a-gltf-model>` by
setting it via an HTML attribute `animation-mixer`. By default, this will play all
the animations of the model at once.

<img class="stretch" data-src="media/img/gltf.gif">

<a href="https://aframe-school-gltf-model.glitch.me/solution2.html" target="_blank">View Result</a>  <!-- .element: class="cta-button" -->

---

## Add 3D Models &mdash; Uploading 3D Models

> If you have a model of your own, it can be tricky to upload it to a CDN since
> it consists of multiple files that reference each other. So far the easiest
> way we've found is to dump them into a GitHub repo, publish the repo's master
> branch to GitHub Pages, and use `rawgit.com` to serve them. Alternatively,
> set up Amazon S3. More to come.

------

## Add Tracked Controls &mdash; Add Hand Controls

> Tracked hand controls provide immersion and interactivity with hand
> controllers. In the following Glitch, we've pre-recorded hand control
> movements and button presses with [A-Frame Motion
> Capture](https://github.com/dmarcos/aframe-motion-capture-components).
> Now we just have to add the hands and handle the interaction events.

<a href="https://glitch.com/~aframe-school-hand-controls" target="_blank">Remix Lesson on Glitch</a>  <!-- .element: class="cta-button glitch" -->

1. Find `<a-entity id="left">` and add the [hand-controls component](https://aframe.io/docs/0.5.0/components/hand-controls.html)
configured to the left hand (`hand-controls="left"`)
2. Find `<a-entity id="right">` and add the hand-controls component
configured to the right hand (`hand-controls="right"`)
3. View the result and see the hands moving with pre-recorded motions

<img class="stretch" data-src="media/img/trackedcontrols.gif">

<a href="https://aframe-school-hand-controls.glitch.me/solution.html" target="_blank">View Result</a>  <!-- .element: class="cta-button" -->

---

## Add Tracked Controls &mdash; Add Interactivity

> There are many components to add interactivity to hand controls.
> [controller-cursor](https://github.com/bryik/aframe-controller-cursor-component),
> [aabb-collider +
> grab](https://github.com/aframevr/aframe/tree/master/examples/showcase/tracked-controls/components),
> [super-hands](https://github.com/wmurphyrd/aframe-super-hands-component). For
> this lesson, we'll use controller-cursor that acts as a pointing laser for
> each hand. Continue from your previous Glitch.

1. Add `controller-cursor` component to both hands
2. In the `controller-event-handler` component, change the color of the boxes
when they are hovered over with the `mouseenter` event, and restore the color
with the `mouseleave` event

<img class="stretch" data-src="media/img/trackedcontrols2.gif">

<a href="https://aframe-school-hand-controls.glitch.me/solution2.html" target="_blank">View Result</a>  <!-- .element: class="cta-button" -->

------


<!-- Lessons end here. -->


## Поздравления!

Вы закончили школу A-Frame и теперь получили виртуальную несертифицированную
степень по WebVR.

<img class="stretch" data-src="https://cdn.hackaday.io/images/4174761433219325627.png">

Обратитесь к [документации](https://aframe.io/docs/), чтобы получить больше знаний и стать
мастером.
