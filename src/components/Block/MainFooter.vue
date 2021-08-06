<template>
  <div>
    <footer class="footer">
      <div class="footer__top">
        <div class="container">
          <div class="row">
            <div class="col-12">
              <div class="footer__top-inner">
                <a href="" class="footer__logo">
                  <img :src="require(`@/assets/img/logo-white.svg`)" alt="">
                </a>
                <ul class="footer__nav">
                  <li class="footer__nav-item">
                    <a href="" class="footer__nav-link">Expertenauswahl</a>
                  </li>
                  <li class="footer__nav-item">
                    <a href="" class="footer__nav-link">Dienstleistungen</a>
                  </li>
                  <li class="footer__nav-item">
                    <a href="" class="footer__nav-link">Neueste Bewertungen</a>
                  </li>
                  <li class="footer__nav-item">
                    <a href="" class="footer__nav-link">Über den Service</a>
                  </li>
                  <li class="footer__nav-item">
                    <a href="" class="footer__nav-link">Service-News</a>
                  </li>
                  <li class="footer__nav-item">
                    <a href="" class="footer__nav-link">FAQ</a>
                  </li>
                  <li class="footer__nav-item">
                    <a href="" class="footer__nav-link">Kontakt</a>
                  </li>
                </ul>
                <div class="footer__copyright d-none d-xxl-block">
                  © 2021 Alle Rechte vorbehalten
                </div>
                <ul class="langs">
                  <li class="langs__item">
                    <a href="" class="langs__item-link">
                      Eng
                      <svg width="10" height="6" viewBox="0 0 10 6" fill="none" xmlns="http://www.w3.org/2000/svg">
                        <path d="M1.08984 1L4.92727 5L8.42318 1" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
                      </svg>
                    </a>
                    <ul class="langs__sublist">
                      <li class="langs__sublist-item">
                        <a href="" class="langs__sublist-link">Deu</a>
                      </li>
                    </ul>
                  </li>
                </ul>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="footer__bot d-xxl-none">
        <div class="container">
          <div class="row">
            <div class="col-12">
              <div class="footer__copyright">
                © 2021 Alle Rechte vorbehalten
              </div>
            </div>
          </div>
        </div>
      </div>
    </footer>
  
    <!-- <div class="scroll-top">
        <svg width="18" height="10" viewBox="0 0 18 10" fill="none" xmlns="http://www.w3.org/2000/svg">
            <path d="M1 9L9.37257 1L17 9" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"/>
        </svg>
    </div> -->
  
    <div class="progress-wrap">
      <svg class="progress-circle svg-content" width="100%" height="100%" viewBox="-1 -1 102 102">
        <path d="M50,1 a49,49 0 0,1 0,98 a49,49 0 0,1 0,-98"/>
      </svg>
    </div>
  
  </div>
</template>

<script>
export default {
  
  name:'MainFooter'
}

</script>
