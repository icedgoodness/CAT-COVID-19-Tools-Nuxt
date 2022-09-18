<template>
  <div class="circle-container">
    <div class="circle-circle1">
      <span class="circle-text">
        <span class="circle-text01"></span>
        <span class="circle-text02"></span>
        <span class="circle-text03"></span>
        <span class="circle-text04">
          CAT Covid-19 predicts covid-19 patients&apos; mortality with two
          different methods; model 1 and model 2. Model 1 is recommended for
          patients with limited resources and Model 2 can be used when laboratory
          data exists.
        </span>
        <br />
        <span></span>
        <span class="circle-text06"></span>
      </span>
      <img :alt="image_alt" :src="image_src" class="circle-image" />
      <span class="circle-text07">
        <span class="circle-text08">What does CAT</span>
        <br />
        <span class="circle-text10">Covid-19 do?</span>
      </span>
    </div>
    <div class="circle-circle2">
      <span class="circle-text11">
        <span class="circle-text12">
          CAT Covid-19 can be used by clinicians, patients and their families and
          significant others. Patients should use it in consultation with a
          medical professional.
        </span>
      </span>
      <img :alt="image_alt1" :src="image_src1" class="circle-image1" />
      <span class="circle-text13">
        <span class="circle-text14">
          Who is CAT
          <span v-html="rawccxz"></span>
        </span>
        <br />
        <span class="circle-text16">Covid-19 for?</span>
      </span>
    </div>
    <div class="circle-circle3">
      <span class="circle-text17">
        <span class="circle-text18">
          To read more go to
          <span v-html="raw7qv2"></span>
        </span>
        <span class="circle-text19">About CAT Covid-19</span>
      </span>
      <img :alt="image_alt2" :src="image_src2" class="circle-image2" />
      <span class="circle-text20">
        <span class="circle-text21">Learn More</span>
      </span>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Circle',
  props: {
    image_alt1: {
      type: String,
      default: 'image',
    },
    image_src1: {
      type: String,
      default: '/playground_assets/ellipse%201.svg',
    },
    image_alt: {
      type: String,
      default: 'image',
    },
    image_alt2: {
      type: String,
      default: 'image',
    },
    image_src: {
      type: String,
      default: '/playground_assets/ellipse%201.svg',
    },
    image_src2: {
      type: String,
      default: '/playground_assets/ellipse%201.svg',
    },
  },

  data() {
    return {
      rawccxz: ' ',
      raw7qv2: ' ',
    }
  },
}
</script>

<style scoped>
.circle-container {
  flex: 0 0 auto;
  width: 100%;
  height: 500px;
  display: flex;
  position: relative;
  align-items: center;
  justify-content: center;
}
.circle-circle1 {
  display: flex;
  position: relative;
  align-items: center;
  margin-right: var(--dl-space-space-oneandhalfunits);
  justify-content: center;
}
.circle-text {
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
.circle-text01 {
  text-align: center;
  font-family: Open Sans;
}
.circle-text02 {
  text-align: center;
  font-family: Open Sans;
}
.circle-text03 {
  text-align: center;
  font-family: Open Sans;
}
.circle-text04 {
  text-align: center;
}
.circle-text06 {
  text-align: center;
}
.circle-image {
  width: 330px;
  height: 330px;
  opacity: 1;
  object-fit: cover;
}
.circle-text07 {
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
.circle-text08 {
  font-style: normal;
  text-align: center;
  font-family: Farro;
  font-weight: 700;
}
.circle-text10 {
  font-style: normal;
  text-align: center;
  font-family: Farro;
  font-weight: 700;
}
.circle-circle2 {
  display: flex;
  position: relative;
  margin-top: 150px;
  align-items: center;
  margin-right: var(--dl-space-space-oneandhalfunits);
  justify-content: center;
}
.circle-text11 {
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
.circle-text12 {
  text-align: center;
  font-family: Open Sans;
}
.circle-image1 {
  width: 330px;
  height: 330px;
  opacity: 1;
  object-fit: cover;
}
.circle-text13 {
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
.circle-text14 {
  font-style: normal;
  text-align: center;
  font-family: Farro;
  font-weight: 700;
}
.circle-text16 {
  font-style: normal;
  font-family: Farro;
  font-weight: 700;
}
.circle-circle3 {
  display: flex;
  position: relative;
  align-items: center;
  margin-right: 0px;
  justify-content: center;
}
.circle-text17 {
  top: 150px;
  left: 0px;
  position: absolute;
  font-size: 18px;
  text-align: center;
  font-family: Open Sans;
  padding-left: var(--dl-space-space-oneandhalfunits);
  padding-right: var(--dl-space-space-oneandhalfunits);
}
.circle-text18 {
  text-align: center;
  font-family: Open Sans;
}
.circle-text19 {
  font-style: normal;
  text-align: center;
  font-family: Open Sans;
  font-weight: 700;
}
.circle-image2 {
  width: 330px;
  height: 330px;
  opacity: 1;
  object-fit: cover;
}
.circle-text20 {
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
.circle-text21 {
  font-style: normal;
  text-align: center;
  font-family: Farro;
  font-weight: 700;
}
@media(max-width: 1200px) {
  .circle-container {
    height: auto;
  }
}
@media(max-width: 991px) {
  .circle-container {
    height: auto;
    flex-wrap: wrap;
    align-items: flex-start;
    justify-content: center;
  }
  .circle-circle1 {
    align-self: flex-start;
  }
  .circle-circle2 {
    align-self: center;
    margin-top: 0px;
  }
  .circle-circle3 {
    align-self: flex-end;
  }
}
@media(max-width: 767px) {
  .circle-circle2 {
    margin-top: 0px;
  }
}
@media(max-width: 650px) {
  .circle-circle2 {
    margin-top: 0px;
  }
}
</style>
