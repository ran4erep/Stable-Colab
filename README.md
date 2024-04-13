<h1 align="center">Всем привет, меня зовут <a href="https://ran4erep.github.io" target="_blank">Вадим</a>!
<img src="https://github.com/ran4erep/ran4erep.github.io/blob/master/img/Hi.gif" height="32"/></h1>
<h3 align="center">А это мой Python скрипт для того чтобы работать с нейросетью Stable Diffusion через сервис Google Colaboratory без платной подписки.</h3>

<a href="https://colab.research.google.com/github/ran4erep/Stable-Colab/blob/main/Stable_Diffusion.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Открыть в Колабе"/></a> Русская версия
<br><br>
<a href="https://colab.research.google.com/github/ran4erep/Stable-Colab/blob/main/Stable_Diffusion_English.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a> English version

<h3 align="right"><a href="https://git.io/typing-svg"><img src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&pause=1000&color=247EA6&random=false&width=435&lines=Tensors+must+flow..." alt="Typing SVG" /></a></h3>

The English version of the manual is located below the Russian version.

<h2>Инструкция по началу использования скрипта:</h2>
<br>Видео-инструкция:<br>
<a href="https://www.youtube.com/embed/klMvuBeYGIU?si=ipb0xSfkFhl1E7wS" target="_blank"><img src="https://github.com/ran4erep/ran4erep.github.io/blob/master/test/sd_play.jpg" alt="IMAGE ALT TEXT HERE" width="320" height="180" border="10"></a>
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
    <dt>1.5.0 - Добавлена возможность использования моделей с сайта CivitAI. Оперативной памяти Google Colab хватает только на конвертацию 1.5/2.0 моделей, так что XL модели с CivitAI вы использовать не сможете, даже и не пытайтесь. Также добавлена очистка видеопамяти перед каждой генерацией изображения, следовательно ошибок "cuda out of memory" станет меньше.</dt>
    <dd><ul>
      <li>1.5.1 - Добавлена возможность использовать LoRA модели с сайта CivitAI. Мелкие фиксы связанные с добавлением LoRA моделей.</li>
      <li>1.5.2 - Добавлена поддержка параметра CLIP skip. Исправлена перезагрузка и переконвертация моделей с CivitAI при смене параметров, а также исправлены мелкие баги. Создана отдельная англоязычная версия скрипта.</li>
      <li>1.5.3 - Дообавлена возможность писать промпты на любых языках. Немного переделан вывод промпта при генерации. Исправлены различные баги.</li>
      <li>1.5.4 - Добавлена возможность генерировать несколько изображений в режимах image2image и inpainting.</li>
      <li>1.5.5 - В список заранее заготовленных моделей были добавлены две модели для режима Inpainting. Немного облагородил блоки с загрузкой изображений для режимов Img2Img и Inpainting. Добавлена возможность выключать веса токенов (для совместимости, так как, к примеру, модель Kandinsky Inpainting выдаёт ошибку с включенными весами).</li>
    </ul></dd>
</dl>

<h2>English version:</h2>

Go to the <a href="https://colab.research.google.com">Google Colab</a> website and import the Stable_Diffusion_English.ipynb file by clicking <b>File --> Open Notepad --> Upload</b>
<br><br>
...or use the "Open in Colab" button just above on this page and the secret magic will open Colab right away with the desired notepad. ✨

<p>Make sure that your session will be handled by the video card by clicking <b>Runtime Environment --> Change Runtime Environment --> T4 GPU</b>.
  <img src="https://github.com/ran4erep/ran4erep.github.io/blob/master/img/gpu.png" height="256" align="right" /></p>
<br>
Then all you have to do is just run blocks of code sequentially and eventually you'll end up generating your kitties (or whatever it is that people usually generate with neural networks). It is desirable to have some experience with a Stable Diffusion web interface. If you are a beginner, try generating images on free services like <a href="https://playgroundai.com">playgroundai.com</a>. And when you understand what SD models there are, how Stable Diffusion and its tokens are organized, what are the settings and how they affect the generation of images, it will be easier to use this script and you will feel yourself like a fish in water. 🐟💦
<br><br>

<h3>If you have any suggestions on how to edit this README file, if you want to report bugs in the script or if you have any other questions, then write to me on E-Mail <a href="mailto:r4darksoulii@gmail.com">r4darksoulii@gmail.com</a>.</h3>

<h4>If you want to support me, buy me a cup of coffee, ☕ https://www.buymeacoffee.com/ran4erep <br> would be much appreciated. :)</h4>

<br>
<br>
<dl>
  <dt>1.0.0 - First version of the script.</dt>
  <dt>1.1.0 - Added user interface. Now you don't even need to know what variables are in Python. 🙌</dt>
    <dd><ul>
      <li>1.1.1 - Minor fixes and interface improvements.</li>
      <li>1.1.2 - Added an aspect ratio calculator and merged SD installation with Google Drive connection.</li>
    </ul></dd>
  <dt>1.2.0 - Added generation of multiple images at one time.</dt>
      <dd><ul>
        <li>1.2.1 - Added prompt weights, redesigned mechanism for saving images to Google Drive, minor fixes.</li>
        <li>1.2.2 - Added the ability to connect LoRA models.</li>
        <li>1.2.3 - Images in Google Drive are now saved in folders with the current date name, and the time of generation is added to the file name.</li>
      </ul></dd>
  <dt>1.3.0 - Scheduler selection moved to the "Pipeline Customization" block, because when changing it on a running model, RAM consumption increases enormously due to reloading of other components of the Pipeline into it. Style selection has been added. Styles are pre-prepared prompts that create a particular style.</dt>
  <dd><ul>
    <li>1.3.1 - Minor fixes. An error was occurring when saving a file to Google Drive with a long prompt.</li>
    <li>1.3.2 - The speed of script installation has been increased. Now it is installed for ~30 seconds.</li>
    <li>1.3.3 - Added real-time diffusion display. The number of "#" characters in generation information is now equal to the length of the longest string.</li>
  </ul></dd>
  <dt>1.4.0 - Added support for image2image.</dt>
    <dd><ul>
      <li>1.4.1 - Added support for Inpainting. Slightly redesigned interface. Fixed several bugs.</li>
      <li>1.4.2 - Fixed a lot of bugs, including critical bugs with Inpainting. Completely redesigned the basic principle of the script: now there is only one pipline for all modes of operation, it saves Colab's resources. Added function of displaying the list of models loaded during the session.</li>
    </ul></dd>
    <dt>1.5.0 - Added ability to use models from CivitAI website. Google Colab's RAM is only enough to convert 1.5/2.0 models, so you can't use XL models from CivitAI, don't even try. Also added clearing of video memory before each image generation, hence "cuda out of memory" errors will be fewer.</dt>
    <dd><ul>
      <li>1.5.1 - Added ability to use LoRA models from CivitAI site. Minor fixes related to adding LoRA models.</li>
      <li>1.5.2 - Added support for CLIP skip parameter. Fixed reloading and reconversion of models with CivitAI when changing parameters, and also fixed minor bugs. Created a separate English version of the script.</li>
    </ul></dd>
</dl>
