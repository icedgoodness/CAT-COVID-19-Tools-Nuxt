<template>
  <div class="model2-container">
    <app-header2 rootClassName="header2-root-class-name"></app-header2>
    <div class="model2-pod">
      <img
        alt="image"
        src="/playground_assets/pod%20bg.svg"
        class="model2-image"
      />
      <div class="model2-container1">
        <img alt="image" src="/playground_assets/pod.svg" class="model2-image1" />
        <div class="model2-pod-content">
          <div class="model2-upperhalf">
            <span class="model2-pod-title">Patient&apos;s full name</span>
            <div class="model2-pod-input">
              <input
                type="text"
                placeholder="Type here"
                class="model2-textinput input"
              />
              <img
                alt="image"
                src="/playground_assets/bi_info-circle-fill.svg"
                class="model2-image2"
              />
            </div>
          </div>
          <div class="model2-lowerhalf">
            <span class="model2-pod-hint">Press ➤ to proceed</span>
            <div class="model2-button-nextprevreset">
              <img
                alt="image"
                src="/playground_assets/previous.svg"
                class="model2-prev"
              />
              <img
                alt="image"
                src="/playground_assets/reset.svg"
                class="model2-reset"
              />
              <img
                alt="image"
                src="/playground_assets/next.svg"
                class="model2-next"
              />
            </div>
          </div>
        </div>
      </div>
    </div>
    <app-footer rootClassName="footer-root-class-name"></app-footer>
  </div>
</template>

<script>
import AppHeader2 from '../components/header2'
import AppFooter from '../components/footer'

export default {
  name: 'Model2',
  components: {
    AppHeader2,
    AppFooter,
  },
  head: {
    title: 'Model-2 - CAT COVID-19 Tools',
    meta: [
      {
        property: 'og:title',
        content: 'Model-2 - CAT COVID-19 Tools',
      },
    ],
  },
}
</script>

<style scoped>
.model2-container {
  width: 100%;
  height: auto;
  display: flex;
  overflow: auto;
  min-height: 100vh;
  align-items: center;
  flex-direction: column;
  justify-content: space-between;
  background-image: linear-gradient(135deg, rgb(255, 255, 255) 24.00%,rgb(255, 251, 251) 50.00%,rgb(234, 255, 249) 73.00%,rgb(196, 248, 223) 88.00%,rgb(225, 218, 218) 100.00%);
}
.model2-pod {
  width: 880px;
  height: 900px;
  position: relative;
  object-fit: scale-down;
  align-items: center;
  background-size: cover;
  justify-content: center;
  background-position: center;
}
.model2-image {
  top: 0px;
  left: 0px;
  right: 0px;
  width: auto;
  bottom: 0px;
  margin: auto;
  position: absolute;
  object-fit: cover;
}
.model2-container1 {
  width: 698px;
  height: 718.5208740234375px;
}
.model2-image1 {
  top: 0px;
  left: 0px;
  right: 0px;
  width: 697.5px;
  bottom: 0px;
  margin: auto;
  position: absolute;
  object-fit: scale-down;
}
.model2-pod-content {
  top: 0px;
  left: 0px;
  right: 0px;
  width: 300px;
  bottom: 0px;
  height: 200px;
  margin: auto;
  display: flex;
  position: absolute;
  align-items: center;
  flex-direction: column;
  justify-content: center;
}
.model2-upperhalf {
  display: flex;
  align-items: center;
  flex-direction: column;
  justify-content: center;
}
.model2-pod-title {
  width: 200px;
  align-self: flex-start;
  font-style: normal;
  margin-top: 0px;
  font-family: Open Sans;
  font-weight: 700;
  margin-bottom: var(--dl-space-space-unit);
}
.model2-pod-input {
  width: auto;
  height: auto;
  display: flex;
  flex-wrap: wrap;
  align-self: flex-end;
  align-items: center;
  flex-direction: row;
  justify-content: center;
}
.model2-textinput {
  align-self: flex-end;
  margin-top: var(--dl-space-space-halfunit);
}
.model2-image2 {
  width: auto;
  align-self: flex-start;
  object-fit: cover;
}
.model2-lowerhalf {
  width: 100%;
  display: flex;
  align-items: center;
  flex-direction: column;
  justify-content: center;
}
.model2-pod-hint {
  align-self: flex-start;
  margin-top: var(--dl-space-space-halfunit);
  margin-left: var(--dl-space-space-unit);
  margin-bottom: var(--dl-space-space-halfunit);
}
.model2-button-nextprevreset {
  flex: 0 0 auto;
  width: auto;
  display: flex;
  align-self: flex-end;
  margin-top: var(--dl-space-space-unit);
  align-items: flex-start;
}
.model2-prev {
  width: auto;
  object-fit: cover;
}
.model2-reset {
  width: auto;
  object-fit: cover;
}
.model2-next {
  width: auto;
  object-fit: cover;
}
@media(max-width: 1200px) {
  .model2-container {
    align-items: center;
    justify-content: space-between;
  }
  .model2-pod {
    height: 900px;
    position: 0px;
    flex-wrap: wrap;
    align-self: center;
    margin-top: 100px;
    margin-bottom: 100px;
  }
  .model2-image {
    top: 0px;
    left: 0px;
    right: 0px;
    width: auto;
    bottom: 0px;
    margin: auto;
    position: absolute;
  }
  .model2-container1 {
    position: static;
  }
  .model2-image1 {
    top: 0px;
    flex: 0;
    left: 0px;
    width: 698px;
    margin: auto;
    position: absolute;
  }
  .model2-pod-content {
    width: 300px;
    height: 200px;
    flex-direction: column;
  }
  .model2-upperhalf {
    position: relative;
  }
  .model2-pod-title {
    font-style: normal;
    font-family: Open Sans;
    font-weight: 700;
  }
  .model2-textinput {
    align-self: flex-start;
  }
  .model2-image2 {
    width: 20px;
  }
  .model2-pod-hint {
    color: var(--dl-color-primary-hijautua);
    font-size: 15px;
    margin-left: var(--dl-space-space-unit);
  }
  .model2-button-nextprevreset {
    width: 180px;
    height: var(--dl-size-size-small);
    align-self: flex-end;
    align-items: center;
    justify-content: center;
  }
}
@media(max-width: 991px) {
  .model2-pod-content {
    top: 0px;
    left: 0px;
    right: 0px;
    bottom: 0px;
    margin: auto;
  }
}
@media(max-width: 767px) {
  .model2-pod-content {
    top: 0px;
    left: 0px;
    right: 0px;
    bottom: 0px;
    margin: auto;
  }
}
@media(max-width: 650px) {
  .model2-pod-content {
    top: 0px;
    left: 0px;
    right: 0px;
    bottom: 0px;
    margin: auto;
  }
}
</style>
