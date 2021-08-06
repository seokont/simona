<template>
  <div class="wrapper">
    <main-header></main-header>
    <section class="promo">
      <div class="promo__slider">
        <carousel ref="carousel" :dots="false" :nav="false" :lazyLoad="true" :autoplay="true" :lazyLoadEager="5"
                  :loop="false" :rewind="false" :items="1"
                  :autoWidth="false" :margin="20"
                  :class="['carousel__home']">
          <div class="promo__slider-item" v-for="item in slider" :key="item.id">
            <div class="container">
              <div class="row">
                <div class="col-12">
                  <h1 class="promo__title" data-aos="slide-down">
                    {{ item.title }}
                  </h1>
                  <div class="promo__btn-wrap" data-aos="slide-down">
                    <a href="" class="btn btn--main btn--static">
								<span>
									{{ item.button }}
								</span>
                    </a>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </carousel>
      </div>
      <div class="promo__nav">
        <img class="promo__nav-zodiaks" src="@/assets/img/zodiac.svg" alt="">
        <img class="promo__nav-bg" src="@/assets/img/circle.svg" alt="">
        <div class="promo__nav-prev">
          <svg width="71" height="12" viewBox="0 0 71 12" fill="none" xmlns="http://www.w3.org/2000/svg">
            <path
              d="M9.38519 0.0371094C6.58248 1.73402 3.78429 3.43814 0.984734 5.13955V6.35241C3.65112 7.97149 6.31661 9.59148 8.98255 11.211C9.10537 11.3023 9.27002 11.3473 9.36089 11.4724H9.37843C9.48011 11.2762 9.61687 11.1003 9.71854 10.9047C7.11918 9.33775 4.53468 7.74476 1.93172 6.1846C24.9336 6.18505 47.9356 6.1855 70.9375 6.18415C70.9366 5.89174 70.9375 5.59887 70.9371 5.30645C49.0288 5.306 27.1205 5.306 5.21217 5.306C4.12169 5.29881 3.02985 5.32085 1.93936 5.29476C2.22818 5.15035 2.49406 4.965 2.77297 4.80305C5.08891 3.3963 7.40395 1.9882 9.72079 0.582354C9.61282 0.398356 9.49495 0.220207 9.38519 0.0371094Z"
              fill="white"/>
          </svg>
        </div>
        <div class="promo__nav-next">
          <svg width="70" height="12" viewBox="0 0 70 12" fill="none" xmlns="http://www.w3.org/2000/svg">
            <path
              d="M61.5836 0.0371094C64.3863 1.73402 67.1845 3.43814 69.984 5.13955V6.35241C67.3176 7.97149 64.6521 9.59148 61.9862 11.211C61.8634 11.3023 61.6987 11.3473 61.6079 11.4724H61.5903C61.4886 11.2762 61.3519 11.1003 61.2502 10.9047C63.8496 9.33775 66.4341 7.74476 69.037 6.1846C46.0351 6.18505 23.0332 6.1855 0.03125 6.18415C0.0321497 5.89174 0.03125 5.59887 0.0316999 5.30645C21.94 5.306 43.8483 5.306 65.7566 5.306C66.8471 5.29881 67.9389 5.32085 69.0294 5.29476C68.7406 5.15035 68.4747 4.965 68.1958 4.80305C65.8798 3.3963 63.5648 1.9882 61.248 0.582354C61.3559 0.398356 61.4738 0.220207 61.5836 0.0371094Z"
              fill="white"/>
          </svg>
        </div>
      </div>
    </section>
    <section class="benefits-section mt-lg mb-lg">
      <div class="container benefits-section__list">
        <div class="row">
          <div class="col-xl-3 col-md-6 benefits-section__list-item" data-aos="fade-up">
            <div class="benefits-section__item">
              <div class="benefits-section__item-icon">
                <img src="@/assets/img/benefit-icon-1.svg" alt="">
              </div>
              <div class="benefits-section__item-title">
                Kostenloser Support-Service für alle Benutzer
              </div>
            </div>
          </div>
          <div class="col-xl-3 col-md-6 benefits-section__list-item" data-aos="fade-up" data-aos-delay="200">
            <div class="benefits-section__item">
              <div class="benefits-section__item-icon">
                <img src="@/assets/img/benefit-icon-2.svg" alt="">
              </div>
              <div class="benefits-section__item-title">
                Eine Stunde der ersten Beratung mit einem Experten ist kostenlos!
              </div>
            </div>
          </div>
          <div class="col-xl-3 col-md-6 benefits-section__list-item" data-aos="fade-up" data-aos-delay="400">
            <div class="benefits-section__item">
              <div class="benefits-section__item-icon">
                <img src="@/assets/img/benefit-icon-3.svg" alt="">
              </div>
              <div class="benefits-section__item-title">
                Sie können nicht mit einem Spezialisten sprechen? Wählen Sie schriftliche Konsultationen im Chat
              </div>
            </div>
          </div>
          <div class="col-xl-3 col-md-6 benefits-section__list-item" data-aos="fade-up" data-aos-delay="600">
            <div class="benefits-section__item">
              <div class="benefits-section__item-icon">
                <img src="@/assets/img/benefit-icon-4.svg" alt="">
              </div>
              <div class="benefits-section__item-title">
                Kostenloser Support-Service für alle Benutzer
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
    <section class="expert-section pb-lg">
      <div class="container">
        <div class="row">
          <div class="col-12">
            <div class="section__header">
              <div class="section__line">
                <svg data-aos="zoom-in" data-aos-delay="600" class="section__line-dot" width="3" height="3"
                     viewBox="0 0 3 3" fill="none" xmlns="http://www.w3.org/2000/svg">
                  <circle cx="1.5" cy="1.5" r="1.5"/>
                </svg>
                <svg data-aos="zoom-left" data-aos-delay="400" class="section__line-line" width="623" height="1"
                     viewBox="0 0 623 1" fill="none" xmlns="http://www.w3.org/2000/svg">
                  <line x1="4.37114e-08" y1="0.5" x2="623" y2="0.500054"/>
                </svg>
                <svg data-aos="zoom-in" data-aos-delay="200" class="section__line-dot" width="3" height="3"
                     viewBox="0 0 3 3" fill="none" xmlns="http://www.w3.org/2000/svg">
                  <circle cx="1.5" cy="1.5" r="1.5"/>
                </svg>
                <svg data-aos="zoom-in" class="section__line-middle" width="30" height="30" viewBox="0 0 30 30"
                     fill="none" xmlns="http://www.w3.org/2000/svg">
                  <circle cx="15" cy="15" r="14.3" stroke-width="1.4"/>
                  <circle cx="15" cy="15" r="1.3" stroke-width="1.4"/>
                  <path
                    d="M15.0239 6H14.9789C14.9754 6.04957 14.955 6.09633 14.9227 6.13359C14.222 7.34437 13.5206 8.56008 12.8175 9.77156C11.4236 9.39504 10.0307 9.01359 8.63672 8.63672C9.01289 10.0303 9.39609 11.4225 9.77051 12.8168C8.51578 13.548 7.25684 14.2716 6 14.9993V15C7.25648 15.7288 8.51613 16.4523 9.77121 17.1829C9.39504 18.5768 9.01359 19.9693 8.63672 21.3629C10.0307 20.9868 11.4232 20.605 12.8168 20.2288C13.5473 21.4839 14.2716 22.7432 14.9996 24H15C15.7288 22.7439 16.4516 21.4839 17.1836 20.2295C18.5775 20.6043 19.9697 20.9868 21.3633 21.3633C20.9864 19.9693 20.6053 18.5768 20.2284 17.1825C21.4846 16.4534 22.7432 15.7281 24 15C22.7439 14.2712 21.4842 13.548 20.2295 12.8168C20.6043 11.4225 20.9871 10.0307 21.3633 8.63672C19.9693 9.01289 18.5771 9.39609 17.1829 9.77051C16.4776 8.56008 15.7805 7.34473 15.0766 6.13324C15.0573 6.09105 15.012 6.04992 15.0239 6ZM15.2341 10.8702C16.1479 10.9198 17.038 11.2889 17.7229 11.8943C18.491 12.5651 19.0015 13.5266 19.1101 14.5416C19.1973 15.3108 19.0658 16.1046 18.7287 16.8018C18.3479 17.5998 17.6993 18.266 16.9136 18.671C16.1791 19.0553 15.327 19.2061 14.5046 19.107C13.6163 19.0064 12.7641 18.6049 12.1246 17.9798C11.4932 17.3755 11.0674 16.5641 10.9226 15.7028C10.7855 14.8949 10.8878 14.0466 11.2239 13.2984C11.568 12.5275 12.1569 11.87 12.8832 11.4408C13.5874 11.0224 14.4171 10.8231 15.2341 10.8702Z"/>
                </svg>
                <svg data-aos="zoom-in" data-aos-delay="200" class="section__line-dot" width="3" height="3"
                     viewBox="0 0 3 3" fill="none" xmlns="http://www.w3.org/2000/svg">
                  <circle cx="1.5" cy="1.5" r="1.5"/>
                </svg>
                <svg data-aos="zoom-right" data-aos-delay="400" class="section__line-line" width="623" height="1"
                     viewBox="0 0 623 1" fill="none" xmlns="http://www.w3.org/2000/svg">
                  <line x1="4.37114e-08" y1="0.5" x2="623" y2="0.500054"/>
                </svg>
                <svg data-aos="zoom-in" data-aos-delay="600" class="section__line-dot" width="3" height="3"
                     viewBox="0 0 3 3" fill="none" xmlns="http://www.w3.org/2000/svg">
                  <circle cx="1.5" cy="1.5" r="1.5"/>
                </svg>
              </div>
              <h2 class="section__title">Experten</h2>
            </div>
          </div>
          <div class="col-lg-3" data-aos="fade-right">
            <a href="" class="btn btn--border-main filter-display-btn d-lg-none">
              <span>Filter</span>
            </a>
            <div class="filter d-lg-block">
              <div class="filter__group">
                <div class="filter__group-title">
                  Spezialisierung
                  <svg width="12" height="8" viewBox="0 0 12 8" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <path d="M1 1L6.23286 6.45455L11 1" stroke-width="1.5" stroke-linecap="round"
                          stroke-linejoin="round"/>
                  </svg>
                </div>
                <div class="filter__group-body">
                  empty
                </div>
              </div>
              <div class="filter__group">
                <div class="filter__group-title">
                  Thema der Frage
                  <svg width="12" height="8" viewBox="0 0 12 8" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <path d="M1 1L6.23286 6.45455L11 1" stroke-width="1.5" stroke-linecap="round"
                          stroke-linejoin="round"/>
                  </svg>
                </div>
                <div class="filter__group-body">
                  <label for="checkbox-1" class="checkbox">
                    <input type="checkbox" id="checkbox-1" class="checkbox__input">
                    <div class="checkbox__marker"></div>
                    <div class="checkbox__text">Liebe</div>
                  </label>
                  <label for="checkbox-2" class="checkbox">
                    <input type="checkbox" id="checkbox-2" class="checkbox__input">
                    <div class="checkbox__marker"></div>
                    <div class="checkbox__text">Die Familie</div>
                  </label>
                  <label for="checkbox-3" class="checkbox">
                    <input type="checkbox" id="checkbox-3" class="checkbox__input">
                    <div class="checkbox__marker"></div>
                    <div class="checkbox__text">Finanzen</div>
                  </label>
                  <label for="checkbox-4" class="checkbox">
                    <input type="checkbox" id="checkbox-4" class="checkbox__input">
                    <div class="checkbox__marker"></div>
                    <div class="checkbox__text">Arbeit</div>
                  </label>
                  <label for="checkbox-5" class="checkbox">
                    <input type="checkbox" id="checkbox-5" class="checkbox__input">
                    <div class="checkbox__marker"></div>
                    <div class="checkbox__text">Energie</div>
                  </label>
                </div>
              </div>
              <div class="filter__group">
                <div class="filter__group-title">
                  Status
                  <svg width="12" height="8" viewBox="0 0 12 8" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <path d="M1 1L6.23286 6.45455L11 1" stroke-width="1.5" stroke-linecap="round"
                          stroke-linejoin="round"/>
                  </svg>
                </div>
                <div class="filter__group-body">
                  empty
                </div>
              </div>
              <div class="filter__group">
                <div class="filter__group-title">
                  Land
                  <svg width="12" height="8" viewBox="0 0 12 8" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <path d="M1 1L6.23286 6.45455L11 1" stroke-width="1.5" stroke-linecap="round"
                          stroke-linejoin="round"/>
                  </svg>
                </div>
                <div class="filter__group-body">
                  empty
                </div>
              </div>
              <div class="filter__group">
                <div class="filter__group-title">
                  Stadt
                  <svg width="12" height="8" viewBox="0 0 12 8" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <path d="M1 1L6.23286 6.45455L11 1" stroke-width="1.5" stroke-linecap="round"
                          stroke-linejoin="round"/>
                  </svg>
                </div>
                <div class="filter__group-body">
                  empty
                </div>
              </div>
              <div class="filter__group">
                <div class="filter__group-title">
                  Erfahrung
                  <svg width="12" height="8" viewBox="0 0 12 8" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <path d="M1 1L6.23286 6.45455L11 1" stroke-width="1.5" stroke-linecap="round"
                          stroke-linejoin="round"/>
                  </svg>
                </div>
                <div class="filter__group-body">
                  empty
                </div>
              </div>
              <div class="filter__group">
                <div class="filter__group-title">
                  Fußboden
                  <svg width="12" height="8" viewBox="0 0 12 8" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <path d="M1 1L6.23286 6.45455L11 1" stroke-width="1.5" stroke-linecap="round"
                          stroke-linejoin="round"/>
                  </svg>
                </div>
                <div class="filter__group-body">
                  empty
                </div>
              </div>
              <div class="filter__group">
                <div class="filter__group-title">
                  Kommunikationsart
                  <svg width="12" height="8" viewBox="0 0 12 8" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <path d="M1 1L6.23286 6.45455L11 1" stroke-width="1.5" stroke-linecap="round"
                          stroke-linejoin="round"/>
                  </svg>
                </div>
                <div class="filter__group-body">
                  empty
                </div>
              </div>
            </div>
          </div>
          <div class="col-lg-9">
            <div class="inline-filter">
              <ul class="inline-filter__tabs">
                <li class="inline-filter__tabs-item">
                  <a href="" class="inline-filter__tabs-link active">
                    <span>Alle 265</span>
                  </a>
                </li>
                <li class="inline-filter__tabs-item">
                  <a href="" class="inline-filter__tabs-link"><span>Verfügbare 75</span></a>
                </li>
                <li class="inline-filter__tabs-item">
                  <a href="" class="inline-filter__tabs-link"><span>Exklusiv 262</span></a>
                </li>
                <li class="inline-filter__tabs-item">
                  <a href="" class="inline-filter__tabs-link"><span>Neue 3</span></a>
                </li>
              </ul>
              <div class="display-btns d-none d-xl-flex">
                <a href="" class="display-btn display-btn-inline active">
                  <svg width="12" height="10" viewBox="0 0 12 10" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <rect width="12" height="1.51667" rx="0.758333"/>
                    <rect y="4" width="12" height="1.51667" rx="0.758333"/>
                    <rect y="8" width="12" height="1.51667" rx="0.758333"/>
                  </svg>
                </a>
                <a href="" class="display-btn display-btn-cards">
                  <svg width="10" height="12" viewBox="0 0 10 12" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <rect y="12" width="12" height="1.51667" rx="0.758333" transform="rotate(-90 0 12)"/>
                    <rect x="4" y="12" width="12" height="1.51667" rx="0.758333" transform="rotate(-90 4 12)"/>
                    <rect x="8" y="12" width="12" height="1.51667" rx="0.758333" transform="rotate(-90 8 12)"/>
                  </svg>
                </a>
              </div>
            </div>
            <div class="expert-cards">
              <div class="expert-card" v-for="user in users.slice(0,2)" :key="user.id">
                <div class="expert-card__body">
                  <div class="expert-card__ava">
                    <div class="expert-card__status on"></div>
                    <img :src="require(`@/assets/img/${user.big_avatar}`)" alt="">
                  </div>
                  <div class="expert-card__inner">
                    <div class="expert-card__name">
                      Catherine
                    </div>
                    <ul class="expert-card__info">
                      <li>
                        <img src="@/assets/img/loc-icon.svg" alt="">
                        {{ user.location }}
                      </li>
                      <li>
                        <img src="@/assets/img/clock-icon.svg" alt="">
                        {{ user.term }}
                      </li>
                    </ul>
                    <div class="expert-card__block">
                      <div class="expert-card__block-row">
                        <div class="expert-card__exp expert-card__exp--green">
                          {{ user.status }}
                        </div>
                        <button class="expert-card__add-btn add-btn">
                          <svg width="16" height="14" viewBox="0 0 16 14" fill="none"
                               xmlns="http://www.w3.org/2000/svg">
                            <path
                              d="M14.2176 2.06106C12.7456 0.589021 10.3592 0.589021 8.88733 2.06106L7.99873 2.9495L7.11029 2.06122C5.63825 0.589178 3.2517 0.589178 1.77981 2.06122C0.307771 3.53326 0.307771 5.91966 1.77981 7.3917L2.66825 8.27967L7.99873 13.6101L13.3292 8.27967L14.2175 7.3917C15.6897 5.91966 15.6897 3.5331 14.2176 2.06106ZM11.5523 8.27998L7.99873 11.8336L4.44529 8.27998L2.66857 6.50326C1.68715 5.522 1.68715 3.93092 2.66857 2.94934C3.64998 1.96809 5.24091 1.96809 6.22217 2.94934L7.99873 4.72638L9.77561 2.9495C10.7569 1.96825 12.3479 1.96825 13.3292 2.9495C14.3105 3.93107 14.3105 5.52185 13.3292 6.50342L11.5523 8.27998Z"/>
                          </svg>
                        </button>
                      </div>
                      <div class="expert-card__block-row">
                        <div class="expert-card__reviews">
                          <div class="js-rating" data-rateyo-read-only="true" data-rating="5"></div>
                        </div>
                        <a href="" class="expert-card__review-link">
                          {{ user.review }} bewertungen
                        </a>
                      </div>
                    </div>
                    <p class="expert-card__text">
                      {{ user.text }}
                    </p>
                    <ul class="tags expert-card__tags">
                      <li class="tags__item" v-for="tag in user.tags" :key="tag+'ww'">
                        <a href="" class="tags__link">
                          <span>{{ tag }}</span>
                        </a>
                      </li>
                      <!--                      <li class="tags__item">-->
                      <!--                        <a href="" class="tags__link">-->
                      <!--                          <span>#Numerologie</span>-->
                      <!--                        </a>-->
                      <!--                      </li>-->
                      <!--                      <li class="tags__item">-->
                      <!--                        <a href="" class="tags__link">-->
                      <!--                          <span>#Hellsehen</span>-->
                      <!--                        </a>-->
                      <!--                      </li>-->
                    </ul>
                  </div>
                </div>
                <div class="expert-card__footer">
                  <div class="expert-card__price">
                    <div class="expert-card__price-value">
                      € 0/Min
                    </div>
                    <a href="" class="expert-card__price-btn green">
                      <span>Kostenlos anrufen</span>
                    </a>
                  </div>
                  <div class="expert-card__price">
                    <div class="expert-card__price-value">
                      € 0
                    </div>
                    <a href="" class="expert-card__price-btn border-green">
                      <span>Online-Chat kostenlos</span>
                    </a>
                  </div>
                </div>
              </div>
              <div class="banner">
                <div class="banner__content">
                  <h3 class="banner__title">
                    Banner, das für die
                    Dienste der Website wirbt
                  </h3>
                  <p class="banner__text">
                    Sie können beispielsweise schreiben, dass die erste Stunde des Anrufs für alle neuen Benutzer
                    kostenlos ist.
                  </p>
                </div>
                <a href="" class="btn btn--border-white btn--dynamic-lg">
                  Schaltflächentext
                </a>
              </div>
              <div class="expert-card" v-for="user in users.slice(2)" :key="user.id+'mm'">
                <div class="expert-card__body">
                  <div class="expert-card__ava">
                    <div class="expert-card__status on"></div>
                    <img :src="require(`@/assets/img/${user.big_avatar}`)" alt="">
                  </div>
                  <div class="expert-card__inner">
                    <div class="expert-card__name">
                      Catherine
                    </div>
                    <ul class="expert-card__info">
                      <li>
                        <img src="@/assets/img/loc-icon.svg" alt="">
                        {{ user.location }}
                      </li>
                      <li>
                        <img src="@/assets/img/clock-icon.svg" alt="">
                        {{ user.term }}
                      </li>
                    </ul>
                    <div class="expert-card__block">
                      <div class="expert-card__block-row">
                        <div class="expert-card__exp expert-card__exp--green">
                          {{ user.status }}
                        </div>
                        <button class="expert-card__add-btn add-btn">
                          <svg width="16" height="14" viewBox="0 0 16 14" fill="none"
                               xmlns="http://www.w3.org/2000/svg">
                            <path
                              d="M14.2176 2.06106C12.7456 0.589021 10.3592 0.589021 8.88733 2.06106L7.99873 2.9495L7.11029 2.06122C5.63825 0.589178 3.2517 0.589178 1.77981 2.06122C0.307771 3.53326 0.307771 5.91966 1.77981 7.3917L2.66825 8.27967L7.99873 13.6101L13.3292 8.27967L14.2175 7.3917C15.6897 5.91966 15.6897 3.5331 14.2176 2.06106ZM11.5523 8.27998L7.99873 11.8336L4.44529 8.27998L2.66857 6.50326C1.68715 5.522 1.68715 3.93092 2.66857 2.94934C3.64998 1.96809 5.24091 1.96809 6.22217 2.94934L7.99873 4.72638L9.77561 2.9495C10.7569 1.96825 12.3479 1.96825 13.3292 2.9495C14.3105 3.93107 14.3105 5.52185 13.3292 6.50342L11.5523 8.27998Z"/>
                          </svg>
                        </button>
                      </div>
                      <div class="expert-card__block-row">
                        <div class="expert-card__reviews">
                          <div class="js-rating" data-rateyo-read-only="true" data-rating="5"></div>
                        </div>
                        <a href="" class="expert-card__review-link">
                          {{ user.review }} bewertungen
                        </a>
                      </div>
                    </div>
                    <p class="expert-card__text">
                      {{ user.text }}
                    </p>
                    <ul class="tags expert-card__tags">
                      <li class="tags__item" v-for="tag in user.tags" :key="tag+'aa'">
                        <a href="" class="tags__link">
                          <span>{{ tag }}</span>
                        </a>
                      </li>
                      <!--                      <li class="tags__item">-->
                      <!--                        <a href="" class="tags__link">-->
                      <!--                          <span>#Numerologie</span>-->
                      <!--                        </a>-->
                      <!--                      </li>-->
                      <!--                      <li class="tags__item">-->
                      <!--                        <a href="" class="tags__link">-->
                      <!--                          <span>#Hellsehen</span>-->
                      <!--                        </a>-->
                      <!--                      </li>-->
                    </ul>
                  </div>
                </div>
                <div class="expert-card__footer">
                  <div class="expert-card__price">
                    <div class="expert-card__price-value">
                      € 0/Min
                    </div>
                    <a href="" class="expert-card__price-btn green">
                      <span>Kostenlos anrufen</span>
                    </a>
                  </div>
                  <div class="expert-card__price">
                    <div class="expert-card__price-value">
                      € 0
                    </div>
                    <a href="" class="expert-card__price-btn border-green">
                      <span>Online-Chat kostenlos</span>
                    </a>
                  </div>
                </div>
              </div>
              <!--              <div class="expert-card">-->
              <!--                <div class="expert-card__body">-->
              <!--                  <div class="expert-card__ava">-->
              <!--                    <div class="expert-card__status on"></div>-->
              <!--                    <img src="img/big-ava.jpg" alt="">-->
              <!--                  </div>-->
              <!--                  <div class="expert-card__inner">-->
              <!--                    <div class="expert-card__name">-->
              <!--                      Catherine-->
              <!--                    </div>-->
              <!--                    <ul class="expert-card__info">-->
              <!--                      <li>-->
              <!--                        <img src="img/loc-icon.svg" alt="">-->
              <!--                        Deutschland, Berlin-->
              <!--                      </li>-->
              <!--                      <li>-->
              <!--                        <img src="img/clock-icon.svg" alt="">-->
              <!--                        Berufserfahrung 5 jahre-->
              <!--                      </li>-->
              <!--                    </ul>-->
              <!--                    <div class="expert-card__block">-->
              <!--                      <div class="expert-card__block-row">-->
              <!--                        <div class="expert-card__exp expert-card__exp&#45;&#45;green">-->
              <!--                          Neuling-->
              <!--                        </div>-->
              <!--                        <button class="expert-card__add-btn add-btn">-->
              <!--                          <svg width="16" height="14" viewBox="0 0 16 14" fill="none" xmlns="http://www.w3.org/2000/svg">-->
              <!--                            <path d="M14.2176 2.06106C12.7456 0.589021 10.3592 0.589021 8.88733 2.06106L7.99873 2.9495L7.11029 2.06122C5.63825 0.589178 3.2517 0.589178 1.77981 2.06122C0.307771 3.53326 0.307771 5.91966 1.77981 7.3917L2.66825 8.27967L7.99873 13.6101L13.3292 8.27967L14.2175 7.3917C15.6897 5.91966 15.6897 3.5331 14.2176 2.06106ZM11.5523 8.27998L7.99873 11.8336L4.44529 8.27998L2.66857 6.50326C1.68715 5.522 1.68715 3.93092 2.66857 2.94934C3.64998 1.96809 5.24091 1.96809 6.22217 2.94934L7.99873 4.72638L9.77561 2.9495C10.7569 1.96825 12.3479 1.96825 13.3292 2.9495C14.3105 3.93107 14.3105 5.52185 13.3292 6.50342L11.5523 8.27998Z"/>-->
              <!--                          </svg>-->
              <!--                        </button>-->
              <!--                      </div>-->
              <!--                      <div class="expert-card__block-row">-->
              <!--                        <div class="expert-card__reviews">-->
              <!--                          <div class="js-rating" data-rateyo-read-only="true" data-rating="5"></div>-->
              <!--                        </div>-->
              <!--                        <a href="" class="expert-card__review-link">-->
              <!--                          226 bewertungen-->
              <!--                        </a>-->
              <!--                      </div>-->
              <!--                    </div>-->
              <!--                    <p class="expert-card__text">-->
              <!--                      Hellsehen-fühlen ganz OHNE HilfsmittelnIch helfe Dir mit meinen Bildern Licht dunkeln zubringen. Gemeinsam schaffen wir das! Ich bin von Herzen für Dich da.️ Hellsehen-fühlen ganz OHNE HilfsmittelnIch helfe Dir mit...-->
              <!--                    </p>-->
              <!--                    <ul class="tags expert-card__tags">-->
              <!--                      <li class="tags__item">-->
              <!--                        <a href="" class="tags__link">-->
              <!--                          <span>#Astrologie</span>-->
              <!--                        </a>-->
              <!--                      </li>-->
              <!--                      <li class="tags__item">-->
              <!--                        <a href="" class="tags__link">-->
              <!--                          <span>#Numerologie</span>-->
              <!--                        </a>-->
              <!--                      </li>-->
              <!--                      <li class="tags__item">-->
              <!--                        <a href="" class="tags__link">-->
              <!--                          <span>#Hellsehen</span>-->
              <!--                        </a>-->
              <!--                      </li>-->
              <!--                    </ul>-->
              <!--                  </div>-->
              <!--                </div>-->
              <!--                <div class="expert-card__footer">-->
              <!--                  <div class="expert-card__price">-->
              <!--                    <div class="expert-card__price-value">-->
              <!--                      € 0/Min-->
              <!--                    </div>-->
              <!--                    <a href="" class="expert-card__price-btn green">-->
              <!--                      <span>Kostenlos anrufen</span>-->
              <!--                    </a>-->
              <!--                  </div>-->
              <!--                  <div class="expert-card__price">-->
              <!--                    <div class="expert-card__price-value">-->
              <!--                      € 0-->
              <!--                    </div>-->
              <!--                    <a href="" class="expert-card__price-btn border-green">-->
              <!--                      <span>Online-Chat kostenlos</span>-->
              <!--                    </a>-->
              <!--                  </div>-->
              <!--                </div>-->
              <!--              </div>-->
              <!--              <div class="expert-card">-->
              <!--                <div class="expert-card__body">-->
              <!--                  <div class="expert-card__ava">-->
              <!--                    <div class="expert-card__status off"></div>-->
              <!--                    <img src="img/big-ava.jpg" alt="">-->
              <!--                  </div>-->
              <!--                  <div class="expert-card__inner">-->
              <!--                    <div class="expert-card__name">-->
              <!--                      Catherine-->
              <!--                    </div>-->
              <!--                    <ul class="expert-card__info">-->
              <!--                      <li>-->
              <!--                        <img src="img/loc-icon.svg" alt="">-->
              <!--                        Deutschland, Berlin-->
              <!--                      </li>-->
              <!--                      <li>-->
              <!--                        <img src="img/clock-icon.svg" alt="">-->
              <!--                        Berufserfahrung 5 jahre-->
              <!--                      </li>-->
              <!--                    </ul>-->
              <!--                    <div class="expert-card__block">-->
              <!--                      <div class="expert-card__block-row">-->
              <!--                        <div class="expert-card__exp expert-card__exp&#45;&#45;purpure">-->
              <!--                          Exclusive-->
              <!--                        </div>-->
              <!--                        <button class="expert-card__add-btn add-btn">-->
              <!--                          <svg width="16" height="14" viewBox="0 0 16 14" fill="none" xmlns="http://www.w3.org/2000/svg">-->
              <!--                            <path d="M14.2176 2.06106C12.7456 0.589021 10.3592 0.589021 8.88733 2.06106L7.99873 2.9495L7.11029 2.06122C5.63825 0.589178 3.2517 0.589178 1.77981 2.06122C0.307771 3.53326 0.307771 5.91966 1.77981 7.3917L2.66825 8.27967L7.99873 13.6101L13.3292 8.27967L14.2175 7.3917C15.6897 5.91966 15.6897 3.5331 14.2176 2.06106ZM11.5523 8.27998L7.99873 11.8336L4.44529 8.27998L2.66857 6.50326C1.68715 5.522 1.68715 3.93092 2.66857 2.94934C3.64998 1.96809 5.24091 1.96809 6.22217 2.94934L7.99873 4.72638L9.77561 2.9495C10.7569 1.96825 12.3479 1.96825 13.3292 2.9495C14.3105 3.93107 14.3105 5.52185 13.3292 6.50342L11.5523 8.27998Z"/>-->
              <!--                          </svg>-->
              <!--                        </button>-->
              <!--                      </div>-->
              <!--                      <div class="expert-card__block-row">-->
              <!--                        <div class="expert-card__reviews">-->
              <!--                          <div class="js-rating" data-rateyo-read-only="true" data-rating="5"></div>-->
              <!--                        </div>-->
              <!--                        <a href="" class="expert-card__review-link">-->
              <!--                          226 bewertungen-->
              <!--                        </a>-->
              <!--                      </div>-->
              <!--                    </div>-->
              <!--                    <p class="expert-card__text">-->
              <!--                      Hellsehen-fühlen ganz OHNE HilfsmittelnIch helfe Dir mit meinen Bildern Licht dunkeln zubringen. Gemeinsam schaffen wir das! Ich bin von Herzen für Dich da.️ Hellsehen-fühlen ganz OHNE HilfsmittelnIch helfe Dir mit...-->
              <!--                    </p>-->
              <!--                    <ul class="tags expert-card__tags">-->
              <!--                      <li class="tags__item">-->
              <!--                        <a href="" class="tags__link">-->
              <!--                          <span>#Astrologie</span>-->
              <!--                        </a>-->
              <!--                      </li>-->
              <!--                      <li class="tags__item">-->
              <!--                        <a href="" class="tags__link">-->
              <!--                          <span>#Numerologie</span>-->
              <!--                        </a>-->
              <!--                      </li>-->
              <!--                      <li class="tags__item">-->
              <!--                        <a href="" class="tags__link">-->
              <!--                          <span>#Hellsehen</span>-->
              <!--                        </a>-->
              <!--                      </li>-->
              <!--                    </ul>-->
              <!--                  </div>-->
              <!--                </div>-->
              <!--                <div class="expert-card__footer">-->
              <!--                  <div class="expert-card__price">-->
              <!--                    <div class="expert-card__price-value">-->
              <!--                      € 0/Min-->
              <!--                    </div>-->
              <!--                    <a href="" class="expert-card__price-btn purpure">-->
              <!--                      <span>Zeit buchen</span>-->
              <!--                    </a>-->
              <!--                  </div>-->
              <!--                  <div class="expert-card__price">-->
              <!--                    <div class="expert-card__price-value">-->
              <!--                      € 0-->
              <!--                    </div>-->
              <!--                    <a href="" class="expert-card__price-btn border-purpure">-->
              <!--                      <span>Online-Chat kostenlos</span>-->
              <!--                    </a>-->
              <!--                  </div>-->
              <!--                </div>-->
              <!--              </div>-->
              <!--              <div class="expert-card">-->
              <!--                <div class="expert-card__body">-->
              <!--                  <div class="expert-card__ava">-->
              <!--                    <div class="expert-card__status on"></div>-->
              <!--                    <img src="img/big-ava.jpg" alt="">-->
              <!--                  </div>-->
              <!--                  <div class="expert-card__inner">-->
              <!--                    <div class="expert-card__name">-->
              <!--                      Catherine-->
              <!--                    </div>-->
              <!--                    <ul class="expert-card__info">-->
              <!--                      <li>-->
              <!--                        <img src="img/loc-icon.svg" alt="">-->
              <!--                        Deutschland, Berlin-->
              <!--                      </li>-->
              <!--                      <li>-->
              <!--                        <img src="img/clock-icon.svg" alt="">-->
              <!--                        Berufserfahrung 5 jahre-->
              <!--                      </li>-->
              <!--                    </ul>-->
              <!--                    <div class="expert-card__block">-->
              <!--                      <div class="expert-card__block-row">-->
              <!--                        <div class="expert-card__exp expert-card__exp&#45;&#45;green">-->
              <!--                          Neuling-->
              <!--                        </div>-->
              <!--                        <button class="expert-card__add-btn add-btn">-->
              <!--                          <svg width="16" height="14" viewBox="0 0 16 14" fill="none" xmlns="http://www.w3.org/2000/svg">-->
              <!--                            <path d="M14.2176 2.06106C12.7456 0.589021 10.3592 0.589021 8.88733 2.06106L7.99873 2.9495L7.11029 2.06122C5.63825 0.589178 3.2517 0.589178 1.77981 2.06122C0.307771 3.53326 0.307771 5.91966 1.77981 7.3917L2.66825 8.27967L7.99873 13.6101L13.3292 8.27967L14.2175 7.3917C15.6897 5.91966 15.6897 3.5331 14.2176 2.06106ZM11.5523 8.27998L7.99873 11.8336L4.44529 8.27998L2.66857 6.50326C1.68715 5.522 1.68715 3.93092 2.66857 2.94934C3.64998 1.96809 5.24091 1.96809 6.22217 2.94934L7.99873 4.72638L9.77561 2.9495C10.7569 1.96825 12.3479 1.96825 13.3292 2.9495C14.3105 3.93107 14.3105 5.52185 13.3292 6.50342L11.5523 8.27998Z"/>-->
              <!--                          </svg>-->
              <!--                        </button>-->
              <!--                      </div>-->
              <!--                      <div class="expert-card__block-row">-->
              <!--                        <div class="expert-card__reviews">-->
              <!--                          <div class="js-rating" data-rateyo-read-only="true" data-rating="5"></div>-->
              <!--                        </div>-->
              <!--                        <a href="" class="expert-card__review-link">-->
              <!--                          226 bewertungen-->
              <!--                        </a>-->
              <!--                      </div>-->
              <!--                    </div>-->
              <!--                    <p class="expert-card__text">-->
              <!--                      Hellsehen-fühlen ganz OHNE HilfsmittelnIch helfe Dir mit meinen Bildern Licht dunkeln zubringen. Gemeinsam schaffen wir das! Ich bin von Herzen für Dich da.️ Hellsehen-fühlen ganz OHNE HilfsmittelnIch helfe Dir mit...-->
              <!--                    </p>-->
              <!--                    <ul class="tags expert-card__tags">-->
              <!--                      <li class="tags__item">-->
              <!--                        <a href="" class="tags__link">-->
              <!--                          <span>#Astrologie</span>-->
              <!--                        </a>-->
              <!--                      </li>-->
              <!--                      <li class="tags__item">-->
              <!--                        <a href="" class="tags__link">-->
              <!--                          <span>#Numerologie</span>-->
              <!--                        </a>-->
              <!--                      </li>-->
              <!--                      <li class="tags__item">-->
              <!--                        <a href="" class="tags__link">-->
              <!--                          <span>#Hellsehen</span>-->
              <!--                        </a>-->
              <!--                      </li>-->
              <!--                    </ul>-->
              <!--                  </div>-->
              <!--                </div>-->
              <!--                <div class="expert-card__footer">-->
              <!--                  <div class="expert-card__price">-->
              <!--                    <div class="expert-card__price-value">-->
              <!--                      € 0/Min-->
              <!--                    </div>-->
              <!--                    <a href="" class="expert-card__price-btn green">-->
              <!--                      <span>Kostenlos anrufen</span>-->
              <!--                    </a>-->
              <!--                  </div>-->
              <!--                  <div class="expert-card__price">-->
              <!--                    <div class="expert-card__price-value">-->
              <!--                      € 0-->
              <!--                    </div>-->
              <!--                    <a href="" class="expert-card__price-btn border-green">-->
              <!--                      <span>Online-Chat kostenlos</span>-->
              <!--                    </a>-->
              <!--                  </div>-->
              <!--                </div>-->
              <!--              </div>-->
              <!--              <div class="expert-card">-->
              <!--                <div class="expert-card__body">-->
              <!--                  <div class="expert-card__ava">-->
              <!--                    <div class="expert-card__status on"></div>-->
              <!--                    <img src="img/big-ava.jpg" alt="">-->
              <!--                  </div>-->
              <!--                  <div class="expert-card__inner">-->
              <!--                    <div class="expert-card__name">-->
              <!--                      Catherine-->
              <!--                    </div>-->
              <!--                    <ul class="expert-card__info">-->
              <!--                      <li>-->
              <!--                        <img src="img/loc-icon.svg" alt="">-->
              <!--                        Deutschland, Berlin-->
              <!--                      </li>-->
              <!--                      <li>-->
              <!--                        <img src="img/clock-icon.svg" alt="">-->
              <!--                        Berufserfahrung 5 jahre-->
              <!--                      </li>-->
              <!--                    </ul>-->
              <!--                    <div class="expert-card__block">-->
              <!--                      <div class="expert-card__block-row">-->
              <!--                        <div class="expert-card__exp expert-card__exp&#45;&#45;green">-->
              <!--                          Neuling-->
              <!--                        </div>-->
              <!--                        <button class="expert-card__add-btn add-btn">-->
              <!--                          <svg width="16" height="14" viewBox="0 0 16 14" fill="none" xmlns="http://www.w3.org/2000/svg">-->
              <!--                            <path d="M14.2176 2.06106C12.7456 0.589021 10.3592 0.589021 8.88733 2.06106L7.99873 2.9495L7.11029 2.06122C5.63825 0.589178 3.2517 0.589178 1.77981 2.06122C0.307771 3.53326 0.307771 5.91966 1.77981 7.3917L2.66825 8.27967L7.99873 13.6101L13.3292 8.27967L14.2175 7.3917C15.6897 5.91966 15.6897 3.5331 14.2176 2.06106ZM11.5523 8.27998L7.99873 11.8336L4.44529 8.27998L2.66857 6.50326C1.68715 5.522 1.68715 3.93092 2.66857 2.94934C3.64998 1.96809 5.24091 1.96809 6.22217 2.94934L7.99873 4.72638L9.77561 2.9495C10.7569 1.96825 12.3479 1.96825 13.3292 2.9495C14.3105 3.93107 14.3105 5.52185 13.3292 6.50342L11.5523 8.27998Z"/>-->
              <!--                          </svg>-->
              <!--                        </button>-->
              <!--                      </div>-->
              <!--                      <div class="expert-card__block-row">-->
              <!--                        <div class="expert-card__reviews">-->
              <!--                          <div class="js-rating" data-rateyo-read-only="true" data-rating="5"></div>-->
              <!--                        </div>-->
              <!--                        <a href="" class="expert-card__review-link">-->
              <!--                          226 bewertungen-->
              <!--                        </a>-->
              <!--                      </div>-->
              <!--                    </div>-->
              <!--                    <p class="expert-card__text">-->
              <!--                      Hellsehen-fühlen ganz OHNE HilfsmittelnIch helfe Dir mit meinen Bildern Licht dunkeln zubringen. Gemeinsam schaffen wir das! Ich bin von Herzen für Dich da.️ Hellsehen-fühlen ganz OHNE HilfsmittelnIch helfe Dir mit...-->
              <!--                    </p>-->
              <!--                    <ul class="tags expert-card__tags">-->
              <!--                      <li class="tags__item">-->
              <!--                        <a href="" class="tags__link">-->
              <!--                          <span>#Astrologie</span>-->
              <!--                        </a>-->
              <!--                      </li>-->
              <!--                      <li class="tags__item">-->
              <!--                        <a href="" class="tags__link">-->
              <!--                          <span>#Numerologie</span>-->
              <!--                        </a>-->
              <!--                      </li>-->
              <!--                      <li class="tags__item">-->
              <!--                        <a href="" class="tags__link">-->
              <!--                          <span>#Hellsehen</span>-->
              <!--                        </a>-->
              <!--                      </li>-->
              <!--                    </ul>-->
              <!--                  </div>-->
              <!--                </div>-->
              <!--                <div class="expert-card__footer">-->
              <!--                  <div class="expert-card__price">-->
              <!--                    <div class="expert-card__price-value">-->
              <!--                      € 0/Min-->
              <!--                    </div>-->
              <!--                    <a href="" class="expert-card__price-btn green">-->
              <!--                      <span>Kostenlos anrufen</span>-->
              <!--                    </a>-->
              <!--                  </div>-->
              <!--                  <div class="expert-card__price">-->
              <!--                    <div class="expert-card__price-value">-->
              <!--                      € 0-->
              <!--                    </div>-->
              <!--                    <a href="" class="expert-card__price-btn border-green">-->
              <!--                      <span>Online-Chat kostenlos</span>-->
              <!--                    </a>-->
              <!--                  </div>-->
              <!--                </div>-->
              <!--              </div>-->
              <!--              <div class="expert-card">-->
              <!--                <div class="expert-card__body">-->
              <!--                  <div class="expert-card__ava">-->
              <!--                    <div class="expert-card__status off"></div>-->
              <!--                    <img src="img/big-ava.jpg" alt="">-->
              <!--                  </div>-->
              <!--                  <div class="expert-card__inner">-->
              <!--                    <div class="expert-card__name">-->
              <!--                      Catherine-->
              <!--                    </div>-->
              <!--                    <ul class="expert-card__info">-->
              <!--                      <li>-->
              <!--                        <img src="img/loc-icon.svg" alt="">-->
              <!--                        Deutschland, Berlin-->
              <!--                      </li>-->
              <!--                      <li>-->
              <!--                        <img src="img/clock-icon.svg" alt="">-->
              <!--                        Berufserfahrung 5 jahre-->
              <!--                      </li>-->
              <!--                    </ul>-->
              <!--                    <div class="expert-card__block">-->
              <!--                      <div class="expert-card__block-row">-->
              <!--                        <div class="expert-card__exp expert-card__exp&#45;&#45;purpure">-->
              <!--                          Exclusive-->
              <!--                        </div>-->
              <!--                        <button class="expert-card__add-btn add-btn">-->
              <!--                          <svg width="16" height="14" viewBox="0 0 16 14" fill="none" xmlns="http://www.w3.org/2000/svg">-->
              <!--                            <path d="M14.2176 2.06106C12.7456 0.589021 10.3592 0.589021 8.88733 2.06106L7.99873 2.9495L7.11029 2.06122C5.63825 0.589178 3.2517 0.589178 1.77981 2.06122C0.307771 3.53326 0.307771 5.91966 1.77981 7.3917L2.66825 8.27967L7.99873 13.6101L13.3292 8.27967L14.2175 7.3917C15.6897 5.91966 15.6897 3.5331 14.2176 2.06106ZM11.5523 8.27998L7.99873 11.8336L4.44529 8.27998L2.66857 6.50326C1.68715 5.522 1.68715 3.93092 2.66857 2.94934C3.64998 1.96809 5.24091 1.96809 6.22217 2.94934L7.99873 4.72638L9.77561 2.9495C10.7569 1.96825 12.3479 1.96825 13.3292 2.9495C14.3105 3.93107 14.3105 5.52185 13.3292 6.50342L11.5523 8.27998Z"/>-->
              <!--                          </svg>-->
              <!--                        </button>-->
              <!--                      </div>-->
              <!--                      <div class="expert-card__block-row">-->
              <!--                        <div class="expert-card__reviews">-->
              <!--                          <div class="js-rating" data-rateyo-read-only="true" data-rating="5"></div>-->
              <!--                        </div>-->
              <!--                        <a href="" class="expert-card__review-link">-->
              <!--                          226 bewertungen-->
              <!--                        </a>-->
              <!--                      </div>-->
              <!--                    </div>-->
              <!--                    <p class="expert-card__text">-->
              <!--                      Hellsehen-fühlen ganz OHNE HilfsmittelnIch helfe Dir mit meinen Bildern Licht dunkeln zubringen. Gemeinsam schaffen wir das! Ich bin von Herzen für Dich da.️ Hellsehen-fühlen ganz OHNE HilfsmittelnIch helfe Dir mit...-->
              <!--                    </p>-->
              <!--                    <ul class="tags expert-card__tags">-->
              <!--                      <li class="tags__item">-->
              <!--                        <a href="" class="tags__link">-->
              <!--                          <span>#Astrologie</span>-->
              <!--                        </a>-->
              <!--                      </li>-->
              <!--                      <li class="tags__item">-->
              <!--                        <a href="" class="tags__link">-->
              <!--                          <span>#Numerologie</span>-->
              <!--                        </a>-->
              <!--                      </li>-->
              <!--                      <li class="tags__item">-->
              <!--                        <a href="" class="tags__link">-->
              <!--                          <span>#Hellsehen</span>-->
              <!--                        </a>-->
              <!--                      </li>-->
              <!--                    </ul>-->
              <!--                  </div>-->
              <!--                </div>-->
              <!--                <div class="expert-card__footer">-->
              <!--                  <div class="expert-card__price">-->
              <!--                    <div class="expert-card__price-value">-->
              <!--                      € 0/Min-->
              <!--                    </div>-->
              <!--                    <a href="" class="expert-card__price-btn purpure">-->
              <!--                      <span>Zeit buchen</span>-->
              <!--                    </a>-->
              <!--                  </div>-->
              <!--                  <div class="expert-card__price">-->
              <!--                    <div class="expert-card__price-value">-->
              <!--                      € 0-->
              <!--                    </div>-->
              <!--                    <a href="" class="expert-card__price-btn border-purpure">-->
              <!--                      <span>Online-Chat kostenlos</span>-->
              <!--                    </a>-->
              <!--                  </div>-->
              <!--                </div>-->
              <!--              </div>-->
            </div>
          </div>
          <div class="col-lg-9 offset-lg-3">
            <div class="expert-cards__footer">
              <ul class="pagenav">
                <li class="pagenav__item">
                  <a href="" class="pagenav__prev">
                    <svg width="13" height="11" viewBox="0 0 13 11" fill="none" xmlns="http://www.w3.org/2000/svg">
                      <path d="M4.92883 1L1.00228 5.52108L4.92883 9.63636M1 5.48125H11.3636H1Z" stroke-width="1.6"
                            stroke-linecap="round" stroke-linejoin="round"/>
                    </svg>
                  </a>
                </li>
                <li class="pagenav__item active">
                  <a href="" class="pagenav__link">
                    1
                  </a>
                </li>
                <li class="pagenav__item">
                  <a href="" class="pagenav__link">
                    2
                  </a>
                </li>
                <li class="pagenav__item">
                  <a href="" class="pagenav__link">
                    3
                  </a>
                </li>
                <li class="pagenav__item">
                  <a href="" class="pagenav__link">
                    ...
                  </a>
                </li>
                <li class="pagenav__item">
                  <a href="" class="pagenav__link">
                    81
                  </a>
                </li>
                <li class="pagenav__item">
                  <a href="" class="pagenav__next">
                    <svg width="13" height="11" viewBox="0 0 13 11" fill="none" xmlns="http://www.w3.org/2000/svg">
                      <path d="M7.79773 1L11.7243 5.52108L7.79773 9.63636M11.7266 5.48125H1.36293H11.7266Z"
                            stroke-width="1.6" stroke-linecap="round" stroke-linejoin="round"/>
                    </svg>
                  </a>
                </li>
              </ul>
            </div>
          </div>
        </div>
      </div>
    </section>
    <section class="section services-section pt-lg pb-lg">
      <div class="container">
        <div class="row">
          <div class="col-12">
            <div class="section__header section__header--white">
              <div class="section__line section__line--light">
                <svg data-aos="zoom-in" data-aos-delay="600" class="section__line-dot" width="3" height="3"
                     viewBox="0 0 3 3" fill="none" xmlns="http://www.w3.org/2000/svg">
                  <circle cx="1.5" cy="1.5" r="1.5"/>
                </svg>
                <svg data-aos="zoom-left" data-aos-delay="400" class="section__line-line" width="623" height="1"
                     viewBox="0 0 623 1" fill="none" xmlns="http://www.w3.org/2000/svg">
                  <line x1="4.37114e-08" y1="0.5" x2="623" y2="0.500054"/>
                </svg>
                <svg data-aos="zoom-in" data-aos-delay="200" class="section__line-dot" width="3" height="3"
                     viewBox="0 0 3 3" fill="none" xmlns="http://www.w3.org/2000/svg">
                  <circle cx="1.5" cy="1.5" r="1.5"/>
                </svg>
                <svg data-aos="zoom-in" class="section__line-middle" width="30" height="30" viewBox="0 0 30 30"
                     fill="none" xmlns="http://www.w3.org/2000/svg">
                  <circle cx="15" cy="15" r="14.3" stroke="#D5D9E0" stroke-width="1.4"/>
                  <rect x="21.5" y="12.3789" width="3" height="3" transform="rotate(45 21.5 12.3789)" fill="#D5D9E0"/>
                  <path
                    d="M12.7746 7.75105C13.7767 7.24352 14.8952 6.9894 16.0099 7.00034C17.1553 7.01446 18.3013 7.31022 19.3085 7.87811V7.88623C18.9452 7.98187 18.6091 8.16646 18.2747 8.3394C17.1859 8.94717 16.2678 9.87506 15.6415 10.9805C15.0935 11.9394 14.7676 13.0343 14.7071 14.1478C14.6292 15.5334 14.9503 16.9427 15.6266 18.1413C16.412 19.5457 17.6846 20.6366 19.1449 21.2112C18.2564 21.6739 17.2736 21.9383 16.281 21.9905C14.9411 22.0636 13.5832 21.7371 12.4127 21.0559C11.5 20.5283 10.6962 19.797 10.0815 18.9196C9.21543 17.6917 8.73001 16.185 8.69531 14.6652V14.3006C8.73443 12.7921 9.22223 11.2999 10.0839 10.0836C10.7771 9.09188 11.7089 8.27976 12.7746 7.75105Z"
                    fill="#D5D9E0"/>
                </svg>
                <svg data-aos="zoom-in" data-aos-delay="200" class="section__line-dot" width="3" height="3"
                     viewBox="0 0 3 3" fill="none" xmlns="http://www.w3.org/2000/svg">
                  <circle cx="1.5" cy="1.5" r="1.5"/>
                </svg>
                <svg data-aos="zoom-left" data-aos-delay="400" class="section__line-line" width="623" height="1"
                     viewBox="0 0 623 1" fill="none" xmlns="http://www.w3.org/2000/svg">
                  <line x1="4.37114e-08" y1="0.5" x2="623" y2="0.500054"/>
                </svg>
                <svg data-aos="zoom-in" data-aos-delay="600" class="section__line-dot" width="3" height="3"
                     viewBox="0 0 3 3" fill="none" xmlns="http://www.w3.org/2000/svg">
                  <circle cx="1.5" cy="1.5" r="1.5"/>
                </svg>
              </div>
              <h2 class="section__title" data-aos="fade-up">
                Dienstleistungen
              </h2>
            </div>
            <div class="services-slider">
              <carouselxx :slideValue="slideController" :nav="false" :lazyLoad="true" :loop="true" :rewind="false"
                          :items="3"
                          :autoWidth="false" :margin="20" :dots="false"
                          :responsive="{0:{items:1},350:{items:1},600:{items:1},1024:{items:3},1280:{items:3}}"
                          :class="['carousel__service']">
                <div class="services-slider__item" v-for="service in services" :key="service.id">
                  <div class="service-card">
                    <button class="service-card__add-btn add-btn">
                      <svg width="16" height="14" viewBox="0 0 16 14" fill="none" xmlns="http://www.w3.org/2000/svg">
                        <path
                          d="M14.2176 2.06106C12.7456 0.589021 10.3592 0.589021 8.88733 2.06106L7.99873 2.9495L7.11029 2.06122C5.63825 0.589178 3.2517 0.589178 1.77981 2.06122C0.307771 3.53326 0.307771 5.91966 1.77981 7.3917L2.66825 8.27967L7.99873 13.6101L13.3292 8.27967L14.2175 7.3917C15.6897 5.91966 15.6897 3.5331 14.2176 2.06106ZM11.5523 8.27998L7.99873 11.8336L4.44529 8.27998L2.66857 6.50326C1.68715 5.522 1.68715 3.93092 2.66857 2.94934C3.64998 1.96809 5.24091 1.96809 6.22217 2.94934L7.99873 4.72638L9.77561 2.9495C10.7569 1.96825 12.3479 1.96825 13.3292 2.9495C14.3105 3.93107 14.3105 5.52185 13.3292 6.50342L11.5523 8.27998Z"/>
                      </svg>
                    </button>
                    <div class="service-card__img">
                      <img :src="require(`@/assets/img/${service.service_card}`)" alt="">
                    </div>
                    <div class="service-card__content">
                      <div class="service-card__header">
                        <div class="service-card__author">
                          <div class="service-card__author-ava">
                            <img :src="require(`@/assets/img/${service.avatar}`)" alt="">
                          </div>
                          <div class="service-card__author-inner">
                            <div class="service-card__author-title">
                              Autor
                            </div>
                            <a href="" class="service-card__author-name">
                              {{ service.author }}
                            </a>
                          </div>
                        </div>
                        <div class="service-card__reviews">
                          <div class="service-card__reviews-rate js-rating" data-rateyo-read-only="true"
                               data-rating="2"></div>
                          <a href="" class="service-card__reviews-link">{{ service.reviews }} bewertungen</a>
                        </div>
                      </div>
                      <a href="" class="service-card__title">
                        {{ service.title }}
                      </a>
                      <div class="service-card__text">
                        {{ service.text }}
                      </div>
                      <div class="service-card__footer">
                        <div class="service-card__price">
                          € {{ service.price }}
                        </div>
                        <a href="" class="btn btn--main btn--static">
                          <span>Mehr Details</span>
                        </a>
                      </div>
                    </div>
                  </div>
                </div>
              </carouselxx>
              <!--              <div class="services-slider__item">-->
              <!--                <div class="service-card">-->
              <!--                  <button class="service-card__add-btn add-btn">-->
              <!--                    <svg width="16" height="14" viewBox="0 0 16 14" fill="none" xmlns="http://www.w3.org/2000/svg">-->
              <!--                      <path d="M14.2176 2.06106C12.7456 0.589021 10.3592 0.589021 8.88733 2.06106L7.99873 2.9495L7.11029 2.06122C5.63825 0.589178 3.2517 0.589178 1.77981 2.06122C0.307771 3.53326 0.307771 5.91966 1.77981 7.3917L2.66825 8.27967L7.99873 13.6101L13.3292 8.27967L14.2175 7.3917C15.6897 5.91966 15.6897 3.5331 14.2176 2.06106ZM11.5523 8.27998L7.99873 11.8336L4.44529 8.27998L2.66857 6.50326C1.68715 5.522 1.68715 3.93092 2.66857 2.94934C3.64998 1.96809 5.24091 1.96809 6.22217 2.94934L7.99873 4.72638L9.77561 2.9495C10.7569 1.96825 12.3479 1.96825 13.3292 2.9495C14.3105 3.93107 14.3105 5.52185 13.3292 6.50342L11.5523 8.27998Z"/>-->
              <!--                    </svg>-->
              <!--                  </button>-->
              <!--                  <div class="service-card__img">-->
              <!--                    <img src="img/service-card-img.jpg" alt="">-->
              <!--                  </div>-->
              <!--                  <div class="service-card__content">-->
              <!--                    <div class="service-card__header">-->
              <!--                      <div class="service-card__author">-->
              <!--                        <div class="service-card__author-ava">-->
              <!--                          <img src="img/ava.png" alt="">-->
              <!--                        </div>-->
              <!--                        <div class="service-card__author-inner">-->
              <!--                          <div class="service-card__author-title">-->
              <!--                            Autor-->
              <!--                          </div>-->
              <!--                          <a href="" class="service-card__author-name">-->
              <!--                            Catherine-->
              <!--                          </a>-->
              <!--                        </div>-->
              <!--                      </div>-->
              <!--                      <div class="service-card__reviews">-->
              <!--                        <div class="service-card__reviews-rate js-rating" data-rateyo-read-only="true" data-rating="2"></div>-->
              <!--                        <a href="" class="service-card__reviews-link">226 bewertungen</a>-->
              <!--                      </div>-->
              <!--                    </div>-->
              <!--                    <a href="" class="service-card__title">-->
              <!--                      Astrologische Vorhersage von Liebe und Familienleben für ein Jahr-->
              <!--                    </a>-->
              <!--                    <div class="service-card__text">-->
              <!--                      Aus der astrologischen Vorhersage erfahren Sie, welche Ereignisse in Ihrem persönlichen Leben Sie im Laufe des Jahres erwarten.-->
              <!--                    </div>-->
              <!--                    <div class="service-card__footer">-->
              <!--                      <div class="service-card__price">-->
              <!--                        € 50-->
              <!--                      </div>-->
              <!--                      <a href="" class="btn btn&#45;&#45;main btn&#45;&#45;static">-->
              <!--                        <span>Mehr Details</span>-->
              <!--                      </a>-->
              <!--                    </div>-->
              <!--                  </div>-->
              <!--                </div>-->
              <!--              </div>-->
              <!--              <div class="services-slider__item">-->
              <!--                <div class="service-card">-->
              <!--                  <button class="service-card__add-btn add-btn">-->
              <!--                    <svg width="16" height="14" viewBox="0 0 16 14" fill="none" xmlns="http://www.w3.org/2000/svg">-->
              <!--                      <path d="M14.2176 2.06106C12.7456 0.589021 10.3592 0.589021 8.88733 2.06106L7.99873 2.9495L7.11029 2.06122C5.63825 0.589178 3.2517 0.589178 1.77981 2.06122C0.307771 3.53326 0.307771 5.91966 1.77981 7.3917L2.66825 8.27967L7.99873 13.6101L13.3292 8.27967L14.2175 7.3917C15.6897 5.91966 15.6897 3.5331 14.2176 2.06106ZM11.5523 8.27998L7.99873 11.8336L4.44529 8.27998L2.66857 6.50326C1.68715 5.522 1.68715 3.93092 2.66857 2.94934C3.64998 1.96809 5.24091 1.96809 6.22217 2.94934L7.99873 4.72638L9.77561 2.9495C10.7569 1.96825 12.3479 1.96825 13.3292 2.9495C14.3105 3.93107 14.3105 5.52185 13.3292 6.50342L11.5523 8.27998Z"/>-->
              <!--                    </svg>-->
              <!--                  </button>-->
              <!--                  <div class="service-card__img">-->
              <!--                    <img src="img/service-card-img.jpg" alt="">-->
              <!--                  </div>-->
              <!--                  <div class="service-card__content">-->
              <!--                    <div class="service-card__header">-->
              <!--                      <div class="service-card__author">-->
              <!--                        <div class="service-card__author-ava">-->
              <!--                          <img src="img/ava.png" alt="">-->
              <!--                        </div>-->
              <!--                        <div class="service-card__author-inner">-->
              <!--                          <div class="service-card__author-title">-->
              <!--                            Autor-->
              <!--                          </div>-->
              <!--                          <a href="" class="service-card__author-name">-->
              <!--                            Catherine-->
              <!--                          </a>-->
              <!--                        </div>-->
              <!--                      </div>-->
              <!--                      <div class="service-card__reviews">-->
              <!--                        <div class="service-card__reviews-rate js-rating" data-rateyo-read-only="true" data-rating="2"></div>-->
              <!--                        <a href="" class="service-card__reviews-link">226 bewertungen</a>-->
              <!--                      </div>-->
              <!--                    </div>-->
              <!--                    <a href="" class="service-card__title">-->
              <!--                      Astrologische Vorhersage-->
              <!--                    </a>-->
              <!--                    <div class="service-card__text">-->
              <!--                      Aus der astrologischen-->
              <!--                    </div>-->
              <!--                    <div class="service-card__footer">-->
              <!--                      <div class="service-card__price">-->
              <!--                        € 50-->
              <!--                      </div>-->
              <!--                      <a href="" class="btn btn&#45;&#45;main btn&#45;&#45;static">-->
              <!--                        <span>Mehr Details</span>-->
              <!--                      </a>-->
              <!--                    </div>-->
              <!--                  </div>-->
              <!--                </div>-->
              <!--              </div>-->
              <!--              <div class="services-slider__item">-->
              <!--                <div class="service-card">-->
              <!--                  <button class="service-card__add-btn add-btn">-->
              <!--                    <svg width="16" height="14" viewBox="0 0 16 14" fill="none" xmlns="http://www.w3.org/2000/svg">-->
              <!--                      <path d="M14.2176 2.06106C12.7456 0.589021 10.3592 0.589021 8.88733 2.06106L7.99873 2.9495L7.11029 2.06122C5.63825 0.589178 3.2517 0.589178 1.77981 2.06122C0.307771 3.53326 0.307771 5.91966 1.77981 7.3917L2.66825 8.27967L7.99873 13.6101L13.3292 8.27967L14.2175 7.3917C15.6897 5.91966 15.6897 3.5331 14.2176 2.06106ZM11.5523 8.27998L7.99873 11.8336L4.44529 8.27998L2.66857 6.50326C1.68715 5.522 1.68715 3.93092 2.66857 2.94934C3.64998 1.96809 5.24091 1.96809 6.22217 2.94934L7.99873 4.72638L9.77561 2.9495C10.7569 1.96825 12.3479 1.96825 13.3292 2.9495C14.3105 3.93107 14.3105 5.52185 13.3292 6.50342L11.5523 8.27998Z"/>-->
              <!--                    </svg>-->
              <!--                  </button>-->
              <!--                  <div class="service-card__img">-->
              <!--                    <img src="img/service-card-img.jpg" alt="">-->
              <!--                  </div>-->
              <!--                  <div class="service-card__content">-->
              <!--                    <div class="service-card__header">-->
              <!--                      <div class="service-card__author">-->
              <!--                        <div class="service-card__author-ava">-->
              <!--                          <img src="img/ava.png" alt="">-->
              <!--                        </div>-->
              <!--                        <div class="service-card__author-inner">-->
              <!--                          <div class="service-card__author-title">-->
              <!--                            Autor-->
              <!--                          </div>-->
              <!--                          <a href="" class="service-card__author-name">-->
              <!--                            Catherine-->
              <!--                          </a>-->
              <!--                        </div>-->
              <!--                      </div>-->
              <!--                      <div class="service-card__reviews">-->
              <!--                        <div class="service-card__reviews-rate js-rating" data-rateyo-read-only="true" data-rating="2"></div>-->
              <!--                        <a href="" class="service-card__reviews-link">226 bewertungen</a>-->
              <!--                      </div>-->
              <!--                    </div>-->
              <!--                    <a href="" class="service-card__title">-->
              <!--                      Astrologische Vorhersage von Liebe und Familienleben für ein Jahr-->
              <!--                    </a>-->
              <!--                    <div class="service-card__text">-->
              <!--                      Aus der astrologischen Vorhersage erfahren Sie, welche Ereignisse in Ihrem persönlichen Leben Sie im Laufe des Jahres erwarten.-->
              <!--                    </div>-->
              <!--                    <div class="service-card__footer">-->
              <!--                      <div class="service-card__price">-->
              <!--                        € 50-->
              <!--                      </div>-->
              <!--                      <a href="" class="btn btn&#45;&#45;main btn&#45;&#45;static">-->
              <!--                        <span>Mehr Details</span>-->
              <!--                      </a>-->
              <!--                    </div>-->
              <!--                  </div>-->
              <!--                </div>-->
              <!--              </div>-->
            </div>
            <div class="services-section__footer">
              <button class="services-section__arr-prev slider-arr slider-arr--white" @click="slideController--">
                <svg width="12" height="12" viewBox="0 0 12 12" fill="none" xmlns="http://www.w3.org/2000/svg">
                  <path d="M4.74524 1.68164L0.818687 6.20272L4.74524 10.318M0.816406 6.16289H11.18H0.816406Z"
                        stroke-width="1.6" stroke-linecap="round" stroke-linejoin="round"/>
                </svg>
              </button>
              <a href="" class="btn btn--border-white btn--static">
                <span>Zeige alles</span>
              </a>
              <button class="services-section__arr-next slider-arr slider-arr--white" @click="slideController++">
                <svg width="12" height="12" viewBox="0 0 12 12" fill="none" xmlns="http://www.w3.org/2000/svg">
                  <path d="M7.25476 1.68164L11.1813 6.20272L7.25476 10.318M11.1836 6.16289H0.819958H11.1836Z"
                        stroke-width="1.6" stroke-linecap="round" stroke-linejoin="round"/>
                </svg>
              </button>
            </div>
          </div>
        </div>
      </div>
    </section>
    <section class="reviews-section pt-lg pb-lg">
      <div class="container-fluid">
        <div class="row">
          <div class="col-12">
            <div class="section__header">
              <div class="section__line">
                <svg data-aos="zoom-in" data-aos-delay="600" class="section__line-dot" width="3" height="3"
                     viewBox="0 0 3 3" fill="none" xmlns="http://www.w3.org/2000/svg">
                  <circle cx="1.5" cy="1.5" r="1.5"/>
                </svg>
                <svg data-aos="zoom-right" data-aos-delay="400" class="section__line-line" width="623" height="1"
                     viewBox="0 0 623 1" fill="none" xmlns="http://www.w3.org/2000/svg">
                  <line x1="4.37114e-08" y1="0.5" x2="623" y2="0.500054"/>
                </svg>
                <svg data-aos="zoom-in" data-aos-delay="200" class="section__line-dot" width="3" height="3"
                     viewBox="0 0 3 3" fill="none" xmlns="http://www.w3.org/2000/svg">
                  <circle cx="1.5" cy="1.5" r="1.5"/>
                </svg>
                <svg data-aos="zoom-in" class="section__line-middle" width="30" height="30" viewBox="0 0 30 30"
                     fill="none" xmlns="http://www.w3.org/2000/svg">
                  <circle cx="15" cy="15" r="14.3" stroke-width="1.4"/>
                  <circle cx="15" cy="15" r="1.3" stroke-width="1.4"/>
                  <path
                    d="M15.0239 6H14.9789C14.9754 6.04957 14.955 6.09633 14.9227 6.13359C14.222 7.34437 13.5206 8.56008 12.8175 9.77156C11.4236 9.39504 10.0307 9.01359 8.63672 8.63672C9.01289 10.0303 9.39609 11.4225 9.77051 12.8168C8.51578 13.548 7.25684 14.2716 6 14.9993V15C7.25648 15.7288 8.51613 16.4523 9.77121 17.1829C9.39504 18.5768 9.01359 19.9693 8.63672 21.3629C10.0307 20.9868 11.4232 20.605 12.8168 20.2288C13.5473 21.4839 14.2716 22.7432 14.9996 24H15C15.7288 22.7439 16.4516 21.4839 17.1836 20.2295C18.5775 20.6043 19.9697 20.9868 21.3633 21.3633C20.9864 19.9693 20.6053 18.5768 20.2284 17.1825C21.4846 16.4534 22.7432 15.7281 24 15C22.7439 14.2712 21.4842 13.548 20.2295 12.8168C20.6043 11.4225 20.9871 10.0307 21.3633 8.63672C19.9693 9.01289 18.5771 9.39609 17.1829 9.77051C16.4776 8.56008 15.7805 7.34473 15.0766 6.13324C15.0573 6.09105 15.012 6.04992 15.0239 6ZM15.2341 10.8702C16.1479 10.9198 17.038 11.2889 17.7229 11.8943C18.491 12.5651 19.0015 13.5266 19.1101 14.5416C19.1973 15.3108 19.0658 16.1046 18.7287 16.8018C18.3479 17.5998 17.6993 18.266 16.9136 18.671C16.1791 19.0553 15.327 19.2061 14.5046 19.107C13.6163 19.0064 12.7641 18.6049 12.1246 17.9798C11.4932 17.3755 11.0674 16.5641 10.9226 15.7028C10.7855 14.8949 10.8878 14.0466 11.2239 13.2984C11.568 12.5275 12.1569 11.87 12.8832 11.4408C13.5874 11.0224 14.4171 10.8231 15.2341 10.8702Z"/>
                </svg>
                <svg data-aos="zoom-in" data-aos-delay="200" class="section__line-dot" width="3" height="3"
                     viewBox="0 0 3 3" fill="none" xmlns="http://www.w3.org/2000/svg">
                  <circle cx="1.5" cy="1.5" r="1.5"/>
                </svg>
                <svg data-aos="zoom-right" data-aos-delay="400" class="section__line-line" width="623" height="1"
                     viewBox="0 0 623 1" fill="none" xmlns="http://www.w3.org/2000/svg">
                  <line x1="4.37114e-08" y1="0.5" x2="623" y2="0.500054"/>
                </svg>
                <svg data-aos="zoom-in" data-aos-delay="600" class="section__line-dot" width="3" height="3"
                     viewBox="0 0 3 3" fill="none" xmlns="http://www.w3.org/2000/svg">
                  <circle cx="1.5" cy="1.5" r="1.5"/>
                </svg>
              </div>
              <h2 class="section__title" data-aos="fade-up">
                Neueste bewertungen
              </h2>
            </div>
            <div class="reviews-section__slider">
              <carouselxx :slideValue="slideControllerForBewertungen" :nav="false" :lazyLoad="true" :loop="true"
                          :rewind="false" :items="4"
                          :autoWidth="false" :margin="20" :dots="false"
                          :responsive="{0:{items:1},350:{items:1},600:{items:1},1024:{items:3},1280:{items:4}}"
                          :class="['carousel__service']">
                <div class="reviews-section__slider-item" v-for="review in reviews" :key="review.id">
                  <div class="review-card">
                    <div class="review-card__header">
                      <div class="review-card__client">
                        alexandria Über
                      </div>
                      <a href="" class="review-card__expert">
                        <div class="review-card__expert-ava">
                          <img :src="require(`@/assets/img/${review.avatar}`)" alt="">
                        </div>
                        <div class="review-card__expert-name">
                          {{ review.author }}
                        </div>
                      </a>
                    </div>
                    <div class="review-card__body">
                      <div class="review-card__rates js-rating" data-rateyo-read-only="true" data-rating="5"></div>
                      <div class="review-card__text">
                        {{ review.text }}
                      </div>
                      <ul class="review-card__tags tags">
                        <li class="tags__item" v-for="(ite,ind) in review.numbers" :key="ind">
                          <a href="" class="tags__link">
											<span>
												{{ ite }}
											</span>
                          </a>
                        </li>
                        <!--                        <li class="tags__item">-->
                        <!--                          <a href="" class="tags__link">-->
                        <!--											<span>-->
                        <!--												#Numerologie-->
                        <!--											</span>-->
                        <!--                          </a>-->
                        <!--                        </li>-->
                        <!--                        <li class="tags__item">-->
                        <!--                          <a href="" class="tags__link">-->
                        <!--											<span>-->
                        <!--												#Hellsehen-->
                        <!--											</span>-->
                        <!--                          </a>-->
                        <!--                        </li>-->
                        <!--                        <li class="tags__item">-->
                        <!--                          <a href="" class="tags__link">-->
                        <!--											<span>-->
                        <!--												#Numerologie-->
                        <!--											</span>-->
                        <!--                          </a>-->
                        <!--                        </li>-->
                      </ul>
                      <div class="review-card__date">
                        {{ review.data }}
                      </div>
                    </div>
                  </div>
                </div>
              </carouselxx>
              <!--              <div class="reviews-section__slider-item">-->
              <!--                <div class="review-card">-->
              <!--                  <div class="review-card__header">-->
              <!--                    <div class="review-card__client">-->
              <!--                      alexandria Über-->
              <!--                    </div>-->
              <!--                    <a href="" class="review-card__expert">-->
              <!--                      <div class="review-card__expert-ava">-->
              <!--                        <img src="img/ava.png" alt="">-->
              <!--                      </div>-->
              <!--                      <div class="review-card__expert-name">-->
              <!--                        Catherine-->
              <!--                      </div>-->
              <!--                    </a>-->
              <!--                  </div>-->
              <!--                  <div class="review-card__body">-->
              <!--                    <div class="review-card__rates js-rating" data-rateyo-read-only="true" data-rating="5"></div>-->
              <!--                    <div class="review-card__text">-->
              <!--                      Bin sowas von happy. Das 2.-->
              <!--                    </div>-->
              <!--                    <ul class="review-card__tags tags">-->
              <!--                      <li class="tags__item">-->
              <!--                        <a href="" class="tags__link">-->
              <!--											<span>-->
              <!--												#Astrologie-->
              <!--											</span>-->
              <!--                        </a>-->
              <!--                      </li>-->
              <!--                      <li class="tags__item">-->
              <!--                        <a href="" class="tags__link">-->
              <!--											<span>-->
              <!--												#Numerologie-->
              <!--											</span>-->
              <!--                        </a>-->
              <!--                      </li>-->
              <!--                      <li class="tags__item">-->
              <!--                        <a href="" class="tags__link">-->
              <!--											<span>-->
              <!--												#Hellsehen-->
              <!--											</span>-->
              <!--                        </a>-->
              <!--                      </li>-->
              <!--                      <li class="tags__item">-->
              <!--                        <a href="" class="tags__link">-->
              <!--											<span>-->
              <!--												#Numerologie-->
              <!--											</span>-->
              <!--                        </a>-->
              <!--                      </li>-->
              <!--                    </ul>-->
              <!--                    <div class="review-card__date">-->
              <!--                      12. Mai 2021 um 11:25 Uhr-->
              <!--                    </div>-->
              <!--                  </div>-->
              <!--                </div>-->
              <!--              </div>-->
              <!--              <div class="reviews-section__slider-item">-->
              <!--                <div class="review-card">-->
              <!--                  <div class="review-card__header">-->
              <!--                    <div class="review-card__client">-->
              <!--                      alexandria Über-->
              <!--                    </div>-->
              <!--                    <a href="" class="review-card__expert">-->
              <!--                      <div class="review-card__expert-ava">-->
              <!--                        <img src="img/ava.png" alt="">-->
              <!--                      </div>-->
              <!--                      <div class="review-card__expert-name">-->
              <!--                        Catherine-->
              <!--                      </div>-->
              <!--                    </a>-->
              <!--                  </div>-->
              <!--                  <div class="review-card__body">-->
              <!--                    <div class="review-card__rates js-rating" data-rateyo-read-only="true" data-rating="5"></div>-->
              <!--                    <div class="review-card__text">-->
              <!--                      Bin sowas von happy. Das 2. Treffen war gestern. Du sagtest er ist wie ein Geschenk für mich. Heut kann ich es bestätigen. BINGO. Du sagtest, nach dem 2ten Treffen wirst du nicht mehr nach dem Mann aus der Vergangenheit fragen. Danke lieber Alessandro, kann nur sagen, empfehlenswert. Bin sowas von happy. Das 2. Treffen...-->
              <!--                    </div>-->
              <!--                    <ul class="review-card__tags tags">-->
              <!--                      <li class="tags__item">-->
              <!--                        <a href="" class="tags__link">-->
              <!--											<span>-->
              <!--												#Astrologie-->
              <!--											</span>-->
              <!--                        </a>-->
              <!--                      </li>-->
              <!--                      <li class="tags__item">-->
              <!--                        <a href="" class="tags__link">-->
              <!--											<span>-->
              <!--												#Numerologie-->
              <!--											</span>-->
              <!--                        </a>-->
              <!--                      </li>-->
              <!--                      <li class="tags__item">-->
              <!--                        <a href="" class="tags__link">-->
              <!--											<span>-->
              <!--												#Hellsehen-->
              <!--											</span>-->
              <!--                        </a>-->
              <!--                      </li>-->
              <!--                      <li class="tags__item">-->
              <!--                        <a href="" class="tags__link">-->
              <!--											<span>-->
              <!--												#Numerologie-->
              <!--											</span>-->
              <!--                        </a>-->
              <!--                      </li>-->
              <!--                    </ul>-->
              <!--                    <div class="review-card__date">-->
              <!--                      12. Mai 2021 um 11:25 Uhr-->
              <!--                    </div>-->
              <!--                  </div>-->
              <!--                </div>-->
              <!--              </div>-->
              <!--              <div class="reviews-section__slider-item">-->
              <!--                <div class="review-card">-->
              <!--                  <div class="review-card__header">-->
              <!--                    <div class="review-card__client">-->
              <!--                      alexandria Über-->
              <!--                    </div>-->
              <!--                    <a href="" class="review-card__expert">-->
              <!--                      <div class="review-card__expert-ava">-->
              <!--                        <img src="img/ava.png" alt="">-->
              <!--                      </div>-->
              <!--                      <div class="review-card__expert-name">-->
              <!--                        Catherine-->
              <!--                      </div>-->
              <!--                    </a>-->
              <!--                  </div>-->
              <!--                  <div class="review-card__body">-->
              <!--                    <div class="review-card__rates js-rating" data-rateyo-read-only="true" data-rating="5"></div>-->
              <!--                    <div class="review-card__text">-->
              <!--                      Bin sowas von happy. Das 2. Treffen war gestern. Du sagtest er ist wie ein Geschenk für mich. Heut kann ich es bestätigen. BINGO. Du sagtest, nach dem 2ten Treffen wirst du nicht mehr nach dem Mann aus der Vergangenheit fragen. Danke lieber Alessandro, kann nur sagen, empfehlenswert. Bin sowas von happy. Das 2. Treffen...-->
              <!--                    </div>-->
              <!--                    <ul class="review-card__tags tags">-->
              <!--                      <li class="tags__item">-->
              <!--                        <a href="" class="tags__link">-->
              <!--											<span>-->
              <!--												#Astrologie-->
              <!--											</span>-->
              <!--                        </a>-->
              <!--                      </li>-->
              <!--                      <li class="tags__item">-->
              <!--                        <a href="" class="tags__link">-->
              <!--											<span>-->
              <!--												#Numerologie-->
              <!--											</span>-->
              <!--                        </a>-->
              <!--                      </li>-->
              <!--                      <li class="tags__item">-->
              <!--                        <a href="" class="tags__link">-->
              <!--											<span>-->
              <!--												#Hellsehen-->
              <!--											</span>-->
              <!--                        </a>-->
              <!--                      </li>-->
              <!--                      <li class="tags__item">-->
              <!--                        <a href="" class="tags__link">-->
              <!--											<span>-->
              <!--												#Numerologie-->
              <!--											</span>-->
              <!--                        </a>-->
              <!--                      </li>-->
              <!--                    </ul>-->
              <!--                    <div class="review-card__date">-->
              <!--                      12. Mai 2021 um 11:25 Uhr-->
              <!--                    </div>-->
              <!--                  </div>-->
              <!--                </div>-->
              <!--              </div>-->
              <!--              <div class="reviews-section__slider-item">-->
              <!--                <div class="review-card">-->
              <!--                  <div class="review-card__header">-->
              <!--                    <div class="review-card__client">-->
              <!--                      alexandria Über-->
              <!--                    </div>-->
              <!--                    <a href="" class="review-card__expert">-->
              <!--                      <div class="review-card__expert-ava">-->
              <!--                        <img src="img/ava.png" alt="">-->
              <!--                      </div>-->
              <!--                      <div class="review-card__expert-name">-->
              <!--                        Catherine-->
              <!--                      </div>-->
              <!--                    </a>-->
              <!--                  </div>-->
              <!--                  <div class="review-card__body">-->
              <!--                    <div class="review-card__rates js-rating" data-rateyo-read-only="true" data-rating="5"></div>-->
              <!--                    <div class="review-card__text">-->
              <!--                      Bin sowas von happy. Das 2. Treffen war gestern. Du sagtest er ist wie ein Geschenk für mich. Heut kann ich es bestätigen. BINGO. Du sagtest, nach dem 2ten Treffen wirst du nicht mehr nach dem Mann aus der Vergangenheit fragen. Danke lieber Alessandro, kann nur sagen, empfehlenswert. Bin sowas von happy. Das 2. Treffen...-->
              <!--                    </div>-->
              <!--                    <ul class="review-card__tags tags">-->
              <!--                      <li class="tags__item">-->
              <!--                        <a href="" class="tags__link">-->
              <!--											<span>-->
              <!--												#Astrologie-->
              <!--											</span>-->
              <!--                        </a>-->
              <!--                      </li>-->
              <!--                      <li class="tags__item">-->
              <!--                        <a href="" class="tags__link">-->
              <!--											<span>-->
              <!--												#Numerologie-->
              <!--											</span>-->
              <!--                        </a>-->
              <!--                      </li>-->
              <!--                      <li class="tags__item">-->
              <!--                        <a href="" class="tags__link">-->
              <!--											<span>-->
              <!--												#Hellsehen-->
              <!--											</span>-->
              <!--                        </a>-->
              <!--                      </li>-->
              <!--                      <li class="tags__item">-->
              <!--                        <a href="" class="tags__link">-->
              <!--											<span>-->
              <!--												#Numerologie-->
              <!--											</span>-->
              <!--                        </a>-->
              <!--                      </li>-->
              <!--                    </ul>-->
              <!--                    <div class="review-card__date">-->
              <!--                      12. Mai 2021 um 11:25 Uhr-->
              <!--                    </div>-->
              <!--                  </div>-->
              <!--                </div>-->
              <!--              </div>-->
            </div>
            <div class="reviews-section__footer">
              <button class="reviews-section__arr-prev slider-arr" @click="slideControllerForBewertungen--">
                <svg width="12" height="12" viewBox="0 0 12 12" fill="none" xmlns="http://www.w3.org/2000/svg">
                  <path d="M4.74524 1.68164L0.818687 6.20272L4.74524 10.318M0.816406 6.16289H11.18H0.816406Z"
                        stroke-width="1.6" stroke-linecap="round" stroke-linejoin="round"/>
                </svg>
              </button>
              <a href="" class="btn btn--main btn--static">
                <span>Zeige alles</span>
              </a>
              <button class="reviews-section__arr-next slider-arr" @click="slideControllerForBewertungen++">
                <svg width="12" height="12" viewBox="0 0 12 12" fill="none" xmlns="http://www.w3.org/2000/svg">
                  <path d="M7.25476 1.68164L11.1813 6.20272L7.25476 10.318M11.1836 6.16289H0.819958H11.1836Z"
                        stroke-width="1.6" stroke-linecap="round" stroke-linejoin="round"/>
                </svg>
              </button>
            </div>
          </div>
        </div>
      </div>
    </section>
    <section class="text-section pt-lg pb-lg">
      <div class="container">
        <div class="row">
          <div class="col-12">
            <div class="section__header section__header--white">
              <div class="section__line section__line--light">
                <svg data-aos="zoom-in" data-aos-delay="600" class="section__line-dot" width="3" height="3"
                     viewBox="0 0 3 3" fill="none" xmlns="http://www.w3.org/2000/svg">
                  <circle cx="1.5" cy="1.5" r="1.5"/>
                </svg>
                <svg data-aos="zoom-left" data-aos-delay="400" class="section__line-line" width="623" height="1"
                     viewBox="0 0 623 1" fill="none" xmlns="http://www.w3.org/2000/svg">
                  <line x1="4.37114e-08" y1="0.5" x2="623" y2="0.500054"/>
                </svg>
                <svg data-aos="zoom-in" data-aos-delay="200" class="section__line-dot" width="3" height="3"
                     viewBox="0 0 3 3" fill="none" xmlns="http://www.w3.org/2000/svg">
                  <circle cx="1.5" cy="1.5" r="1.5"/>
                </svg>
                <svg data-aos="zoom-in" class="section__line-middle" width="30" height="30" viewBox="0 0 30 30"
                     fill="none" xmlns="http://www.w3.org/2000/svg">
                  <circle cx="15" cy="15" r="14.3" stroke="#D5D9E0" stroke-width="1.4"/>
                  <rect x="21.5" y="12.3789" width="3" height="3" transform="rotate(45 21.5 12.3789)" fill="#D5D9E0"/>
                  <path
                    d="M12.7746 7.75105C13.7767 7.24352 14.8952 6.9894 16.0099 7.00034C17.1553 7.01446 18.3013 7.31022 19.3085 7.87811V7.88623C18.9452 7.98187 18.6091 8.16646 18.2747 8.3394C17.1859 8.94717 16.2678 9.87506 15.6415 10.9805C15.0935 11.9394 14.7676 13.0343 14.7071 14.1478C14.6292 15.5334 14.9503 16.9427 15.6266 18.1413C16.412 19.5457 17.6846 20.6366 19.1449 21.2112C18.2564 21.6739 17.2736 21.9383 16.281 21.9905C14.9411 22.0636 13.5832 21.7371 12.4127 21.0559C11.5 20.5283 10.6962 19.797 10.0815 18.9196C9.21543 17.6917 8.73001 16.185 8.69531 14.6652V14.3006C8.73443 12.7921 9.22223 11.2999 10.0839 10.0836C10.7771 9.09188 11.7089 8.27976 12.7746 7.75105Z"
                    fill="#D5D9E0"/>
                </svg>
                <svg data-aos="zoom-in" data-aos-delay="200" class="section__line-dot" width="3" height="3"
                     viewBox="0 0 3 3" fill="none" xmlns="http://www.w3.org/2000/svg">
                  <circle cx="1.5" cy="1.5" r="1.5"/>
                </svg>
                <svg data-aos="zoom-right" data-aos-delay="400" class="section__line-line" width="623" height="1"
                     viewBox="0 0 623 1" fill="none" xmlns="http://www.w3.org/2000/svg">
                  <line x1="4.37114e-08" y1="0.5" x2="623" y2="0.500054"/>
                </svg>
                <svg data-aos="zoom-in" data-aos-delay="600" class="section__line-dot" width="3" height="3"
                     viewBox="0 0 3 3" fill="none" xmlns="http://www.w3.org/2000/svg">
                  <circle cx="1.5" cy="1.5" r="1.5"/>
                </svg>
              </div>
              <h2 class="section__title" data-aos="fade-up">
                Über den Service
              </h2>
              <p class="section__text" data-aos="fade-up" data-aos-delay="200">
                Es ist ein lang erwiesener Fakt, dass ein Leser vom Text abgelenkt wird, wenn er sich ein Layout
                ansieht. Der Punkt, Lorem Ipsum zu nutzen, ist, dass es mehr oder weniger die normale Anordnung von
                Buchstaben darstellt und somit nach lesbarer Sprache aussieht. Viele Desktop Publisher und Webeditoren
                nutzen mittlerweile Lorem Ipsum als den Standardtext, auch die Suche im Internet nach "lorem ipsum"
                macht viele Webseiten sichtbar, wo diese noch immer vorkommen. Mittlerweile gibt es mehrere Versionen
                des Lorem Ipsum, einige zufällig, andere bewusst
              </p>
            </div>
            <div class="text-section__main-block">
              <img src="../assets/img/grey-divider.svg" data-aos="fade-up" alt="" class="text-section__main-block-icon">
              <h3 class="text-section__main-block-title" data-aos="fade-up" data-aos-delay="200">
                So nutzen Sie den Dienst <br>
                in 3 Minuten 45 Sekunden
              </h3>
              <div data-aos="zoom-in" data-aos-delay="400" class="text-section__main-block-video">
                <img src="../assets/img/yb-img.jpg" alt="">
                <a href="" class="text-section__main-block-play-btn">
                  <svg width="23" height="26" viewBox="0 0 23 26" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <path
                      d="M21.6758 12.1342C22.3424 12.5191 22.3424 13.4814 21.6758 13.8663L2.08755 25.1755C1.42088 25.5604 0.587545 25.0793 0.587545 24.3095V1.69096C0.587545 0.921157 1.42088 0.440031 2.08755 0.824932L21.6758 12.1342Z"/>
                  </svg>
                </a>
              </div>
            </div>
            <div class="text-section__blocks">
              <div class="row">
                <div class="col-lg-6">
                  <div class="text-section__block">
                    <img src="../assets/img/icon-1.svg" data-aos="fade-right" alt="">
                    <h3 data-aos="fade-right" data-aos-delay="200">Kunde werden</h3>
                    <p data-aos="fade-right" data-aos-delay="400">
                      Es ist ein lang erwiesener Fakt, dass ein Leser vom Text abgelenkt wird, wenn er sich ein Layout
                      ansieht. Der Punkt, Lorem Ipsum zu nutzen, ist, dass es mehr oder weniger die normale Anordnung
                      von Buchstaben darstellt und somit nach lesbarer Sprache aussieht. Viele Desktop Publisher und
                      Webeditoren nutzen mittlerweile
                    </p>
                  </div>
                </div>
                <div class="col-lg-6">
                  <div class="text-section__block">
                    <img src="../assets/img/icon-2.svg" data-aos="fade-left" alt="">
                    <h3 data-aos="fade-left" data-aos-delay="200">Berater werden</h3>
                    <p data-aos="fade-left" data-aos-delay="400">
                      Es ist ein lang erwiesener Fakt, dass ein Leser vom Text abgelenkt wird, wenn er sich ein Layout
                      ansieht. Der Punkt, Lorem Ipsum zu nutzen, ist, dass es mehr oder weniger die normale Anordnung
                      von Buchstaben darstellt und somit nach lesbarer Sprache aussieht. Viele Desktop Publisher und
                      Webeditoren nutzen mittlerweile
                    </p>
                  </div>
                </div>
                <div class="col-lg-8 offset-lg-2">
                  <div class="text-section__block">
                    <img src="../assets/img/icon-3.svg" data-aos="fade-up" alt="">
                    <h3 data-aos="fade-up" data-aos-delay="200">Über die Zahlung für Dienstleistungen</h3>
                    <p data-aos="fade-up" data-aos-delay="400">
                      Es ist ein lang erwiesener Fakt, dass ein Leser vom Text abgelenkt wird, wenn er sich ein Layout
                      ansieht. Der Punkt, Lorem Ipsum zu nutzen, ist, dass es mehr oder weniger die normale Anordnung
                      von Buchstaben darstellt und somit nach lesbarer Sprache aussieht. Viele Desktop Publisher und
                      Webeditoren nutzen mittlerweile
                    </p>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
    <section class="section faq-section pt-lg pb-lg">
      <div class="container">
        <img src="../assets/img/faq=section-img.png" alt="" class="faq-section__img">
        <div class="row">
          <div class="col-12">
            <div class="section__header">
              <div class="section__line">
                <svg data-aos="zoom-in" data-aos-delay="600" class="section__line-dot" width="3" height="3"
                     viewBox="0 0 3 3" fill="none" xmlns="http://www.w3.org/2000/svg">
                  <circle cx="1.5" cy="1.5" r="1.5"/>
                </svg>
                <svg data-aos="zoom-left" data-aos-delay="400" class="section__line-line" width="623" height="1"
                     viewBox="0 0 623 1" fill="none" xmlns="http://www.w3.org/2000/svg">
                  <line x1="4.37114e-08" y1="0.5" x2="623" y2="0.500054"/>
                </svg>
                <svg data-aos="zoom-in" data-aos-delay="200" class="section__line-dot" width="3" height="3"
                     viewBox="0 0 3 3" fill="none" xmlns="http://www.w3.org/2000/svg">
                  <circle cx="1.5" cy="1.5" r="1.5"/>
                </svg>
                <svg data-aos="zoom-in" class="section__line-middle" width="30" height="30" viewBox="0 0 30 30"
                     fill="none" xmlns="http://www.w3.org/2000/svg">
                  <circle cx="15" cy="15" r="14.3" stroke-width="1.4"/>
                  <circle cx="15" cy="15" r="1.3" stroke-width="1.4"/>
                  <path
                    d="M15.0239 6H14.9789C14.9754 6.04957 14.955 6.09633 14.9227 6.13359C14.222 7.34437 13.5206 8.56008 12.8175 9.77156C11.4236 9.39504 10.0307 9.01359 8.63672 8.63672C9.01289 10.0303 9.39609 11.4225 9.77051 12.8168C8.51578 13.548 7.25684 14.2716 6 14.9993V15C7.25648 15.7288 8.51613 16.4523 9.77121 17.1829C9.39504 18.5768 9.01359 19.9693 8.63672 21.3629C10.0307 20.9868 11.4232 20.605 12.8168 20.2288C13.5473 21.4839 14.2716 22.7432 14.9996 24H15C15.7288 22.7439 16.4516 21.4839 17.1836 20.2295C18.5775 20.6043 19.9697 20.9868 21.3633 21.3633C20.9864 19.9693 20.6053 18.5768 20.2284 17.1825C21.4846 16.4534 22.7432 15.7281 24 15C22.7439 14.2712 21.4842 13.548 20.2295 12.8168C20.6043 11.4225 20.9871 10.0307 21.3633 8.63672C19.9693 9.01289 18.5771 9.39609 17.1829 9.77051C16.4776 8.56008 15.7805 7.34473 15.0766 6.13324C15.0573 6.09105 15.012 6.04992 15.0239 6ZM15.2341 10.8702C16.1479 10.9198 17.038 11.2889 17.7229 11.8943C18.491 12.5651 19.0015 13.5266 19.1101 14.5416C19.1973 15.3108 19.0658 16.1046 18.7287 16.8018C18.3479 17.5998 17.6993 18.266 16.9136 18.671C16.1791 19.0553 15.327 19.2061 14.5046 19.107C13.6163 19.0064 12.7641 18.6049 12.1246 17.9798C11.4932 17.3755 11.0674 16.5641 10.9226 15.7028C10.7855 14.8949 10.8878 14.0466 11.2239 13.2984C11.568 12.5275 12.1569 11.87 12.8832 11.4408C13.5874 11.0224 14.4171 10.8231 15.2341 10.8702Z"/>
                </svg>
                <svg data-aos="zoom-in" data-aos-delay="200" class="section__line-dot" width="3" height="3"
                     viewBox="0 0 3 3" fill="none" xmlns="http://www.w3.org/2000/svg">
                  <circle cx="1.5" cy="1.5" r="1.5"/>
                </svg>
                <svg data-aos="zoom-right" data-aos-delay="400" class="section__line-line" width="623" height="1"
                     viewBox="0 0 623 1" fill="none" xmlns="http://www.w3.org/2000/svg">
                  <line x1="4.37114e-08" y1="0.5" x2="623" y2="0.500054"/>
                </svg>
                <svg data-aos="zoom-in" data-aos-delay="600" class="section__line-dot" width="3" height="3"
                     viewBox="0 0 3 3" fill="none" xmlns="http://www.w3.org/2000/svg">
                  <circle cx="1.5" cy="1.5" r="1.5"/>
                </svg>
              </div>
              <h2 data-aos="fade-up" class="section__title">Häufig gestellte fragen</h2>
            </div>
            <div class="row">
              <div class="col-lg-8 offset-lg-2">
                <div class="accardion-items">
                  <div class="accardion">
                    <div class="accardion__item" v-for="faq in faqs" :key="faq.id" @click="clickActiveFaq(faq.id)"
                         :class="{active:faq.openTab}">
                      <div class="accardion__item-header">
                        <div class="accardion__item-title">
                          {{ faq.title }}
                        </div>
                        <svg class="accardion__item-arr" width="13" height="8" viewBox="0 0 13 8" fill="none"
                             xmlns="http://www.w3.org/2000/svg">
                          <path d="M1 1L6.75614 7L12 1" stroke-width="1.5" stroke-linecap="round"
                                stroke-linejoin="round"/>
                        </svg>
                      </div>
                      <div class="accardion__item-body" data-aos="fade-up" data-aos-delay="600">
                        <p>
                          {{ faq.text }}
                        </p>
                      </div>
                    </div>
                    <!--                    <div class="accardion__item">-->
                    <!--                      <div class="accardion__item-header">-->
                    <!--                        <div class="accardion__item-title">-->
                    <!--                          Wie lade ich ein Konto für den Dienst auf?-->
                    <!--                        </div>-->
                    <!--                        <svg class="accardion__item-arr" width="13" height="8" viewBox="0 0 13 8" fill="none" xmlns="http://www.w3.org/2000/svg">-->
                    <!--                          <path d="M1 1L6.75614 7L12 1" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>-->
                    <!--                        </svg>-->
                    <!--                      </div>-->
                    <!--                      <div class="accardion__item-body">-->
                    <!--                        <p>-->
                    <!--                          Es ist ein lang erwiesener Fakt, dass ein Leser vom Text abgelenkt wird, wenn er sich ein Layout ansieht. Der Punkt, Lorem Ipsum zu nutzen, ist, dass es mehr oder weniger die normale Anordnung von Buchstaben darstellt und somit nach lesbarer Sprache aussieht. Viele Desktop Publisher und Webeditoren nutzen mittlerweile Lorem Ipsum als den Standardtext, auch die Suche im Internet nach "lorem ipsum" macht viele Webseiten sichtbar, wo diese noch immer vorkommen. Mittlerweile gibt es mehrere Versionen des Lorem Ipsum, einige zufällig, andere bewusst-->
                    <!--                        </p>-->
                    <!--                      </div>-->
                    <!--                    </div>-->
                    <!--                    <div class="accardion__item">-->
                    <!--                      <div class="accardion__item-header">-->
                    <!--                        <div class="accardion__item-title">-->
                    <!--                          Hier ist der Titel der Frage. Beim Klicken wird es entfaltet und die Antwort erscheint-->
                    <!--                        </div>-->
                    <!--                        <svg class="accardion__item-arr" width="13" height="8" viewBox="0 0 13 8" fill="none" xmlns="http://www.w3.org/2000/svg">-->
                    <!--                          <path d="M1 1L6.75614 7L12 1" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>-->
                    <!--                        </svg>-->
                    <!--                      </div>-->
                    <!--                      <div class="accardion__item-body">-->
                    <!--                        <p>-->
                    <!--                          Es ist ein lang erwiesener Fakt, dass ein Leser vom Text abgelenkt wird, wenn er sich ein Layout ansieht. Der Punkt, Lorem Ipsum zu nutzen, ist, dass es mehr oder weniger die normale Anordnung von Buchstaben darstellt und somit nach lesbarer Sprache aussieht. Viele Desktop Publisher und Webeditoren nutzen mittlerweile Lorem Ipsum als den Standardtext, auch die Suche im Internet nach "lorem ipsum" macht viele Webseiten sichtbar, wo diese noch immer vorkommen. Mittlerweile gibt es mehrere Versionen des Lorem Ipsum, einige zufällig, andere bewusst-->
                    <!--                        </p>-->
                    <!--                      </div>-->
                    <!--                    </div>-->
                    <!--                    <div class="accardion__item">-->
                    <!--                      <div class="accardion__item-header">-->
                    <!--                        <div class="accardion__item-title">-->
                    <!--                          Wie überlasse ich eine Bewertung einem Spezialisten?-->
                    <!--                        </div>-->
                    <!--                        <svg class="accardion__item-arr" width="13" height="8" viewBox="0 0 13 8" fill="none" xmlns="http://www.w3.org/2000/svg">-->
                    <!--                          <path d="M1 1L6.75614 7L12 1" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>-->
                    <!--                        </svg>-->
                    <!--                      </div>-->
                    <!--                      <div class="accardion__item-body">-->
                    <!--                        <p>-->
                    <!--                          Es ist ein lang erwiesener Fakt, dass ein Leser vom Text abgelenkt wird, wenn er sich ein Layout ansieht. Der Punkt, Lorem Ipsum zu nutzen, ist, dass es mehr oder weniger die normale Anordnung von Buchstaben darstellt und somit nach lesbarer Sprache aussieht. Viele Desktop Publisher und Webeditoren nutzen mittlerweile Lorem Ipsum als den Standardtext, auch die Suche im Internet nach "lorem ipsum" macht viele Webseiten sichtbar, wo diese noch immer vorkommen. Mittlerweile gibt es mehrere Versionen des Lorem Ipsum, einige zufällig, andere bewusst-->
                    <!--                        </p>-->
                    <!--                      </div>-->
                    <!--                    </div>-->
                    <!--                    <div class="accardion__item">-->
                    <!--                      <div class="accardion__item-header">-->
                    <!--                        <div class="accardion__item-title">-->
                    <!--                          Hier ist der Titel der Frage. Beim Klicken wird es entfaltet und die Antwort erscheint-->
                    <!--                        </div>-->
                    <!--                        <svg class="accardion__item-arr" width="13" height="8" viewBox="0 0 13 8" fill="none" xmlns="http://www.w3.org/2000/svg">-->
                    <!--                          <path d="M1 1L6.75614 7L12 1" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>-->
                    <!--                        </svg>-->
                    <!--                      </div>-->
                    <!--                      <div class="accardion__item-body">-->
                    <!--                        <p>-->
                    <!--                          Es ist ein lang erwiesener Fakt, dass ein Leser vom Text abgelenkt wird, wenn er sich ein Layout ansieht. Der Punkt, Lorem Ipsum zu nutzen, ist, dass es mehr oder weniger die normale Anordnung von Buchstaben darstellt und somit nach lesbarer Sprache aussieht. Viele Desktop Publisher und Webeditoren nutzen mittlerweile Lorem Ipsum als den Standardtext, auch die Suche im Internet nach "lorem ipsum" macht viele Webseiten sichtbar, wo diese noch immer vorkommen. Mittlerweile gibt es mehrere Versionen des Lorem Ipsum, einige zufällig, andere bewusst-->
                    <!--                        </p>-->
                    <!--                      </div>-->
                    <!--                    </div>-->
                    <!--                    <div class="accardion__item">-->
                    <!--                      <div class="accardion__item-header">-->
                    <!--                        <div class="accardion__item-title">-->
                    <!--                          Wie lade ich ein Konto für den Dienst auf?-->
                    <!--                        </div>-->
                    <!--                        <svg class="accardion__item-arr" width="13" height="8" viewBox="0 0 13 8" fill="none" xmlns="http://www.w3.org/2000/svg">-->
                    <!--                          <path d="M1 1L6.75614 7L12 1" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>-->
                    <!--                        </svg>-->
                    <!--                      </div>-->
                    <!--                      <div class="accardion__item-body">-->
                    <!--                        <p>-->
                    <!--                          Es ist ein lang erwiesener Fakt, dass ein Leser vom Text abgelenkt wird, wenn er sich ein Layout ansieht. Der Punkt, Lorem Ipsum zu nutzen, ist, dass es mehr oder weniger die normale Anordnung von Buchstaben darstellt und somit nach lesbarer Sprache aussieht. Viele Desktop Publisher und Webeditoren nutzen mittlerweile Lorem Ipsum als den Standardtext, auch die Suche im Internet nach "lorem ipsum" macht viele Webseiten sichtbar, wo diese noch immer vorkommen. Mittlerweile gibt es mehrere Versionen des Lorem Ipsum, einige zufällig, andere bewusst-->
                    <!--                        </p>-->
                    <!--                      </div>-->
                    <!--                    </div>-->
                    <!--                    <div class="accardion__item">-->
                    <!--                      <div class="accardion__item-header">-->
                    <!--                        <div class="accardion__item-title">-->
                    <!--                          Wie überlasse ich eine Bewertung einem Spezialisten?-->
                    <!--                        </div>-->
                    <!--                        <svg class="accardion__item-arr" width="13" height="8" viewBox="0 0 13 8" fill="none" xmlns="http://www.w3.org/2000/svg">-->
                    <!--                          <path d="M1 1L6.75614 7L12 1" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>-->
                    <!--                        </svg>-->
                    <!--                      </div>-->
                    <!--                      <div class="accardion__item-body">-->
                    <!--                        <p>-->
                    <!--                          Es ist ein lang erwiesener Fakt, dass ein Leser vom Text abgelenkt wird, wenn er sich ein Layout ansieht. Der Punkt, Lorem Ipsum zu nutzen, ist, dass es mehr oder weniger die normale Anordnung von Buchstaben darstellt und somit nach lesbarer Sprache aussieht. Viele Desktop Publisher und Webeditoren nutzen mittlerweile Lorem Ipsum als den Standardtext, auch die Suche im Internet nach "lorem ipsum" macht viele Webseiten sichtbar, wo diese noch immer vorkommen. Mittlerweile gibt es mehrere Versionen des Lorem Ipsum, einige zufällig, andere bewusst-->
                    <!--                        </p>-->
                    <!--                      </div>-->
                    <!--                    </div>-->
                  </div>
                </div>
                <a href="" class="btn btn--main btn--static">
							<span>
								Zeige alles
							</span>
                </a>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
    <main-footer></main-footer>
  </div>
</template>
<script>
import MainHeader from './Block/MainHeader'
import MainFooter from './Block/MainFooter'
import carousel from 'vue-owl-carousel'
import carouselxx from 'xx-vue-owl-carousel'
export default {
  components: {
    MainHeader,
    MainFooter,
    carousel,
    carouselxx
  },
  data() {
    return {
      slideControllerForBewertungen: 0,
      slideController: 0,
      slider: [
        {id: 1, title: "Hast du ein problem? Wir werden Ihnen helfen", button: "Starten"},
        {id: 2, title: "Hast du ein problem? Wir werden Ihnen helfen", button: "Starten"},
        {id: 3, title: "Hast du ein problem? Wir werden Ihnen helfen", button: "Starten"},
      ],
      users: [
        {
          id: 1,
          big_avatar: 'big-ava.jpg',
          location: 'Deutschland, Berlin',
          term: 'Berufserfahrung 5 jahre',
          status: 'Neuling',
          review: '226',
          text: 'Hellsehen-fühlen ganz OHNE',
          tags: ['#Astrologie', '#Numerologie', '#Hellsehen'],
          price_bell: '1',
          bell: 'Kostenlos anrufen',
          price: '0'
        },
        {
          id: 2,
          big_avatar: 'big-ava.jpg',
          location: 'Deutschland, Berlin',
          term: 'Berufserfahrung 5 jahre',
          status: 'Neuling',
          review: '226',
          text: 'Hellsehen-fühlen ganz OHNE',
          tags: ['#Astrologie', '#Numerologie', '#Hellsehen'],
          price_bell: '1',
          bell: 'Kostenlos anrufen',
          price: '0'
        },
        {
          id: 3,
          big_avatar: 'big-ava.jpg',
          location: 'Ukraine, Berlin',
          term: 'Berufserfahrung 5 jahre',
          status: 'Neuling',
          review: '226',
          text: 'Hellsehen-fühlen ganz OHNE',
          tags: ['#Astrologie', '#Numerologie', '#Hellsehen'],
          price_bell: '1',
          bell: 'Kostenlos anrufen',
          price: '0'
        },
        {
          id: 4,
          big_avatar: 'big-ava.jpg',
          location: 'Deutschland, Lvov',
          term: 'Berufserfahrung 5 jahre',
          status: 'Neuling',
          review: '226',
          text: 'Hellsehen-fühlen ganz OHNE',
          tags: ['#Astrologie', '#Numerologie', '#Hellsehen'],
          price_bell: '1',
          bell: 'Kostenlos anrufen',
          price: '0'
        },
        {
          id: 5,
          big_avatar: 'big-ava.jpg',
          location: 'Deutschland, Berlin',
          term: 'Berufserfahrung 5 jahre',
          status: 'Neuling',
          review: '226',
          text: 'Hellsehen-fühlen ganz OHNE',
          tags: ['#Astrologie', '#Numerologie', '#Hellsehen'],
          price_bell: '1',
          bell: 'Kostenlos anrufen',
          price: '0'
        },
        {
          id: 6,
          big_avatar: 'big-ava.jpg',
          location: 'Deutschland, Berlin',
          term: 'Berufserfahrung 5 jahre',
          status: 'Neuling',
          review: '226',
          text: 'Hellsehen-fühlen ganz OHNE',
          tags: ['#Astrologie', '#Numerologie', '#Hellsehen'],
          price_bell: '1',
          bell: 'Kostenlos anrufen',
          price: '0'
        },
        {
          id: 7,
          big_avatar: 'big-ava.jpg',
          location: 'Deutschland, Berlin',
          term: 'Berufserfahrung 5 jahre',
          status: 'Neuling',
          review: '226',
          text: 'Hellsehen-fühlen ganz OHNE',
          tags: ['#Astrologie', '#Numerologie', '#Hellsehen'],
          price_bell: '1',
          bell: 'Kostenlos anrufen',
          price: '0'
        }
      ],
      services: [
        {
          id: 1,
          avatar: 'ava.png',
          service_card: 'service-card-img.jpg',
          author: "Catherine",
          reviews: '26',
          title: 'Astrologische Vorhersage von Liebe und Familienleben für ein Jahr',
          text: 'Aus der astrologischen Vorhersage erfahren Sie, welche Ereignisse in Ihrem persönlichen Leben Sie im Laufe des Jahres erwarten.',
          price: '222'
        },
        {
          id: 2,
          avatar: 'ava.png',
          service_card: 'service-card-img.jpg',
          author: "Catherine",
          reviews: '226',
          title: 'Astrologische Vorhersage von Liebe und Familienleben für ein Jahr',
          text: 'Aus der astrologischen Vorhersage erfahren Sie, welche Ereignisse in Ihrem persönlichen Leben Sie im Laufe des Jahres erwarten.',
          price: '44'
        },
        {
          id: 3,
          avatar: 'ava.png',
          service_card: 'service-card-img.jpg',
          author: "Catherine",
          reviews: '445',
          title: 'Astrologische Vorhersage von Liebe und Familienleben für ein Jahr',
          text: 'Aus der astrologischen Vorhersage erfahren Sie, welche Ereignisse in Ihrem persönlichen Leben Sie im Laufe des Jahres erwarten.',
          price: '0'
        },
        {
          id: 4,
          avatar: 'ava.png',
          service_card: 'service-card-img.jpg',
          author: "Catherine",
          reviews: '111',
          title: 'Astrologische Vorhersage von Liebe und Familienleben für ein Jahr',
          text: 'Aus der astrologischen Vorhersage erfahren Sie, welche Ereignisse in Ihrem persönlichen Leben Sie im Laufe des Jahres erwarten.',
          price: '0'
        },
        {
          id: 5,
          avatar: 'ava.png',
          service_card: 'service-card-img.jpg',
          author: "Catherine",
          reviews: '23',
          title: 'Astrologische Vorhersage von Liebe und Familienleben für ein Jahr',
          text: 'Aus der astrologischen Vorhersage erfahren Sie, welche Ereignisse in Ihrem persönlichen Leben Sie im Laufe des Jahres erwarten.',
          price: '0'
        },
        {
          id: 6,
          avatar: 'ava.png',
          service_card: 'service-card-img.jpg',
          author: "Catherine",
          reviews: '226',
          title: 'Astrologische Vorhersage von Liebe und Familienleben für ein Jahr',
          text: 'Aus der astrologischen Vorhersage erfahren Sie, welche Ereignisse in Ihrem persönlichen Leben Sie im Laufe des Jahres erwarten.',
          price: '0'
        },
      ],
      reviews: [
        {
          id: 1,
          author: 'Catherine',
          avatar: 'ava.png',
          text: 'Bin sowas von happy. Das 2. Treffen war gestern. Du sagtest er ist wie ein Geschenk für mich. Heut kann ich es bestätigen. BINGO. Du sagtest, nach dem 2ten Treffen wirst du nicht mehr nach dem Mann aus der Vergangenheit fragen. Danke lieber Alessandro, kann nur sagen, empfehlenswert. Bin sowas von happy. Das 2. Treffen...',
          numbers: ['#Astrologie', '#Numerologie', '#Numerologie', '#Hellsehen'],
          data: '12. Mai 2021 um 11:25 Uhr'
        },
        {
          id: 2,
          author: 'Catherine',
          avatar: 'ava.png',
          text: 'Bin sowas von happy. Das 2. Treffen war gestern. Du sagtest er ist wie ein Geschenk für mich. Heut kann ich es bestätigen. BINGO. Du sagtest, nach dem 2ten Treffen wirst du nicht mehr nach dem Mann aus der Vergangenheit fragen. Danke lieber Alessandro, kann nur sagen, empfehlenswert. Bin sowas von happy. Das 2. Treffen...',
          numbers: ['#Astrologie', '#Numerologie', '#Numerologie', '#Hellsehen'],
          data: '12. Mai 2021 um 11:25 Uhr'
        },
        {
          id: 3,
          author: 'Catherine',
          avatar: 'ava.png',
          text: 'Bin sowas von happy. Das 2. Treffen war gestern. Du sagtest er ist wie ein Geschenk für mich. Heut kann ich es bestätigen. BINGO. Du sagtest, nach dem 2ten Treffen wirst du nicht mehr nach dem Mann aus der Vergangenheit fragen. Danke lieber Alessandro, kann nur sagen, empfehlenswert. Bin sowas von happy. Das 2. Treffen...',
          numbers: ['#Astrologie', '#Numerologie', '#Numerologie', '#Hellsehen'],
          data: '12. Mai 2021 um 11:25 Uhr'
        },
        {
          id: 4,
          author: 'Catherine',
          avatar: 'ava.png',
          text: 'Bin sowas von happy. Das 2. Treffen war gestern. Du sagtest er ist wie ein Geschenk für mich. Heut kann ich es bestätigen. BINGO. Du sagtest, nach dem 2ten Treffen wirst du nicht mehr nach dem Mann aus der Vergangenheit fragen. Danke lieber Alessandro, kann nur sagen, empfehlenswert. Bin sowas von happy. Das 2. Treffen...',
          numbers: ['#Astrologie', '#Numerologie', '#Numerologie', '#Hellsehen'],
          data: '12. Mai 2021 um 11:25 Uhr'
        },
        {
          id: 5,
          author: 'Catherine',
          avatar: 'ava.png',
          text: 'Bin sowas von happy. Das 2. Treffen war gestern. Du sagtest er ist wie ein Geschenk für mich. Heut kann ich es bestätigen. BINGO. Du sagtest, nach dem 2ten Treffen wirst du nicht mehr nach dem Mann aus der Vergangenheit fragen. Danke lieber Alessandro, kann nur sagen, empfehlenswert. Bin sowas von happy. Das 2. Treffen...',
          numbers: ['#Astrologie', '#Numerologie', '#Numerologie', '#Hellsehen'],
          data: '12. Mai 2021 um 11:25 Uhr'
        },
      ],
      faqs: [
        {
          id: 1,
          openTab: false,
          title: 'Hier ist der Titel der Frage. Beim Klicken wird es entfaltet und die Antwort erscheint ',
          text: 'Es ist ein lang erwiesener Fakt, dass ein Leser vom Text abgelenkt wird, wenn er sich ein Layout ansieht. Der Punkt, Lorem Ipsum zu nutzen, ist, dass es mehr oder weniger die normale Anordnung von Buchstaben darstellt und somit nach lesbarer Sprache aussieht. Viele Desktop Publisher und Webeditoren nutzen mittlerweile Lorem Ipsum als den Standardtext, auch die Suche im Internet nach "lorem ipsum" macht viele Webseiten sichtbar, wo diese noch immer vorkommen. Mittlerweile gibt es mehrere Versionen des Lorem Ipsum, einige zufällig, andere bewusst '
        },
        {
          id: 2,
          openTab: false,
          title: 'Wie lade ich ein Konto für den Dienst auf?',
          text: 'Es ist ein lang erwiesener Fakt, dass ein Leser vom Text abgelenkt wird, wenn er sich ein Layout ansieht. Der Punkt, Lorem Ipsum zu nutzen, ist, dass es mehr oder weniger die normale Anordnung von Buchstaben darstellt und somit nach lesbarer Sprache aussieht. Viele Desktop Publisher und Webeditoren nutzen mittlerweile Lorem Ipsum als den Standardtext, auch die Suche im Internet nach "lorem ipsum" macht viele Webseiten sichtbar, wo diese noch immer vorkommen. Mittlerweile gibt es mehrere Versionen des Lorem Ipsum, einige zufällig, andere bewusst '
        },
        {
          id: 3,
          openTab: false,
          title: 'Hier ist der Titel der Frage. Beim Klicken wird es entfaltet und die Antwort erscheint',
          text: 'Es ist ein lang erwiesener Fakt, dass ein Leser vom Text abgelenkt wird, wenn er sich ein Layout ansieht. Der Punkt, Lorem Ipsum zu nutzen, ist, dass es mehr oder weniger die normale Anordnung von Buchstaben darstellt und somit nach lesbarer Sprache aussieht. Viele Desktop Publisher und Webeditoren nutzen mittlerweile Lorem Ipsum als den Standardtext, auch die Suche im Internet nach "lorem ipsum" macht viele Webseiten sichtbar, wo diese noch immer vorkommen. Mittlerweile gibt es mehrere Versionen des Lorem Ipsum, einige zufällig, andere bewusst '
        },
        {
          id: 4,
          openTab: false,
          title: 'Wie überlasse ich eine Bewertung einem Spezialisten? ',
          text: 'Es ist ein lang erwiesener Fakt, dass ein Leser vom Text abgelenkt wird, wenn er sich ein Layout ansieht. Der Punkt, Lorem Ipsum zu nutzen, ist, dass es mehr oder weniger die normale Anordnung von Buchstaben darstellt und somit nach lesbarer Sprache aussieht. Viele Desktop Publisher und Webeditoren nutzen mittlerweile Lorem Ipsum als den Standardtext, auch die Suche im Internet nach "lorem ipsum" macht viele Webseiten sichtbar, wo diese noch immer vorkommen. Mittlerweile gibt es mehrere Versionen des Lorem Ipsum, einige zufällig, andere bewusst '
        },
        {
          id: 5,
          openTab: false,
          title: 'Hier ist der Titel der Frage. Beim Klicken wird es entfaltet und die Antwort erscheint ',
          text: 'Es ist ein lang erwiesener Fakt, dass ein Leser vom Text abgelenkt wird, wenn er sich ein Layout ansieht. Der Punkt, Lorem Ipsum zu nutzen, ist, dass es mehr oder weniger die normale Anordnung von Buchstaben darstellt und somit nach lesbarer Sprache aussieht. Viele Desktop Publisher und Webeditoren nutzen mittlerweile Lorem Ipsum als den Standardtext, auch die Suche im Internet nach "lorem ipsum" macht viele Webseiten sichtbar, wo diese noch immer vorkommen. Mittlerweile gibt es mehrere Versionen des Lorem Ipsum, einige zufällig, andere bewusst '
        },
        {
          id: 6,
          openTab: false,
          title: 'Wie lade ich ein Konto für den Dienst auf? ',
          text: 'Es ist ein lang erwiesener Fakt, dass ein Leser vom Text abgelenkt wird, wenn er sich ein Layout ansieht. Der Punkt, Lorem Ipsum zu nutzen, ist, dass es mehr oder weniger die normale Anordnung von Buchstaben darstellt und somit nach lesbarer Sprache aussieht. Viele Desktop Publisher und Webeditoren nutzen mittlerweile Lorem Ipsum als den Standardtext, auch die Suche im Internet nach "lorem ipsum" macht viele Webseiten sichtbar, wo diese noch immer vorkommen. Mittlerweile gibt es mehrere Versionen des Lorem Ipsum, einige zufällig, andere bewusst '
        },
      ],
    }
  },
  name: 'Home',
  computed: {},
  methods: {
    clickActiveFaq(ids) {
      this.faqs.map(p => {
        if (ids == p.id) {
          p.openTab = !p.openTab
        } else if (ids !== p.id) {
          p.openTab = false
        }
      })
    },
  },
}
</script>




