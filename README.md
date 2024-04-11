# nfactorial
1. tengri.html. tengri2.html две главные страницы, где style.css это стилизация этих двух страниц
2. page1,2,3,4,5,6.html страницы с детальной информацией статей и style2.css стилизация этих страниц.
3. Остальные фота были использованы для дизайна
4. Пагинация страниц в конце каждой страницы:
   <div class="pagination">
            <a href="tengri.html">&laquo;</a>
            <a  href="tengri.html">1</a>
            <a class="active" href="#">2</a>
            <a href="#">&raquo;</a>
          </div>
          <br></br>
5. Фильтрация делит новости на областные (Astana, Atyrau, Aktobe)
6. Поиск ищет новости по ключевым словам
7. JS был использован внутри кода, но сам код для фильтрации и поиска не корректно работает




<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tengri News </title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header>
        <h1>Tengri News</h1>
        <nav>
            <ul>
                <a class="header_tengri-rubrics_item news active" href="tengri.html">NEWS</a>
                <a class="header_tengri-rubrics_item life" href="/mixnews/">LIFE</a>
                <a class="header_tengri-rubrics_item sport" href="https://tengrisport.kz/">SPORT</a>
                <a class="header_tengri-rubrics_item travel" href="https://tengritravel.kz/">TRAVEL</a>
                <a class="header_tengri-rubrics_item guide" href="/tengriguide/">GUIDE</a>
                <a class="header_tengri-rubrics_item edu" href="/tengri-education/">EDU</a>
                <a class="header_tengri-rubrics_item auto" href="https://tengriauto.kz/">AUTO</a>
            </ul>
        
        </nav>
    </header>
    <main>
        <form id="searchForm">
            <input type="text" id="searchInput" placeholder="Search...">
            <button type="submit">Search</button>
        </form> 
        <nav id="categories">
            <button data-category="all" class="active btn" onclick="filterSelection('all')">All</button>
            <button data-category="news"  class="btn" onclick="filterSelection('Atyrau')">Atyrau</button>
            <button data-category="life"  class="btn" onclick="filterSelection('Astana')">Astana</button>
            <button data-category="sport"  class="btn" onclick="filterSelection('Aktobe')">Aktobe</button>
        </nav>
        <section id="news">
            <div id="news" class="container">
                <h1>Последние новости</h1>
                <div class="columns">
                    <div class="column">
                        <div class="news filterDiv Astana">
                            <a href="page1.html"><img src="photo1.png" width="400", height="200"></a>
                            <h2>Материальный резерв разбронирован: спецтехнику направили в пострадавшие регионы</h2>
                            <span>
                                Сегодня  21:41 
                    <span>
                        <span class="content_item_meta_viewings">
                            <img src="view.svg">
                            <span class="tn-text-preloader-dark"
                                  data-views=""
                                  data-id="531330"
                                  data-type="news"
                                  data-lang="ru"
                                  data-travel=""></span>
                        </span>
                        <span class="content_item_meta_comments">
                            <img src="comments.svg">
                            <span class="tn-text-preloader-dark"
                                  data-comments=""
                                  data-id="531330"
                                  data-type="news"
                                  data-lang="ru"></span>
                        </span>
                    </span>    
                        </div>
                        <div class="news filterDiv Astana">
                            <a href="page2.html"><img src="photo2.jpeg" width="400", height="200"></a>
                            <h2>Уровень перелива на водохранилище в СКО стремительно приближается к историческому максимуму</h2>
                            <p>Текст новости 2</p>
                            <span>
                                Сегодня  20:40 
                    <span>
                        <span class="content_item_meta_viewings">
                            <img src="view.svg">
                            <span class="tn-text-preloader-dark"
                                  data-views=""
                                  data-id="531330"
                                  data-type="news"
                                  data-lang="ru"
                                  data-travel=""></span>
                        </span>
                        <span class="content_item_meta_comments">
                            <img src="comments.svg">
                            <span class="tn-text-preloader-dark"
                                  data-comments=""
                                  data-id="531330"
                                  data-type="news"
                                  data-lang="ru"></span>
                        </span>
                    </span>    
                        </div>
                        <div class="news filterDiv Aktobe">
                            <a href="page3.html"><img src="photo3.jpeg" width="400", height="200"></a>
                            <h2>Паводки в Казахстане: Генпрокуратура заявила о начатых расследованиях в 3 областях</h2>
                            <span>
                                Сегодня  19:18 
                    <span>
                        <span class="content_item_meta_viewings">
                            <img src="view.svg">
                            <span class="tn-text-preloader-dark"
                                  data-views=""
                                  data-id="531330"
                                  data-type="news"
                                  data-lang="ru"
                                  data-travel=""></span>
                        </span>
                        <span class="content_item_meta_comments">
                            <img src="comments.svg">
                            <span class="tn-text-preloader-dark"
                                  data-comments=""
                                  data-id="531330"
                                  data-type="news"
                                  data-lang="ru"></span>
                        </span>
                    </span> 
                        </div>
                    </div>
                    <div class="column">
                        <div class="news filterDiv Aktobe">
                            <a href="page4.html"><img src="photo4.jpeg" width="400", height="200"></a>
                            <h2>Паводки в Казахстане: что происходит на водохранилищах страны</h2>
                            <span>
                                Сегодня 18:49 
                    <span>
                        <span class="content_item_meta_viewings">
                            <img src="view.svg">
                            <span class="tn-text-preloader-dark"
                                  data-views=""
                                  data-id="531330"
                                  data-type="news"
                                  data-lang="ru"
                                  data-travel=""></span>
                        </span>
                        <span class="content_item_meta_comments">
                            <img src="comments.svg">
                            <span class="tn-text-preloader-dark"
                                  data-comments=""
                                  data-id="531330"
                                  data-type="news"
                                  data-lang="ru"></span>
                        </span>
                    </span> <br><br>
                        </div>
                        <div class="news filterDiv Atyrau">
                            <a href="page5.html"><img src="photo5.jpeg" width="400", height="200"></a>
                            <h2>В Атырау объявят режим ЧС</h2>
                            <span>
                                Сегодня 17:00
                    <span>
                        <span class="content_item_meta_viewings">
                            <img src="view.svg">
                            <span class="tn-text-preloader-dark"
                                  data-views=""
                                  data-id="531330"
                                  data-type="news"
                                  data-lang="ru"
                                  data-travel=""></span>
                        </span>
                        <span class="content_item_meta_comments">
                            <img src="comments.svg">
                            <span class="tn-text-preloader-dark"
                                  data-comments=""
                                  data-id="531330"
                                  data-type="news"
                                  data-lang="ru"></span>
                        </span>
                    </span> <br><br> <br><br> <br><br><br>
                        </div>
                        <div class="news filterDiv Atyrau">
                            <a href="page6.html"><img src="photo6.jpeg" width="400", height="200"></a>
                            <h2>Даю поручение разбронировать государственный материальный резерв - Токаев</h2>
                            <span>
                                Сегодня 13:16
                    <span>
                        <span class="content_item_meta_viewings">
                            <img src="view.svg">
                            <span class="tn-text-preloader-dark"
                                  data-views=""
                                  data-id="531330"
                                  data-type="news"
                                  data-lang="ru"
                                  data-travel=""></span>
                        </span>
                        <span class="content_item_meta_comments">
                            <img src="comments.svg">
                            <span class="tn-text-preloader-dark"
                                  data-comments=""
                                  data-id="531330"
                                  data-type="news"
                                  data-lang="ru"></span>
                             </span>
                         </span>
                    </div>
                </div>
            </div>
        </section>
        <div class="pagination">
            <a href="#">&laquo;</a>
            <a class="active" href="#">1</a>
            <a href="tengri2.html">2</a>
            <a href="tengri2.html">&raquo;</a>
          </div>
          <br></br>
        
    </main>
    <footer>
        <p>&copy; 2024 Tengri News</p>
    </footer>
    <script >
      
      filterSelection("all")
function filterSelection(c) {
  var x, i;
  x = document.getElementsByClassName("filterDiv");
  if (c == "all") c = "";
  for (i = 0; i < x.length; i++) {
    w3RemoveClass(x[i], "show");
    if (x[i].className.indexOf(c) > -1) w3AddClass(x[i], "show");
  }
}

function w3AddClass(element, name) {
  var i, arr1, arr2;
  arr1 = element.className.split(" ");
  arr2 = name.split(" ");
  for (i = 0; i < arr2.length; i++) {
    if (arr1.indexOf(arr2[i]) == -1) {element.className += " " + arr2[i];}
  }
}

function w3RemoveClass(element, name) {
  var i, arr1, arr2;
  arr1 = element.className.split(" ");
  arr2 = name.split(" ");
  for (i = 0; i < arr2.length; i++) {
    while (arr1.indexOf(arr2[i]) > -1) {
      arr1.splice(arr1.indexOf(arr2[i]), 1);     
    }
  }
  element.className = arr1.join(" ");
}

// Add active class to the current button (highlight it)
var btnContainer = document.getElementById("myBtnContainer");
var btns = btnContainer.getElementsByClassName("btn");
for (var i = 0; i < btns.length; i++) {
  btns[i].addEventListener("click", function(){
    var current = document.getElementsByClassName("active");
    current[0].className = current[0].className.replace(" active", "");
    this.className += " active";
  });
}
    </script>
</body>
</html>
