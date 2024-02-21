<h1 align="center">Всем привет, меня зовут <a href="https://ran4erep.github.io" target="_blank">Вадим</a>!
<img src="https://github.com/ran4erep/ran4erep.github.io/blob/master/img/Hi.gif" height="32"/></h1>
<h3 align="center">А это мой Python скрипт для того чтобы работать с нейросетью Stable Diffusion через сервис Google Colaboratory без платной подписки.</h3>

<a href="https://colab.research.google.com/github/ran4erep/Stable-Colab/blob/main/Stable_Diffusion.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Открыть в Колабе"/></a>

<h3 align="right"><a href="https://git.io/typing-svg"><img src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&pause=1000&color=247EA6&random=false&width=435&lines=Tensors+must+flow..." alt="Typing SVG" /></a></h3>

<h2>Инструкция по началу использования скрипта:</h2>
<br>Видео-инструкция:<br>
<a href="https://www.youtube.com/embed/VQ3YvX0-9wQ?si=KLlCkihAdpZX4qoM" target="_blank"><img src="https://github.com/ran4erep/ran4erep.github.io/blob/master/test/sd_play.jpg" alt="IMAGE ALT TEXT HERE" width="320" height="180" border="10"></a>
<br>
<br>

Зайдите на сайт <a href="https://colab.research.google.com">Google Colab</a>  и импортируйте файл Stable_Diffusion.ipynb нажав <b>Файл --> Открыть блокнот --> Загрузить</b>
<br><br>
...либо воспользуйтесь кнопкой "Open in Colab", которая находиться чуть выше на этой странице и тайное волшебство откроет Колаб сразу с нужным блокнотом. ✨

<p>Убедитесь что ваш сеанс будет обрабатываться при помощи видеокарты, нажав <b>Среда выполнения --> Сменить среду выполнения --> T4 GPU</b>.
  <img src="https://github.com/ran4erep/ran4erep.github.io/blob/master/img/gpu.png" height="256" align="right" /></p>
<br>
Далее всё что вам остаётся так это просто последовательно запускать блоки кода и в конце концов вы всё таки сгененрируете своих котиков (или что там обычно генерируют люди при помощи нейросетей). Желательно иметь какой-нибудь опыт работы с веб-интерфейсом Stable Diffusion. Если вы новичок, то попробуйте сначала погенерировать изображения на бесплатных сервисах по типу <a href="https://playgroundai.com">playgroundai.com</a>. А когда вы разберётесь с тем какие вообще модели SD бывают, как устроен Stable Diffusion и его токены, какие есть настройки и как они влияют на генерацию изображений, вам станет легче пользоваться данным скриптом и вы будете чувствовать себя как рыба в воде. 🐟💦
<br><br>

<h3>Если у вас есть предложения по правке данного README файла, если вы хотите сообщить о багах в скрипте или у вас есть ещё какие-нибудь вопросы, то пишите мне на E-Mail <a href="mailto:r4darksoulii@gmail.com">r4darksoulii@gmail.com</a>.</h3>

<h4>Если хотите меня поддержать, то купите мне чашечку кофе, ☕ https://www.buymeacoffee.com/ran4erep <br> буду очень вам благодарен. :) </h4>

<br>
<br>
<dl>
  <dt>1.0.0 - Первая версия скрипта.</dt>
  <dt>1.1.0 - Добавлен пользовательский интерфейс. Теперь даже не нужно знать что такое переменные в Python. 🙌</dt>
    <dd><ul>
      <li>1.1.1 - Мелкие фиксы и доработка интерфейса.</li>
      <li>1.1.2 - Добавил калькулятор соотношения сторон и объединил установку SD с подключением к Google Drive.</li>
    </ul></dd>
  <dt>1.2.0 - Добавлена генерация нескольких изображений за один раз.</dt>
      <dd><ul>
        <li>1.2.1 - Добавлен вес промптов, переделан механизм сохранения изображений на Google Drive, мелкие фиксы.</li>
        <li>1.2.2 - Добавлена возможность подключать LoRA модели.</li>
        <li>1.2.3 - Теперь изображения в Google Drive сохраняются по папкам с названием текущей даты, а в название файла добавляется время генерации.</li>
      </ul></dd>
  <dt>1.3.0 - Выбор планировщика переехал в блок "Настройка пайплайна", потому что при его смене на работающей моделе колоссально увеличивается потребление оперативной памяти за счёт перезагрузки в неё остальных компонентов пайплайна. Был добавлен выбор стиля. Стили - это заранее заготовленные промпты, которые и создают тот или иной стиль.</dt>
  <dd><ul>
    <li>1.3.1 - Мелкие фиксы. При сохранении файла на Google Drive с длинным промптом возникала ошибка.</li>
    <li>1.3.2 - Увеличена скорость установки скрипта. Теперь он устанавливается ~30 секунд.</li>
    <li>1.3.3 - Добавлено отображение диффузии в реальном времени. Количество символов "#" в информации о генерации теперь равняется длине самой длинной строки.</li>
  </ul></dd>
  <dt>1.4.0 - Добавлена поддержка image2image.</dt>
    <dd><ul>
      <li>1.4.1 - Добавлена поддержка Inpainting. Слегка переделан интерфейс. Исправлено несколько багов.</li>
      <li>1.4.2 - Исправлено множество багов, в том числе критические баги с работой Inpainting. Полностью переделан основной принцип работы скрипта: теперь есть только один пайплайн для всех режимов работы, это экономит ресурсы Колаба. Добавлена функция отображения списка загруженных в течении сессии моделей.</li>
    </ul></dd>
</dl>
