<template>
  <header class="header">
    <div class="container">
      <div class="header__inner">
        <div class="header__inner-item header__inner-item-top">
          <div class="header__location">
            <p class="header__location-title">Работаем в РБ с 2007 г.</p>
          </div>
          <nav class="nav">
            <ul class="sub-menu">
              <li
                class="sub-menu__item"
                v-for="(element, i) of subMenu"
                :key="i"
                :href="element.path"
              >
                <a class="sub-menu__link" href="#">{{ element.name }}</a>
              </li>
            </ul>
          </nav>
          <div class="header__contact">
            <div class="header__contact-time">
              <p class="header__contact-title">контакт-центр</p>
              <p class="header__contact-title">с 8:00 до 19:00</p>
            </div>
            <div class="header__contact-menu">
              <a class="header__contact-menu-link" href="#" target="_blank">
                <svg
                  width="32"
                  height="33"
                  viewBox="0 0 32 33"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <ellipse
                    cx="15.5623"
                    cy="16.0112"
                    rx="15.5623"
                    ry="16.0112"
                    fill="#0088CC"
                  />
                  <path
                    d="M21.1625 11.7702L19.0612 21.7818C18.9027 22.4883 18.4893 22.6642 17.9018 22.3313L14.7002 19.9478L13.1554 21.4489C12.9844 21.6216 12.8414 21.7661 12.512 21.7661L12.742 18.4718L18.6758 13.0546C18.9338 12.8222 18.6199 12.6935 18.2748 12.9258L10.9391 17.5925L7.78105 16.5938C7.0941 16.3771 7.08167 15.8998 7.92403 15.5669L20.2766 10.759C20.8485 10.5423 21.349 10.8877 21.1625 11.7702Z"
                    fill="white"
                  />
                </svg>
              </a>
              <a class="sub-menu__link menu__link-contact" href="#">
                КОНТАКТЫ
              </a>
            </div>

            <address class="header__modal">
              <div class="header__modal-left">
                <ul class="header__modal-left-list">
                  <li class="header__modal-left-item">
                    <span class="header__modal-title"
                      >Самара, ул. Садовая, 199</span
                    >
                    <span class="header__modal-left-subtitle"
                      >(вывеска "Мир кирпича")</span
                    >
                    <a class="header__modal-left-link" href="#"
                      >схема проезда</a
                    >
                  </li>
                  <li class="header__modal-left-item">
                    <p class="header__modal-left-text">
                      Наш центральный офис с выставочным залом
                    </p>
                  </li>
                  <li class="header__modal-left-item">
                    <a class="header__modal-phone" href="tel:+78462151515"
                      >+7 (846) 215-15-15</a
                    >
                    <span class="header__modal-left-caption"
                      >с 8:00 до 19:00 по Самаре</span
                    >
                    <span class="header__modal-left-caption"
                      >менеджер Виктор</span
                    >
                  </li>
                  <li class="header__modal-left-item">
                    <ul class="header__modal-left-user-list">
                      <li class="header__modal-left-user-item">
                        <a
                          class="header__modal-left-user-link"
                          href="#"
                          target="_blank"
                        >
                          <img
                            class="header__modal-left-social-img"
                            src="../images/social/vaiber.svg"
                            alt="Viber"
                          />
                        </a>
                      </li>
                      <li class="header__modal-left-user-item">
                        <a
                          class="header__modal-left-user-link"
                          href="#"
                          target="_blank"
                        >
                          <img
                            class="header__modal-left-social-img"
                            src="../images/social/watsapp.svg"
                            alt="watsapp"
                          />
                        </a>
                      </li>
                      <li class="header__modal-left-user-item">
                        <a
                          class="header__modal-left-user-link"
                          href="#"
                          target="_blank"
                        >
                          <img
                            class="header__modal-left-social-img"
                            src="../images/social/telegram.svg"
                            alt="telegram"
                          />
                        </a>
                      </li>
                      <li class="header__modal-left-user-item">
                        <a
                          class="header__modal-left-user-link"
                          href="#"
                          target="_blank"
                        >
                          <img
                            class="header__modal-left-social-img"
                            src="../images/social/mail.svg"
                            alt="mail"
                          />
                        </a>
                      </li>
                    </ul>
                  </li>
                  <li class="header__modal-left-item">
                    <a
                      class="header__modal-left-email"
                      href="mailto:samara777@samara777.ru"
                      >samara777@samara777.ru</a
                    >
                  </li>
                  <li class="header__modal-left-item">
                    <p class="header__modal-left-descr">
                      Режим работы: Понедельник-Пятница с 8:00 до 17:00, суббота
                      и воскресенье - работаем по предварительной договоренности
                    </p>
                  </li>
                  <li class="header__modal-left-item header__modal-carousel">
                    <img
                      class="header__modal-carousel-img"
                      src="../images/carousel/min-modal-1.jpg"
                      alt="building's facade"
                    />
                  </li>
                </ul>
              </div>
              <div class="header__modal-right">
                <ul class="header__modal-right-list">
                  <li
                    class="header__modal-right-item header__modal-right-item-top"
                  >
                    <span class="header__modal-right-subtitle">
                      Бесплатный звонок с любого номера
                    </span>
                    <a class="header__modal-phone" href="tel:+78005155555">
                      +7 (800) 515-55-55
                    </a>
                    <span class="header__modal-right-subtitle-bottom">
                      с 8:00 до 19:00 по всей России
                    </span>
                  </li>
                  <li
                    class="header__modal-right-item header__modal-right-item-top"
                  >
                    <span class="header__modal-right-subtitle">
                      Мобильный телефон в Москве
                    </span>
                    <a class="header__modal-phone" href="tel:+78464150808">
                      +7 (846) 415-08-08
                    </a>
                    <span class="header__modal-right-subtitle-bottom">
                      с 8:00 до 19:00 по МСК
                    </span>
                  </li>
                  <li
                    class="header__modal-right-item header__modal-right-item-address"
                  >
                    <p class="header__modal-title">Адреса магазинов:</p>
                    <ul class="header__modal-right-address-list">
                      <li class="header__modal-right-address-item">
                        Самара, ул. Садовая, 199
                      </li>
                      <li class="header__modal-right-address-item">
                        Самара, Южное шоссе, 5К
                      </li>
                      <li class="header__modal-right-address-item">
                        Самара, ул. Алма-Атинская, 133
                      </li>
                      <li class="header__modal-right-address-item">
                        Самарская обл., с.Преображенка
                      </li>
                    </ul>
                  </li>
                  <li
                    class="header__modal-right-item header__modal-right-item-bottom"
                  >
                    <a class="header__modal-right-btn" href="#"
                      >Обратный звонок</a
                    >
                    <p class="header__modal-right-text">
                      Наши доброжелательные менеджеры всегда будут рады ответить
                      на Ваш звонок, письмо, или лично проконсультировать Вас в
                      офисах продаж.
                    </p>
                  </li>
                </ul>
              </div>
            </address>
          </div>
        </div>
        <div class="header__inner-item header__inner-item-center">
          <a class="header-logo" href="#">
            <img
              class="header-logo__img"
              src="../assets/images/logo.png"
              alt="Логотип компании"
            />
          </a>
          <form class="header-form" action="#">
            <input
              class="header-form__input"
              type="search"
              placeholder="Поиск по названию, бренду ..."
            />
            <button class="header-form__btn" type="submit"></button>
          </form>
          <div class="header__basket">
            <div class="header__basket-inner">
              <div class="header__basket-item">
                <span class="header__basket-text">Корзина:</span>
                <span class="header__basket-num">0</span>
                <span class="header__basket-rub">₽</span>
              </div>
              <a class="header__basket-item header__basket-icon" href="#">
                <span class="tip">0</span>
              </a>
            </div>
            <a class="header__basket-link" href="#">Как сделать заказ</a>
          </div>
        </div>
        <div class="header__inner-item header__inner-item-bottom">
          <div class="header__catalog-btn">Каталог продукции</div>
          <nav class="main-menu">
            <ul class="main-menu__list">
              <li
                class="main-menu__item"
                v-for="(element, i) of mainMenu"
                :key="i"
                :href="element.path"
              >
                <a class="main-menu__link" href="#">{{ element.name }}</a>
              </li>
            </ul>
          </nav>
        </div>
      </div>
    </div>
  </header>
</template>

<script setup>
import { ref } from "vue";

const mainMenu = [
  {
    name: "Лампы",
    path: "/svetodiodnye-lampy",
  },
  {
    name: "Светильники",
    path: "/svetodiodnye-svetilniki",
  },
  {
    name: "Панели",
    path: "/svetodiodnye-paneli",
  },
  {
    name: "Уличные светильники",
    path: "/ulichnye-svetilniki",
  },
  {
    name: "Прожекторы",
    path: "/svetodiodnye-prozhektory",
  },
  {
    name: "Трековые светильники",
    path: "/trekovye-svetilniki",
  },
];

const caltalog = [
  {
    name: "Светодиодные лампы",
    path: "/svetodiodnye-lampy",
  },
  {
    name: "Светодиодные светильники",
    path: "/svetodiodnye-svetilniki",
  },
  {
    name: "Светодиодные панели",
    path: "/svetodiodnye-paneli",
  },
  {
    name: "Уличные светильники",
    path: "/ulichnye-svetilniki",
  },
  {
    name: "Светодиодные прожекторы",
    path: "/svetodiodnye-prozhektory",
  },
  {
    name: "Трековые светильники",
    path: "/trekovye-svetilniki",
  },
  {
    name: "LED лента и комплектующие",
    path: "/led-lenta-komplektuyushchie",
  },
  {
    name: "Фонари",
    path: "/fonari",
  },
  {
    name: "Электроустановочные изделия",
    path: "/elektroustanovochnye-izdeliya",
  },
  {
    name: "ЭУИ",
    path: "/eui",
  },
  {
    name: "Электромонтажные изделия",
    path: "/elektromontazhnye-izdeliya",
  },
  {
    name: "Элементы питания и зарядные устройства",
    path: "/elementy-pitaniya-i-zaryadnye-ustrojstva",
  },
  {
    name: "Светильники на солнечных батареях",
    path: "/svetilniki-na-solnechnyh-batareyah",
  },
];

const subMenu = [
  {
    name: "ГЛАВНАЯ",
    path: "/",
  },
  {
    name: "О КОМПАНИИ",
    path: "/o-company",
  },
  {
    name: "ДОСТАВКА",
    path: "/dostavka",
  },
  {
    name: "ОТЗЫВЫ",
    path: "/otzivu",
  },
  {
    name: "Как сделать заказ",
    path: "/kak-sdelat-zakaz",
  },
];
</script>