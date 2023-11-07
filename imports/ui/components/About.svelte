<section class="about">
  <div class="container">
    <div class="content">
      <img
        src="/images/svg/Abstract.svg"
        data-aos="zoom-in"
        data-aos-duration="2000"
        alt=""
      />
      <div class="text">
        <h1 class="about-title" data-aos="fade-up" data-aos-duration="1000">
          <span class="name">Артур Арутюнян</span>
        </h1>
        <p class="first" data-aos="fade-up" data-aos-duration="2000">
          Веб-разработчик
        </p>
        <p class="second" data-aos="fade-up" data-aos-duration="3000">
          со страстью к работе и творчеству
        </p>
      </div>
      <div class="scroll-downs" data-aos="fade-up" data-aos-duration="2000">
        <div class="mousey">
          <div class="scroller" />
        </div>
      </div>
    </div>
  </div>
</section>

<style>
  .about {
    background-color: var(--color-dark);
    padding: 50px 0;
    transition: all 0.3s ease;
  }

  .container {
    display: flex;
    justify-content: center;
    align-items: center;
  }

  .content {
    color: var(--color-light);
    position: relative;
  }

  .text {
    position: absolute;
    left: 15%;
    top: 30%;
    text-align: right;
    letter-spacing: -0.5px;
    font-weight: 700;
  }

  .about-title {
    color: var(--color-light);
    font-size: 54px;
    font-style: normal;
    line-height: 110%;
    margin-bottom: 10px;
  }
  .name {
    color: var(--color-beige);
  }

  .first {
    font-size: 40px;
    font-style: normal;
    line-height: 140%;
    margin-bottom: 20px;
  }

  .second {
    font-size: 18px;
    font-style: normal;
    font-weight: 500;
    line-height: 24px;
  }

  .scroll-downs {
    position: absolute;
    top: 0;
    right: 0;
    bottom: 0;
    left: 0;
    margin: 90% auto;
    width: 34px;
    height: 55px;
  }
  .mousey {
    width: 3px;
    padding: 10px 15px;
    height: 35px;
    border: 2px solid #fff;
    border-radius: 25px;
    opacity: 0.75;
    box-sizing: content-box;
  }
  .scroller {
    width: 3px;
    height: 10px;
    border-radius: 25%;
    background-color: #fff;
    animation-name: scroll;
    animation-duration: 2.2s;
    animation-timing-function: cubic-bezier(0.15, 0.41, 0.69, 0.94);
    animation-iteration-count: infinite;
  }
  @keyframes scroll {
    0% {
      opacity: 0;
    }
    10% {
      transform: translateY(0);
      opacity: 1;
    }
    100% {
      transform: translateY(15px);
      opacity: 0;
    }
  }
</style>
