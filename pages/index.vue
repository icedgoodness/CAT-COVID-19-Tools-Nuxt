<template>
  <div class="home-container">
    <app-header1></app-header1>
    <div class="home-middle">
      <div class="home-lines">
        <img
          alt="image"
          src="/playground_assets/line%20dots%20large.svg"
          class="home-line1"
        />
        <img alt="image" src="/playground_assets/line2.svg" class="home-line2" />
        <img alt="image" src="/playground_assets/line3.svg" class="home-line3" />
      </div>
      <div class="home-heading">
        <div class="home-hero">
          <img
            alt="image"
            src="/playground_assets/gadget%20image.svg"
            class="home-image"
          />
          <div class="home-container1">
            <h1 class="home-text">What is CAT Covid-19 ?</h1>
            <h2 class="home-text01">
              <span>
                CAT Covid-19 is a tool to predict covid-19 patients’ mortality
                based on research and validation data that can help mortality risk
                assessment and treatment decision making for patients with
                covid-19
              </span>
            </h2>
            <button class="home-button button">
              <span class="home-text03">Start ➤</span>
            </button>
          </div>
        </div>
      </div>
      <div class="home-circles">
        <div class="home-circle1">
          <span class="home-text04">
            <span class="home-text05"></span>
            <span class="home-text06"></span>
            <span class="home-text07"></span>
            <span class="home-text08">
              CAT Covid-19 predicts covid-19 patients&apos; mortality with two
              different methods; model 1 and model 2. Model 1 is recommended for
              patients with limited resources and Model 2 can be used when
              laboratory data exists.
            </span>
            <br />
            <span></span>
            <span class="home-text10"></span>
          </span>
          <img
            alt="image"
            src="/playground_assets/ellipse%201.svg"
            class="home-image1"
          />
          <span class="home-text11">
            <span class="home-text12">What does CAT</span>
            <br />
            <span class="home-text14">Covid-19 do?</span>
          </span>
        </div>
        <div class="home-circle2">
          <span class="home-text15">
            <span class="home-text16">
              CAT Covid-19 can be used by clinicians, patients and their families
              and significant others. Patients should use it in consultation with
              a medical professional.
            </span>
          </span>
          <img
            alt="image"
            src="/playground_assets/ellipse%201.svg"
            class="home-image2"
          />
          <span class="home-text17">
            <span class="home-text18">
              Who is CAT
              <span v-html="raw7reg"></span>
            </span>
            <br />
            <span class="home-text20">Covid-19 for?</span>
          </span>
        </div>
        <div class="home-circle3">
          <span class="home-text21">
            <span class="home-text22">
              To read more go to
              <span v-html="rawykgm"></span>
            </span>
            <span class="home-text23">About CAT Covid-19</span>
          </span>
          <img
            alt="image"
            src="/playground_assets/ellipse%201.svg"
            class="home-image3"
          />
          <span class="home-text24">
            <span class="home-text25">Learn More</span>
          </span>
        </div>
      </div>
    </div>
    <app-footer></app-footer>
  </div>
</template>

<script>
import AppHeader1 from '../components/header1'
import AppFooter from '../components/footer'

export default {
  name: 'Home',
  components: {
    AppHeader1,
    AppFooter,
  },

  data() {
    return {
      raw7reg: ' ',
      rawykgm: ' ',
    }
  },

  head: {
    title: 'CAT COVID-19 Tools',
    meta: [
      {
        property: 'og:title',
        content: 'CAT COVID-19 Tools',
      },
    ],
  },
}
</script>

<style scoped>
.home-container {
  width: 100%;
  display: flex;
  overflow: auto;
  min-height: 100vh;
  align-items: center;
  flex-direction: column;
  background-image: linear-gradient(135deg, rgb(255, 255, 255) 24.00%,rgb(255, 251, 251) 50.00%,rgb(234, 255, 249) 73.00%,rgb(196, 248, 223) 88.00%,rgb(225, 218, 218) 100.00%);
}
.home-middle {
  width: 100%;
  height: 100%;
  display: flex;
  position: relative;
  align-items: center;
  flex-direction: column;
}
.home-lines {
  top: 200px;
  left: 0px;
  right: 0px;
  width: 95%;
  bottom: 0px;
  height: auto;
  margin: auto;
  display: flex;
  position: absolute;
  flex-wrap: wrap;
  align-items: center;
  flex-direction: column;
  object-position: center;
}
.home-line1 {
  top: 100px;
  left: 0px;
  right: 0px;
  width: 90%;
  height: auto;
  margin: auto;
  position: absolute;
  align-self: center;
  max-height: auto;
  min-height: auto;
  object-fit: cover;
}
.home-line2 {
  top: 0px;
  left: 0px;
  width: 95%;
  height: auto;
  margin: auto;
  display: none;
  position: absolute;
  max-height: 800px;
  min-height: auto;
  object-fit: cover;
}
.home-line3 {
  top: 0px;
  left: 0px;
  width: 95%;
  height: auto;
  margin: auto;
  display: none;
  position: absolute;
  max-height: 800px;
  min-height: auto;
  object-fit: cover;
}
.home-heading {
  flex: 0 0 auto;
  width: auto;
  height: auto;
  display: flex;
  align-items: flex-start;
  justify-content: center;
}
.home-hero {
  width: 100%;
  display: flex;
  position: relative;
  max-width: var(--dl-size-size-maxwidth);
  min-height: 40vh;
  align-items: center;
  padding-top: var(--dl-space-space-twounits);
  padding-left: var(--dl-space-space-twounits);
  padding-right: var(--dl-space-space-twounits);
  flex-direction: row;
  padding-bottom: var(--dl-space-space-halfunit);
  justify-content: space-between;
}
.home-image {
  width: auto;
  object-fit: cover;
}
.home-container1 {
  display: flex;
  margin-left: var(--dl-space-space-twounits);
  flex-direction: column;
}
.home-text {
  font-size: 2.5em;
  text-align: center;
  font-family: Farro;
  font-weight: 700;
  line-height: 1.15;
  text-transform: none;
  text-decoration: none;
}
.home-text01 {
  font-size: 21px;
  align-self: stretch;
  margin-top: var(--dl-space-space-unit);
  text-align: center;
  font-family: Open Sans;
  font-weight: 400;
  line-height: 1.2;
  margin-bottom: var(--dl-space-space-unit);
  text-transform: none;
  text-decoration: none;
}
.home-button {
  color: var(--dl-color-gray-white);
  width: 170px;
  position: relative;
  font-size: 13px;
  align-self: center;
  box-shadow: 5px 5px 10px 0px #d4d4d4;
  margin-top: var(--dl-space-space-unit);
  text-align: center;
  transition: 0.3s;
  font-family: Farro;
  padding-left: 0px;
  border-radius: 10px;
  padding-right: 0px;
  background-color: var(--dl-color-gray-black);
}
.home-button:hover {
  transform: scale(1.02);
}
.home-text03 {
  color: var(--dl-color-primary-100);
  font-size: 25px;
  font-style: normal;
  text-align: center;
  font-weight: 600;
}
.home-circles {
  flex: 0 0 auto;
  width: 100%;
  height: 500px;
  display: flex;
  z-index: 3;
  position: relative;
  align-items: center;
  justify-content: center;
}
.home-circle1 {
  display: flex;
  position: relative;
  transition: 0.1s;
  align-items: center;
  margin-right: var(--dl-space-space-oneandhalfunits);
  justify-content: center;
}
.home-circle1:hover {
  border-radius: var(--dl-radius-radius-round);
  background-color: var(--dl-color-primary-sage);
}
.home-text04 {
  top: 120px;
  left: left;
  right: right;
  bottom: bottom;
  position: absolute;
  font-size: 18px;
  text-align: center;
  font-family: Open Sans;
  padding-left: var(--dl-space-space-oneandhalfunits);
  padding-right: var(--dl-space-space-oneandhalfunits);
}
.home-text05 {
  text-align: center;
  font-family: Open Sans;
}
.home-text06 {
  text-align: center;
  font-family: Open Sans;
}
.home-text07 {
  text-align: center;
  font-family: Open Sans;
}
.home-text08 {
  text-align: center;
}
.home-text10 {
  text-align: center;
}
.home-image1 {
  width: 330px;
  height: 330px;
  opacity: 1;
  object-fit: cover;
}
.home-text11 {
  top: 50px;
  left: lef;
  right: right;
  bottom: bottom;
  margin: auto;
  position: absolute;
  font-size: 26px;
  font-style: normal;
  text-align: center;
  font-family: Farro;
  font-weight: 700;
}
.home-text12 {
  font-style: normal;
  text-align: center;
  font-family: Farro;
  font-weight: 700;
}
.home-text14 {
  font-style: normal;
  text-align: center;
  font-family: Farro;
  font-weight: 700;
}
.home-circle2 {
  display: flex;
  position: relative;
  margin-top: 150px;
  transition: 0.1s;
  align-items: center;
  margin-right: var(--dl-space-space-oneandhalfunits);
  justify-content: center;
}
.home-circle2:hover {
  border-radius: var(--dl-radius-radius-round);
  background-color: var(--dl-color-primary-sage);
}
.home-text15 {
  top: 140px;
  left: left;
  right: right;
  bottom: bottom;
  position: absolute;
  font-size: 18px;
  text-align: center;
  font-family: Open Sans;
  padding-top: 0px;
  padding-left: var(--dl-space-space-oneandhalfunits);
  padding-right: var(--dl-space-space-oneandhalfunits);
}
.home-text16 {
  text-align: center;
  font-family: Open Sans;
}
.home-image2 {
  width: 330px;
  height: 330px;
  opacity: 1;
  object-fit: cover;
}
.home-text17 {
  top: 50px;
  left: lef;
  right: right;
  bottom: bottom;
  margin: auto;
  position: absolute;
  font-size: 26px;
  font-style: normal;
  text-align: center;
  font-family: Farro;
  font-weight: 700;
}
.home-text18 {
  font-style: normal;
  text-align: center;
  font-family: Farro;
  font-weight: 700;
}
.home-text20 {
  font-style: normal;
  font-family: Farro;
  font-weight: 700;
}
.home-circle3 {
  display: flex;
  position: relative;
  transition: 0.1s;
  align-items: center;
  margin-right: 0px;
  justify-content: center;
}
.home-circle3:hover {
  border-radius: var(--dl-radius-radius-round);
  background-color: var(--dl-color-primary-sage);
}
.home-text21 {
  top: 150px;
  left: 0px;
  position: absolute;
  font-size: 18px;
  text-align: center;
  font-family: Open Sans;
  padding-left: var(--dl-space-space-oneandhalfunits);
  padding-right: var(--dl-space-space-oneandhalfunits);
}
.home-text22 {
  text-align: center;
  font-family: Open Sans;
}
.home-text23 {
  font-style: normal;
  text-align: center;
  font-family: Open Sans;
  font-weight: 700;
}
.home-image3 {
  width: 330px;
  height: 330px;
  opacity: 1;
  object-fit: cover;
}
.home-text24 {
  top: 40px;
  left: lef;
  right: right;
  bottom: bottom;
  position: absolute;
  font-size: 26px;
  font-style: normal;
  margin-top: 60px;
  text-align: center;
  font-family: Farro;
  font-weight: 700;
  margin-left: auto;
  margin-right: auto;
  margin-bottom: auto;
}
.home-text25 {
  font-style: normal;
  text-align: center;
  font-family: Farro;
  font-weight: 700;
}
@media(max-width: 1200px) {
  .home-container {
    justify-content: space-between;
  }
  .home-middle {
    position: relative;
    align-self: center;
    padding-left: var(--dl-space-space-threeunits);
    padding-right: var(--dl-space-space-threeunits);
  }
  .home-lines {
    top: 200px;
    left: 0px;
    right: 0px;
    width: auto;
    bottom: 0px;
    height: auto;
    margin: auto;
    position: absolute;
    justify-content: center;
  }
  .home-line1 {
    width: 95%;
    height: auto;
    position: static;
    align-self: center;
    max-height: 100%;
    object-position: center;
  }
  .home-line2 {
    width: auto;
    display: none;
    position: static;
    align-self: center;
    max-height: auto;
    object-position: center;
  }
  .home-line3 {
    display: none;
    position: static;
    align-self: center;
    object-position: center;
  }
  .home-heading {
    align-self: flex-start;
  }
  .home-hero {
    padding-left: var(--dl-space-space-fourunits);
    padding-right: var(--dl-space-space-fourunits);
  }
  .home-image {
    width: 426px;
    height: 318px;
  }
  .home-circles {
    height: auto;
    padding-left: var(--dl-space-space-threeunits);
    padding-right: var(--dl-space-space-threeunits);
  }
}
@media(max-width: 991px) {
  .home-lines {
    top: 0px;
    left: 0px;
    right: 0px;
    bottom: 0px;
    height: auto;
    position: absolute;
    align-self: center;
    align-items: center;
    justify-content: center;
  }
  .home-line1 {
    display: none;
  }
  .home-line2 {
    top: 500px;
    left: 0px;
    right: 0px;
    width: auto;
    bottom: 0px;
    margin: auto;
    display: flex;
    position: absolute;
    align-self: center;
    max-height: auto;
    min-height: auto;
  }
  .home-line3 {
    top: 1010px;
    bottom: 856px;
    display: none;
  }
  .home-heading {
    flex-wrap: wrap;
    align-items: flex-start;
    flex-direction: row;
    justify-content: center;
  }
  .home-hero {
    min-height: auto;
    padding-top: var(--dl-space-space-threeunits);
    padding-left: var(--dl-space-space-threeunits);
    padding-right: var(--dl-space-space-threeunits);
    flex-direction: column;
    padding-bottom: var(--dl-space-space-halfunit);
  }
  .home-image {
    width: auto;
    height: 300px;
  }
  .home-container1 {
    align-items: center;
    margin-left: 0px;
    margin-right: 0px;
    margin-bottom: var(--dl-space-space-twounits);
  }
  .home-circles {
    height: auto;
    flex-wrap: wrap;
    align-items: flex-start;
    justify-content: center;
  }
  .home-circle1 {
    align-self: flex-start;
  }
  .home-circle2 {
    align-self: center;
    margin-top: 0px;
  }
  .home-circle3 {
    align-self: flex-end;
  }
}
@media(max-width: 767px) {
  .home-lines {
    top: 150px;
    left: 0px;
    right: 0px;
    bottom: 0px;
    margin: auto;
    z-index: 0;
    position: absolute;
    flex-wrap: wrap;
    align-self: center;
    flex-direction: column;
  }
  .home-line1 {
    max-height: auto;
  }
  .home-line2 {
    top: 420px;
    left: 0px;
    right: 0px;
    width: auto;
    bottom: 0px;
    height: auto;
    margin: auto;
    position: absolute;
    max-height: auto;
  }
  .home-hero {
    padding-left: var(--dl-space-space-twounits);
    padding-right: var(--dl-space-space-twounits);
    padding-bottom: var(--dl-space-space-halfunit);
  }
  .home-circle2 {
    margin-top: 0px;
  }
}
@media(max-width: 650px) {
  .home-lines {
    top: 0px;
    left: 0px;
    right: 0px;
    bottom: 0px;
    margin: auto;
  }
  .home-line1 {
    top: 0px;
    left: 0px;
    right: 0px;
    bottom: 0px;
    margin: auto;
  }
  .home-line2 {
    display: none;
    position: static;
  }
  .home-line3 {
    top: 400px;
    flex: 0;
    left: 0px;
    right: 0px;
    width: auto;
    bottom: 0px;
    height: 1700px;
    margin: auto;
    display: flex;
    position: absolute;
    max-height: var(--dl-size-size-maxwidth);
    min-height: 1400px;
  }
  .home-hero {
    align-self: flex-start;
    padding-top: var(--dl-space-space-twounits);
    padding-left: var(--dl-space-space-unit);
    padding-right: var(--dl-space-space-unit);
    padding-bottom: var(--dl-space-space-twounits);
  }
  .home-container1 {
    margin-bottom: var(--dl-space-space-unit);
  }
  .home-circle2 {
    margin-top: 0px;
  }
}
</style>
