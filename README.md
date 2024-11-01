# позиционирование ( position )
- static — значение по умолчанию, элемент позиционируется в соответствии с его местом в потоке документа;
- relative — элемент позиционируется относительно своего исходного положения в потоке документа(остальные блоки считают что блок не передвигался). Используется так же для ограничения дочернего блока absolute;
- absolute — элемент позиционируется относительно ближайшего родительского элемента, который имеет позиционирование, отличное от static.
   - При включении свойства рядом стоящие блоки теряют этот элемент и стремяться занять его место.;
   - если элемент не ограничен другим ( relative ), то он позиционируется по окну браузера. иначе по блоку который его ограничивает;
- fixed — элемент позиционируется относительно окна браузера;
    - При использовании этого значения также можно задать параметры top, bottom, left и right, чтобы определить точное местоположение элемента.
    - left и right смещают блок по окну браузера.
    - top, bottom
- sticky — прилипающий элемент остаётся на месте при прокрутке страницы, но при этом может быть отодвинут от своей стандартной позиции.
    - если не указаны top, right, bottom или left, то ведет себя как static.
    - Sticky начинает себя вести как обычный элемент при прокурутке сайта до тех пор, пока не достигнет определенной позиции на странице, которую вы зададите с помощью свойства **top, right, bottom или left.
      Как только элемент достигнет этой позиции при прокрутке страницы, он зафиксируется на месте и будет оставаться там до тех пор, пока пользователь не доскроллит страницу обратно
 # z-index слои 
 z-index: число | auto | inherit
Любые позиционированные элементы на веб-странице могут накладываться друг на друга в определенном порядке, имитируя тем самым третье измерение, перпендикулярное экрану. 
Каждый элемент может находиться как ниже, так и выше других объектов веб-страницы, их размещением по z-оси и управляет z-index. 
Это свойство работает только для элементов, у которых значение position задано как absolute, fixed или relative.
 
