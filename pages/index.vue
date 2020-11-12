<template>
  <div>
    <div class="home-banner">
      <div class="text-center">
        <h1 class="text-white">
          First-Class Services in
        </h1>
        <h5 class="text-white my-4">DESKTOP, MOBILE & WEB APPLICATION DEVELOPMENT</h5>
        <h6 class="text-white">We help you speed up your business process</h6>
        <b-button class="mt-5" pill variant="outline-light">MORE INFO</b-button>
      </div>
    </div>
    <div class="section">
      <h1 class="text-center">How can we help You?</h1>
      <h6 class="text-center">We can help you in the following services.</h6>
      <b-container class="mt-5">
        <b-row>
          <b-col v-for="(service,service_key) in services" :key="service_key" md="4" sm="12" class="text-center mb-3">
            <i v-if="service.icon" class="fa fa-3x fa-user text-primary mb-2"></i>
            <h4 v-html="service.title"></h4>
            <div v-html="service.text"></div>
          </b-col>
        </b-row>
      </b-container>
    </div>
  </div>
</template>

<script>
  export default {
    head: {
      titleTemplate:
        'Best ERP, CRM, POS, EIMS Software & IT Service Provider Company-%s',
      meta: [
        {charset: 'utf-8'},
        {name: 'viewport', content: 'width=device-width, initial-scale=1'},

        // hid is used as unique identifier. Do not use `vmid` for it as it will not work
        {
          hid: 'description',
          name: 'description',
          content:
            'Best ERP, CRM, POS, EIMS Software & IT Service Provider Company',
        },
      ],
    },
    data() {
      return {
        services: [
          {
            icon: 'accusoft',
            title: 'Web Application',
            text: 'We have focused our efforts in most popular operating systems and platforms. Full spectrum of development services spiced with flexible engagement.'
          },
          {
            icon: 'accusoft',
            title: 'Mobile Application',
            text: 'Our custom website development are a creative blend of marketing Productive, engaging and reliable web solutions for business outcomes you desire.'
          },
          {
            icon: 'accusoft',
            title: 'Desktop Application',
            text: 'We have 8 years of Digital Marketing Experience. We can bring lot of clients to your business. Get connected with us, we will bring clients to you.'
          },
          {
            icon: 'accusoft',
            title: 'Web Design',
            text: 'We have focused our efforts in most popular operating systems and platforms. Full spectrum of development services spiced with flexible engagement.'
          },
          {
            icon: 'accusoft',
            title: 'Web Development',
            text: 'Our custom website development are a creative blend of marketing Productive, engaging and reliable web solutions for business outcomes you desire.'
          },
          {
            icon: 'accusoft',
            title: 'eCommerce Website',
            text: 'Now-a-days selling products in digital medias is a common trend. So, your business should be digitized too. We can help building eCommerce Websites for B2B, B2C, C2C, C2B, B2A, C2A.\n'
          },
          {
            icon: 'accusoft',
            title: 'Social Media Marketing',
            text: 'Recently we started services in Renowned Social Medias too. We provide 100% organic Social Media Marketing.'
          },
          {
            icon: 'accusoft',
            title: 'Digital Marketing',
            text: 'We have 8 years of Digital Marketing Experience. We can bring lot of clients to your business. Get connected with us, we will bring clients to you.'
          },
          {
            icon: 'accusoft',
            title: 'Help & Support',
            text: 'We can help you fixing your current products like Websites, Softwares issues'
          }
        ]
      }
    }
  }
</script>

<style>
  .home-banner {
    background-image: url('~assets/home-banner.jpg');
    background-size: cover;
  }

  .home-banner > div {
    padding-top: 80px;
    padding-bottom: 80px;
    background-color: rgba(0, 0, 0, 0.2);
  }

  .section {
    padding-top: 80px;
    padding-bottom: 80px;
  }
</style>
