<template>
  <div>
    <div class="home">
      <div class="bg z-0">
        <section class="screen px-16 wrap z-5 mx-auto w-screen h-screen flex flex-row items-center">
          <div class="Header w-1/2">
          <h1 class="fhead font-bold tracking-tight leading-tight">World trade access <br>on your phone</h1>
          <p class="text text-black-200 headp leading-thight pt-5 phead tracking-normal">Easy App will do ​​movements to empower your business to the highest level. Will you start or if you already have a small-medium business Easy App take you to the next levels of Visibility, Income, Time saving and Customer friendly communication.</p>
          <div class="buttons bhead flex flex-row content-center justify-start items-center">
            <a href="https://apps.apple.com/us/app/apple-store/id375380948?itsct=apps_box_badge&amp;itscg=30200" style="display: inline-block; overflow: hidden; border-radius: 13px; width: 150px; height: 83px;"><img src="https://tools.applemediaservices.com/api/badges/download-on-the-app-store/black/en-us?size=250x83&amp;releaseDate=1276560000&h=7e7b68fad19738b5649a1bfb78ff46e9" alt="Download on the App Store" style="border-radius: 13px; width: 250px; height: 84px;"></a>
            <a class="gwrap" style="height: 70px;" href='https://play.google.com/store/apps/details?id=com.facebook.orca&gl=NO&pcampaignid=pcampaignidMKT-Other-global-all-co-prtnr-py-PartBadge-Mar2515-1'><img class="glink" style="height: 70px;" alt='Get it on Google Play' src='https://play.google.com/intl/en_us/badges/static/images/badges/en_badge_web_generic.png'/></a>
          </div>
          </div>
          <div class="image w-1/2 flex justify-center content-center top-10">
          <nuxt-img src="/Heroimg.png" class="heroimg"/>
          </div>
        </section>
        <section class="screenm stat features w-screen h-1/2 z-10 border-t-8 border-white">
          <div class="stats w-screen">
          <div class="StatCard">
            <h1 class="font-bold leading-none">23.4K</h1>
            <p class="text text-black-200 font-light leading-thight pt-5 tracking-normal">Users</p>
          </div>
          <div class="StatCard">
            <h1 class="font-bold leading-none">250</h1>
            <p class="text text-black-200 font-light leading-thight pt-5 tracking-normal">Active business</p>
          </div>
          <div class="StatCard">
            <h1 class="font-bold leading-none">50.4K</h1>
            <p class="text text-black-200 font-light leading-thight pt-5 tracking-normal">Downloads</p>
          </div>
          <div class="StatCard">
            <h1 class="font-bold leading-none">2.4K</h1>
            <p class="text text-black-200 font-light leading-thight pt-5 tracking-normal">Purchases</p>
          </div>
          <div class="StatCard">
            <h1 class="font-bold leading-none">100%</h1>
            <p class="text text-black-200 font-normal leading-thight pt-5 tracking-normal">Happy Customers</p>
          </div>
          </div>
        </section>
        <section class="screen px-16 w-screen h-screen flex flex-row items-center">
        <div class="vid-text w-1/2">
          <h2 class="font-bold">Video Features</h2>
          <p class="vidp text-black-200 pt-5">Grat Application Ever Lorem ipsum dolor sit amet, consectetur adipiing elit, sed do eiusmod tempor incididunt ut labore et laborused sed do eiusmod tempor incididunt ut labore et laborused.
          </p>
          <a href="" class="link font-medium text-blue-150 leading-loose">Learn More</a>
        </div>
        <div class="vid w-1/2">
          <video width="100%" height="240" controls>
            <source src="http://www.easyapp.no/wp-content/uploads/2021/07/video.mp4?_=1" type="video/mp4">
            Your browser does not support the video tag.
          </video>
        </div>
        </section>
    </div>
    </div>
  </div>
</template>

<style>
.stat{
  background-color: #fbfbfd;
}
.link{
  font-size: 16px;
}
.stats{
  height: 100%;
  padding: 50px;
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  grid-template-rows: repeat(2, 1fr);
  grid-column-gap: 25px;
  grid-row-gap: 25px;
}
.screen{
  scroll-snap-align: start;
}
video{
  border-radius: 10px;
  border-bottom-left-radius: 10px;
  box-shadow: rgba(100, 100, 111, 0.2) 0px 7px 29px 0px;
}
.screenm{
  scroll-snap-align: center;
}
.vidp{
  padding-bottom: 10px;
  font-size: 16px;
  max-width: 75%;
}
.bg{
  height: 100vh;
  width: 100vw;
  background: linear-gradient(125deg, #ECFCFF 0%, #ECFCFF 40%, #B2FCFF calc(40% + 1px), #B2FCFF 60%, #5EDFFF calc(60% + 1px), #5EDFFF 72%, #3E64FF calc(72% + 1px), #3E64FF 100%);
}
h2{
  font-size: 48px;
}
h1{
  font-size: 64px;
}
.text{
  font-size: 20px;
}
.wrap{
  backdrop-filter: blur(200px);
}
.headp{
  max-width: 75%;
}
.heroimg{
  max-height: 75vh;
}
html{
  scroll-snap-type: mandatory;
  scroll-snap-points-y: repeat(100vh);
  scroll-snap-type: y mandatory;
}
</style>

<script>
export default {
     mounted() {
    this.enter()
  },

  methods: {
    enter() {
      const gsap = this.$gsap
      gsap.from('.heroimg', {y: 50, duration: 2, opacity: 0, delay: 0.3, ease: 'power2.inOut' })
      gsap.from('.fhead', {y: -50, duration: 2, opacity: 0})
      gsap.from('.phead', {y: -50, duration: 2, opacity: 0, delay: 0.3 })
      gsap.from('.bhead', {y: -50, duration: 2, opacity: 0, delay: 0.4 })
    }
  }
}
</script>