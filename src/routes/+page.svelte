<style>
    :root {
    --primary-color: rgb(251, 207, 246);
    --secodary-color: rgb(246, 221, 190);
}

* {
    box-sizing:  border-box;
}

main {
    display: flex;
    flex-wrap: wrap;
}

body{
    background-color:  var(--primary-color);
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    margin: 0;
}

header {
    padding: 10px;
    display: flex;
    justify-content: flex-end;
    background-color: var(--secodary-color);
}

.search {
    background-color: transparent;
    border: 2px solid var(--primary-color);
    border-radius: 50px;
    font-family: inherit;
    font-size: 14px;
    padding: 20px 10px;
}

.search::placeholder {
    color: wheat;
}

.search.search:focus{
    outline: none;
    background-color: white;
}

.movie {
    width: 300px;
    margin: 10px;
    background-color: var(--secodary-color);
    box-shadow: 0 4px 5px rgba(0, 0, 0, 0.2);
    position: relative;
    overflow: hidden;
    border-radius: 3px;
}


.movie-info img {
    width: 120%;
}

.movie-info {
    color: black;
    display: flex;
    flex-direction: column; 
    align-items: center;
    justify-content: space-between;
    padding: 20px 30px 30px;
    letter-spacing: 0.5px;
}

.movie-info h3{
    margin-top: 25px; 
}

.movie-info span{
    background-color: var(--primary-color);
    padding: 2px 3px;
    border-radius: 4px;
    font-weight: bold;
}

.movie-info span.green{
    color: rgb(213, 44, 44);
}

.overview {
    background-color: white;
    padding: 20px;
    position: absolute;
    left: 0;
    bottom: 0;
    right: 0;
    max-width: 100%;
    transform: translateY(101%);
    transition: transform 0.3s ease-in;
}

.movie:hover .overview{
    transform: translateY(0)
}

</style>
<h1>Сейчас в кино:</h1>
<main id="main">
 
    <div class="movie" id="movie">
        <div class="movie-info" id="MovieInfoDiv">
            <img src="https://w.forfun.com/fetch/5d/5dfb102df079c1780a4675cbdfb4162c.jpeg" alt="">
            <h3 id="MovieTitle">Легенда
            <span class="green">9.8</span></h3>
        </div>
        <div class="overview">
            <h3 id="Description">Гангстеры-близнецы завоевывают Лондон 1960-х. 
                Драма о знаменитых преступниках с двойной ролью Тома Харди</h3>
        </div>
    </div>
    <div class="movie" id="movie">
        <div class="movie-info" id="MovieInfoDiv">
            <img src="/src/lib/images/lyl.jpg" alt="">
            <h3 id="MovieTitle">Лулу и Бриггс <span class="green">8.4</span></h3>
        </div>
        <div class="overview">
            <h3 id="Description">Рейнджер Бриггс получает необычное задание от армейского руководства – отвезти боевую собаку 
                по кличке Лулу к семье её погибшего хозяина-сержанта.</h3>
        </div>
    </div>
    <div class="movie" id="movie">
        <div class="movie-info" id="MovieInfoDiv">
            <img src="/src/lib/images/dom.jpg" alt="">
            <h3 id="MovieTitle">Дом странных детей Мисс Перегрин <span class="green">7.8</span></h3>
        </div>
        <div class="overview">
            <h3 id="Description">16-летний Джейкоб получает загадочное письмо и отправляется на остров, где вырос его дед. Там он находит детей, 
                которых раньше видел только на фотографиях.</h3>
        </div>
    </div>
    <div class="movie" id="movie">
        <div class="movie-info" id="MovieInfoDiv">
            <img src="/src/lib/images/led.jpg" alt="">
            <h3 id="MovieTitle">Лед 3<span class="green">5.9</span></h3>
        </div>
        <div class="overview">
            <h3 id="Description">Надя выросла и стала фигуристкой. Она мечтает о «Кубке Льда»,
                 как когда-то мечтала ее мама</h3>
        </div>
    </div>
    <div class="movie" id="movie">
        <div class="movie-info" id="MovieInfoDiv">
            <img src="/src/lib/images/do vstrechi.jpg" alt="">
            <h3 id="MovieTitle">До встречи с тобой<span class="green">8.7</span></h3>
        </div>
        <div class="overview">
            <h3 id="Description">Лу не знает, что вот-вот потеряет свою работу и 
                что в ближайшем будущем ей понадобятся все силы, чтобы преодолеть свалившиеся на нее проблемы.</h3>
        </div>
    </div>
    <div class="movie" id="movie">
        <div class="movie-info" id="MovieInfoDiv">
            <img src="/src/lib/images/matriz.jpg" alt="">
            <h3 id="MovieTitle">Матрица времени<span class="green">6.7</span></h3>
        </div>
        <div class="overview">
            <h3 id="Description"> Саманта оказалась в заколдованном круге проклятого дня, и теперь она вынуждена проживать ужас той пятницы снова и снова. Чтобы распутать петлю времени, 
                она должна вычислить ошибку и исправить неверный шаг. </h3>
        </div>
    </div>
    <div class="movie" id="movie">
        <div class="movie-info" id="MovieInfoDiv">
            <img src="/src/lib/images/mast.png" alt="">
            <h3 id="MovieTitle">Мастер и Маргарита <span class="green">9.0</span></h3>
        </div>
        <div class="overview">
            <h3 id="Description">Москва, 1930-е годы. Популярный драматург обвиняется в антисоветчине: спектакль по его пьесе отменяют,
                 а самого его выгоняют из союза литераторов. </h3>
        </div>
    </div>
    <div class="movie" id="movie">
        <div class="movie-info" id="MovieInfoDiv">
            <img src="/src/lib/images/mstiteli.jpg" alt="">
            <h3 id="MovieTitle">Мстители. Финал <span class="green">6.9</span></h3>
        </div>
        <div class="overview">
            <h3 id="Description">Оставшиеся в живых члены команды Мстителей и их союзники должны разработать новый план, который поможет
                 противостоять разрушительным действиям могущественного титана Таноса.</h3>
        </div>
    </div>
    <div class="movie" id="movie">
        <div class="movie-info" id="MovieInfoDiv">
            <img src="/src/lib/images/kry'l.jfif" alt="">
            <h3 id="MovieTitle">Круэлла <span class="green">7.8</span></h3>
        </div>
        <div class="overview">
            <h3 id="Description">Великобритания, 1960-е годы. Эстелла была необычным ребёнком, 
                и особенно трудно ей было мириться со всякого рода несправедливостью. </h3>
        </div>
    </div>
</main>
