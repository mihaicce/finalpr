<template>
<div class="background"></div>
    <div class="background-texture"></div>

    <section class="carousel">
      <h2 class="categories__title">SERVICII</h2>
      <div class="carousel__container">
        <div class="carousel-item">
          <img
            class="carousel-item__img"
            src="../assets/slide2.jpg"
            alt="implant"
          />
          <div class="carousel-item__details">
            <h5 class="carousel-item__details--title">Implantologie</h5>
            <h6 class="carousel-item__details--subtitle">Un implant dentar este o procedură chirurgicală utilizată pentru a înlocui un dinte lipsă sau deteriorat. Este o metodă modernă și eficientă de înlocuire a unui dinte natural. Un implant dentar constă în plasarea unui șurub din titan sau aliaj de titan în osul maxilar sau mandibular, care va acționa ca o rădăcină artificială. După integrarea implantului în os (osseointegrare), acesta servește ca suport pentru montarea unei coroane dentare artificiale, oferind astfel o soluție durabilă și estetică pentru înlocuirea unui dinte natural lipsă.</h6>
          </div>
        </div>
        <div class="carousel-item">
          <img
            class="carousel-item__img"
            src="../assets/brackets.jpg"
            alt="people"
          />
          <div class="carousel-item__details">
            <h5 class="carousel-item__details--title">Ortodontie</h5>
            <h6 class="carousel-item__details--subtitle">Date and Duration</h6>
          </div>
        </div>
        <div class="carousel-item">
          <img
            class="carousel-item__img"
            src="../assets/endo.jpg"
            alt="people"
          />
          <div class="carousel-item__details">
            <div class="controls">
              <span class="fas fa-play-circle"></span>
              <span class="fas fa-plus-circle"></span>
            </div>
            <h5 class="carousel-item__details--title">Endodontie</h5>
            <h6 class="carousel-item__details--subtitle">Date and Duration</h6>
          </div>
        </div>
        <div class="carousel-item">
          <img
            class="carousel-item__img"
            src="../assets/protetica.jpg"
            alt="people"
          />
          <div class="carousel-item__details">
            <div class="controls">
              <span class="fas fa-play-circle"></span>
              <span class="fas fa-plus-circle"></span>
            </div>
            <h5 class="carousel-item__details--title">Protetica</h5>
            <h6 class="carousel-item__details--subtitle">Date and Duration</h6>
          </div>
        </div>
        <div class="carousel-item">
          <img
            class="carousel-item__img"
            src="../assets/paro.jpg"
            alt="people"
          />
          <div class="carousel-item__details">
            <div class="controls">
              <span class="fas fa-play-circle"></span>
              <span class="fas fa-plus-circle"></span>
            </div>
            <h5 class="carousel-item__details--title">Parodontologie</h5>
            <h6 class="carousel-item__details--subtitle">Date and Duration</h6>
          </div>
        </div>
      </div>
    </section>
</template>

<style scoped>
body {
  margin: 0;
  font-family: 'Muli', sans-serif;
  -webkit-box-sizing: border-box;
  box-sizing: border-box;
  overflow-x: hidden;
}

/* .background {
  background: url('https://images.pexels.com/photos/1095624/pexels-photo-1095624.jpeg?auto=compress&cs=tinysrgb&h=750&w=1260')
    center top no-repeat #252746;
  background-size: cover;
  display: block;
  width: 100%;
  height: 1000px;
  position: absolute;
  z-index: 0;
  top: 0;
  left: 0;
} */

/* .background-texture {
  background: -webkit-gradient(
    linear,
    left bottom,
    left top,
    from(#0f0140e6),
    to(rgba(255, 214, 117, 0.9))
  );
  background: linear-gradient(to top, #0f0140e6, rgba(255, 214, 117, 0.9));
  background-size: cover;
  width: 100%;
  height: 1000px;
  position: absolute;
  z-index: 0;
  top: 0;
  left: 0;
} */

.carousel {
  width: 100%;
  overflow-x: scroll;
  padding: 30px;
  padding-top: 80px;
  position: relative;
  -webkit-box-sizing: border-box;
  box-sizing: border-box;
}

.carousel__container {
  white-space: nowrap;
  margin: 70px 0px;
  padding-bottom: 10px;
  display: inline-block;
}

.categories__title {
  color: black;
  font-size: 30px;
  /* position: absolute; */
  text-align: center;
  /* padding-left: 30px; */
}

.carousel-item {
  width: 200px;
  height: 250px;
  border-radius: 20px;
  background-color: #95bcd6;
  overflow: hidden;
  margin-right: 10px;
  margin-top: 70px;
  display: inline-block;
  cursor: pointer;
  -webkit-transition: 1000ms all;
  transition: 1000ms all;
  -webkit-transform-origin: center left;
  transform-origin: center left;
  position: relative;
}

.carousel-item:hover ~ .carousel-item {
  -webkit-transform: translate3d(100px, 0, 0);
  transform: translate3d(100px, 0, 0);
}

.carousel__container:hover .carousel-item {
  opacity: 0.5;
}

.carousel__container:hover .carousel-item:hover {
  -webkit-transform: scale(1.5);
  transform: scale(1.5);
  opacity: 1;
}

.carousel-item__img {
  width: 200px;
  height: 250px;
  -o-object-fit: cover;
  object-fit: cover;
}

.carousel-item__details {
  background: -webkit-gradient(
    linear,
    left bottom,
    left top,
    from(rgba(0, 0, 0, 0.9)),
    to(rgba(0, 0, 0, 0))
  );
  background: linear-gradient(
    to top,
    rgba(0, 0, 0, 0.9) 0%,
    rgba(0, 0, 0, 0) 100%
  );
  font-size: 10px;
  opacity: 0;
  -webkit-transition: 450ms opacity;
  transition: 450ms opacity;
  padding: 10px;
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
}

.carousel-item__details:hover {
  opacity: 1;
}

.carousel-item__details span {
  width: 10px;
  height: 10px;
  font-size: 0.9rem;
  color: #2ecc71;
  background-color: white;
}

/* .carousel-item__details h6 {
  font-size: 0.6rem;
} */

.carousel-item__details .controls {
  padding-top: 180px;
}

.carousel-item__details .carousel-item__details--title,
.carousel-item__details--subtitle {
  color: #fff;
  margin: 5px 0;
}
</style>