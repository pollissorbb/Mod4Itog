<style>
    :root {
    --primary-color: rgb(119, 200, 206);
    --secodary-color: rgb(131, 183, 204);
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
    color: rgb(88, 202, 187);
}

.search.search:focus{
    outline: none;
    background-color: rgb(201, 141, 141);
}

.movie {
    width: 300px;
    margin: 10px;
    background-color: var(--secodary-color);
    box-shadow: 0 4px 5px rgba(204, 101, 218, 0.637);
    position: relative;
    overflow: hidden;
    border-radius: 3px;
}

.movie img{
    width: 100%;
}

.movie-info {
    color: rgb(152, 111, 180);
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 20px 30px 30px;
    letter-spacing: 0.5px;
}

.movie-info h3{
    margin-top: 0;
}

.movie-info span{
    background-color: var(--primary-color);
    padding: 25px 5px;
    border-radius: 3px;
    font-weight: bold;
}

.movie-info span.green{
    color: rgb(149, 76, 197);
}

.overview {
    background-color: rgb(214, 148, 176);
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

<main id="main">
    <div class="movie" id="movie">
        <div class="movie-info" id="MovieInfoDiv">
            <h3 id="MovieTitle">1+1</h3>
            <span class="green">8.8</span>
        </div>
        <div class="overview">
            <h3 id="Description">2011, Франция, драма</h3>
        </div>
    </div>
    <div class="movie" id="movie">
        <div class="movie-info" id="MovieInfoDiv">
            <h3 id="MovieTitle">Унесённые призраками</h3>
            <span class="green">8.5</span>
        </div>
        <div class="overview">
            <h3 id="Description">2001, Япония, аниме</h3>
        </div>
    </div>
    <div class="movie" id="movie">
        <div class="movie-info" id="MovieInfoDiv">
            <h3 id="MovieTitle">Ходячий замок</h3>
            <span class="green">8.3</span>
        </div>
        <div class="overview">
            <h3 id="Description">2004, Япония, аниме</h3>
        </div>
    </div>
    <div class="movie" id="movie">
        <div class="movie-info" id="MovieInfoDiv">
            <h3 id="MovieTitle">Как приручить дракона</h3>
            <span class="green">8.2</span>
        </div>
        <div class="overview">
            <h3 id="Description">2010, США, мультфильм</h3>
        </div>
    </div>
    <div class="movie" id="movie">
        <div class="movie-info" id="MovieInfoDiv">
            <h3 id="MovieTitle">Тайна Коко</h3>
            <span class="green">8.7</span>
        </div>
        <div class="overview">
            <h3 id="Description">2017, США, мультфильм</h3>
        </div>
    </div>
</main>