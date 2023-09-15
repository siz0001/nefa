<template>
  <div class="w-full">
    <!-- Hero section -->
    <section class="w-full h-[70vh] sm:h-[170vh] lg:h-[70vh] flex items-center"><!-- pb-24  -->
      <BaseSection>
        <div class="col-span-12 lg:col-span-6 mt-12 xl:mt-10 space-y-4 sm:space-y-6 px-6 text-center sm:text-left" style="font-family:'Pretendard';">
          <span data-aos="fade-right" data-aos-once="true" class="text-base text-gradient uppercase" style="color:#2E8BAE; font-weight:700;"
            >유튜브 영상기반 최신 낚시정보</span
          >
          <h1
            data-aos="fade-right"
            data-aos-once="true"
            class="text-[2.1rem] sm:text-xl xl:text-3xl leading-tight capitalize sm:pr-8 xl:pr-10"
          >
            기존 낚시 어플들과<br>
            무슨 차이가 있냐구요?
          </h1>
          <h1
            data-aos="fade-down"
            data-aos-once="true"
            class="text-[2.5rem] sm:text-xl xl:text-3xl leading-tight capitalize sm:pr-8 xl:pr-10"
            style="color:#00B3EB; font-weight:900"
          >
            낚시인과 크리에이터의 만남<br>
            유튜브 영상기반 최신 낚시정보<br>
            <span style="color:#243E90">새로운 낚시어플 FISHING YOU</span>
          </h1>
          <div
            data-aos="fade-up"
            data-aos-once="true"
            data-aos-delay="700"
            class="flex flex-col sm:flex-row space-y-4 sm:space-y-0 sm:space-x-4 mt-2"
          >
          </div>
        </div>

        <div class="hidden sm:block col-span-12 lg:col-span-6">
          <div class="w-full">
            <img
              data-aos="fade-up"
              data-aos-once="true"
              :src="require('~/assets/img/fishingyou_main/main_one.png')"
              class="mt-4"
              alt=""
            />
          </div>
        </div>
      </BaseSection>
    </section>

    <section
      class="max-w-screen-xl mx-2 sm:mx-auto px-4 sm:px-6 lg:px-0 py-6 pb-20 sm:py-8 rounded-[2.25rem] sm:rounded-xl bg-white shadow-lg sm:shadow-md transform lg:-translate-y-12"
    >
      <div class="w-full flex flex-col lg:flex-row items-start justify-center">
        <LandingCryptoStatistic
          data-aos="fade-up"
          title="ℹ️ 정보 수집"
          :datasets="informationCollection"
          class="xl:border-r border-gray-200 lg:px-8"
        />
        <LandingCryptoStatistic
          data-aos="fade-up"
          data-aos-delay="150"
          title="🧳 준비"
          :datasets="preparation"
          class="xl:border-r border-gray-200 lg:px-8"
        />
        <LandingCryptoStatistic
          data-aos="fade-up"
          data-aos-delay="300"
          title="🚗 이동"
          :datasets="movement"
          class="lg:px-8"
        />
        <LandingCryptoStatistic
          data-aos="fade-up"
          data-aos-delay="300"
          title="🎣 낚시"
          :datasets="fishingRod"
          class="lg:px-8"
        />
      </div>
    </section>

    <section class="bg-trading-tools  relative max-w-full sm:mx-6 my-24 shadow sm:rounded-2xl overflow-hidden">
      <div class="w-full px-6 sm:px-0 py-32 flex flex-col items-center justify-center space-y-4 text-center">
        <div
            data-aos="flip-down"
            class="text-[2.5rem] sm:text-xl xl:text-3xl leading-tight capitalize sm:pr-8 xl:pr-10"
            style="color:#00B3EB; font-weight:900; font-size:38px;"
          >해결책은 FISHING YOU</div>
          <div
            data-aos="flip-down"
            class="text-[2.5rem] sm:text-xl xl:text-3xl leading-tight capitalize sm:pr-8 xl:pr-10"
            style="color:#243E90; font-weight:900; font-size:38px;"
          >새로운 낚시 어플 FISINGYOU</div>

      </div>
    </section>

    <!-- Buy and trade section -->
    <section class="w-full h-[100vh] sm:h-[200vh] lg:h-[100vh] my-24 flex items-center"><!--  my-24  -->
      <BaseSection>
        <LandingBuyTradeImage class="sm:hidden mb-8" />

        <LandingBuyTradeImage data-aos="fade-left" class="hidden sm:block" />
        <div class="col-span-12 lg:col-span-6 mt-24 xl:mt-22  space-y-4 sm:space-y-6 px-6 text-right sm:text-right" style="font-family: 'Pretendard';">

          <h1
            data-aos="fade-left"
            data-aos-once="true"
            class="text-[2.1rem] sm:text-xl xl:text-3xl leading-tight capitalize sm:pr-8 xl:pr-10"
          >
            이곳에서 낚시 포인트가<br>
            어디에 있을지 궁금하다면?
          </h1>
          <h1
            data-aos="fade-down"
            data-aos-once="true"
            class="text-[2.5rem] sm:text-xl xl:text-3xl leading-tight capitalize sm:pr-8 xl:pr-10"
            style="font-weight:900; color:#00B3EB"
          >
            위치기반 최신 낚시 정보는<br>
            <span style="color:#243E90">새로운 낚시어플 FISHING YOU</span>
          </h1>
          <div
            data-aos="fade-up"
            data-aos-once="true"
            data-aos-delay="700"
            class="flex flex-col space-y-4 sm:pr-8 xl:pr-10 mt-2"
          >
          <p>현재위치에서 다른 사람들은 어떻게 낚시 하는지<br>
          어떤 어종이 잡히는지, 어느 포인트가 있는지<br>
          어떤 유튜버가 다녀가서 낚시 했는지 궁금하시죠?<br>
          이제는 피싱유 어플로 확인해 보세요!</p>

          </div>
        </div>

      </BaseSection>
    </section>



    <!-- Credit card section -->
    <section class="w-full h-[100vh] sm:h-[200vh] lg:h-[100vh] my-36 flex items-center" style="background-color:#F5FFFF "><!-- my-36  -->
      <BaseSection data-aos="fade-down" class="items-center">

        <div class="col-span-12 lg:col-span-6 mt-24 xl:mt-22  space-y-4 sm:space-y-6 px-6 text-left sm:text-left" style="font-family: 'Pretendard'">
          <h1 data-aos="fade-left" data-aos-once="true" class="text-[2.1rem] sm:text-xl xl:text-3xl  leading-tight capitalize sm:pr-8 xl:pr-10">
            나도 유튜브 보니까<br>
            낚시가고 싶은데 저기 어디지?
          </h1>
          <h1 data-aos="fade-down" data-aos-once="true" class="text-[2.5rem] sm:text-xl xl:text-3xl leading-tight capitalize sm:pr-8 xl:pr-10 font-900" style="font-weight:900; color:#00B3EB">
            낚시인과 크리에이터의 만남<br>
            <span style="color:#243E90">새로운 낚시어플 FISHING YOU</span>
          </h1>
          <div data-aos="fade-up" data-aos-once="true" data-aos-delay="700" class="flex flex-col space-y-4 sm:pr-8 xl:pr-10 mt-2">
            <p>새로운 낚시 정보 뿐만 아니라 기존 어플에는 없는<br>
              낚시 크리에이터의 영상시청과 정보공유<br>
              이제는 낚시 크리에이터가 다녀갔던 곳을 손쉽게<br>
              따라서 가 볼 수가 있습니다. 피싱유와 함께 라면요.
            </p>
          </div>
        </div>
        <div class="sm:block col-span-12 lg:col-span-6">
          <div class="w-full">
            <!-- <img :src="require('~/assets/img/nefa-cc.webp')" class="w-[95%]" alt="" /> -->
            <img :src="require('~/assets/img/fishingyou_main/main_three.png')" alt="" />
          </div>
        </div>
      </BaseSection>
    </section>

    <!-- Advanced trading tools section -->
    <!-- <section class="bg-trading-tools relative max-w-full sm:mx-4 my-20 py-16 shadow rounded-2xl overflow-hidden"> -->
      <section class="w-full  h-[100vh] sm:h-[200vh] lg:h-[100vh] my-20 flex items-center">
      <div class="relative max-w-screen-xl px-4 sm:px-2 mx-auto grid grid-cols-12 gap-x-6">
        <LandingTradingToolImage class="sm:hidden" />

        <LandingTradingToolImage data-aos="fade-left" class="hidden sm:block" />
        <div class="col-span-12 lg:col-span-6 mt-24 xl:mt-22  space-y-4 sm:space-y-6 px-6 text-right sm:text-right" style="font-family:'Pretendard'">
          <h1 data-aos="fade-left" data-aos-once="true" class="text-[2.1rem] sm:text-xl xl:text-3xl leading-tight capitalize sm:pr-8 xl:pr-10">
            가까운 곳에 낚시 할만한 장소가<br>
            있을까 궁금할 때에는?
          </h1>
          <h1 data-aos="fade-down" data-aos-once="true" class="text-[2.5rem] sm:text-xl xl:text-3xl leading-tight capitalize sm:pr-8 xl:pr-10" style="font-weight:900; color:#00B3EB">
            위치기반 최신 낚시 정보는<br>
            <span style="color:#243E90">새로운 낚시어플 FISHING YOU</span>
          </h1>
          <div data-aos="fade-up" data-aos-once="true" data-aos-delay="700" class="flex flex-col space-y-4 sm:pr-8 xl:pr-10 mt-2">
            <p>먼곳이 아니더라도, 우리집 근처에서 혹은 근교에서<br>
              어떤 어종이 잡히는지, 어느 포인트가 있는지<br>
              다른사람들은 조과가 얼마나 있었는지 궁금하다면<br>
              이제는 피싱유 어플로 확인해 보세요!
            </p>
          </div>
        </div>
      </div>
    </section>

    <!-- Industry-leading security section -->
    <section class="w-full h-[100vh] sm:h-[200vh] lg:h-[100vh] my-24 flex items-center" style="background-color:#EDFFFD"><!-- my-24  -->
      <div class="relative max-w-screen-xl px-8 mx-auto grid grid-cols-12 gap-x-6">
        <div class="col-span-12 lg:col-span-6 mt-24 xl:mt-22  space-y-4 sm:space-y-6 px-6 text-left sm:text-left" style="font-family:'Pretendard'">
          <h1 data-aos="fade-left" data-aos-once="true" class="text-[2.1rem] sm:text-xl xl:text-3xl leading-tight capitalize sm:pr-8 xl:pr-10">
            만능 낚시 어플 피싱유<br>
            위치기반 낚시와 유튜브까지?
          </h1>
          <h1 data-aos="fade-down" data-aos-once="true" class="text-[2.5rem] sm:text-xl xl:text-3xl leading-tight capitalize sm:pr-8 xl:pr-10" style="font-weight:900; color:#00B3EB">
            낚시인과 크리에이터의 만남<br>
            <span style="color:#243E90">새로운 낚시어플 FISHING YOU</span>
          </h1>
          <div data-aos="fade-up" data-aos-once="true" data-aos-delay="700" class="flex flex-col space-y-4 sm:pr-8 xl:pr-10 mt-2">
            <p>기존 어플에 있던 낚시시정보와 더불어 내 위치기반 낚시까지?<br>
              낚시 크리에이터의 영상시청과 정보공유도 가능해요.<br>
              기본 낚시 정보제공에 이은 영상시청과 위치기반 근교 낚시정보까지<br>
              이제 낚시어플은 피싱유 하나로 완벽합니다.
            </p>
          </div>
        </div>
        <div data-aos="fade-right" class="col-span-12 lg:col-span-6">
          <div class="w-full">
            <img :src="require('~/assets/img/fishingyou_main/main_five.png')" class="w-full" alt="" />
            <!-- <img :src="require('~/assets/img/industry-leading-security.webp')" class="w-full" alt="" /> -->
          </div>
        </div>

      </div>
    </section>

    <section class="bg-color w-full h-[100vh] sm:h-[200vh] lg:h-[100vh] my-24 flex items-center">
      <div class="relative max-w-screen-xl px-8 mx-auto grid grid-cols-12 gap-x-6">
        <div data-aos="fade-right" class="col-span-12 lg:col-span-6">
            <video controls  class="video">
              <source src="">
            </video>
            <img class="fishing-rod" :src="require('~/assets/img/fishingyou_main/fishing_rod.png')"  alt="" />
            <!-- <img :src="require('~/assets/img/industry-leading-security.webp')" class="w-full" alt="" /> -->
        </div>

        <div class="col-span-12 lg:col-span-6 mt-24 xl:mt-22  space-y-4 sm:space-y-6 px-6 text-right sm:text-right" style="font-family:'Pretendard'">
          <h1 data-aos="fade-down" data-aos-once="true" class="text-[2.5rem] sm:text-xl xl:text-3xl leading-tight capitalize sm:pr-8 xl:pr-10 text-app-gradient" style="font-weight:900;">
            특별한 낚시어플 피싱유<br>

          <span class="text-youtube-gradient">이제 유튜브로 피싱유를 확인해 보세요</span>

          </h1>
          <div data-aos="fade-up" data-aos-once="true" data-aos-delay="700" class="flex flex-col space-y-4 sm:pr-8 xl:pr-10 mt-2">
            <p>낚시 조과, 계절별로 잘 잡히는 어종, 미끼, 채비<br>
            서해, 동해, 남해, 배낚시, 방파제 낚시, 낚시터<br>
            기본적인 낚시 정보를 알려주는 어플은 많았습니다.
            </p>
            <p>낚시인과 크리에이터의 만남, 피싱유 어플은<br>
            현재 위치에서 다른 사람들은 어떻게 낚시하는지<br>
            어떤 어종이 잡히는지, 어느 포인트가 있는지<br>
            어떤 유튜버가 낚시했는지를 알 수 있습니다.<br>
            이제는 피싱유 어플로 확인해 보세요!
            </p>
          </div>
        </div>
      </div>
    </section>

    <div class="w-full mb-10 flex justify-center">
      <a
        v-smooth-scroll
        data-aos="flip-up"
        data-aos-delay="150"
        href="#navbar"
        class="px-6 py-3 flex items-center space-x-2 bg-[#FAFAFA] hover:bg-gray-100 hover:shadow-md border border-[#DDDDDD] rounded-md text-gray-700"
      >
        <span>Back to top</span>
        <ArrowUpIcon :size="20" />
      </a>
    </div>
  </div>
</template>

<script>
import aosMixin from '@/mixins/aos'
export default {
  name: 'IndexPage',
  mixins: [aosMixin],
  data() {
    return {
      selected: 0,
      dropdownConcurency: false,
      dropdownCrypto: false,
      currencySelected: {
        img: 'country-icon/eng.png',
        name: 'USD',
      },
      currencies: [
        {
          img: 'country-icon/eng.png',
          name: 'USD',
        },
      ],
      cryptoSelected: {
        img: 'crypto-icon/bitcoin.png',
        name: 'BTC',
      },
      cryptocurrencies: [
        {
          img: 'crypto-icon/bitcoin.png',
          name: 'BTC',
        },
      ],
      informationCollection: [
        {
          id: 1,
          text: '인터넷 검색',
        },
        {
          id: 2,
          text: '지인 정보',
        },
        {
          id: 3,
          text: '단체 톡방',
        },
        {
          id: 4,
          text: '낚시 서적 등',
        },
        {
          id: 5,
          detail: '비용 1 ~ 5만',
        },

        {
          id: 6,
          detail: '시간 1 ~ 3일',
        },
      ],
      preparation: [
        {
          id: 1,
          text: '음식',
        },
        {
          id: 2,
          text: '장비',
        },
        {
          id: 3,
          text: '채비',
        },
        {
          id: 4,
          text: '미끼',
        },
        {
          id: 5,
          text: '기타',
        },
        {
          id: 6,
          detail: '비용 1 ~ 10만',
        },

        {
          id: 7,
          detail: '시간 1 ~ 2일',
        },
      ],
      movement: [
        {
          id: 1,
          text: '기름값',
        },
        {
          id: 2,
          text: '배값',
        },
        {
          id: 3,
          text: '톨게이트 비용',
        },
        {
          id: 4,
          text: '식사비',
        },
        {
          id: 5,
          text: '휴게소 이용비',
        },
        {
          id: 6,
          detail: '비용 5 ~ 20만',
        },

        {
          id: 7,
          detail: '시간 1 ~ 5시간',
        },
      ],
      fishingRod: [
        {
          id: 1,
          detail: '소요시간: 1시간 ~ 1일',
        },
      ],
      accordions: [
        {
          title: 'Why should I choose NEFA?',
          description:
            "We're industry pioneers, having been in the cryptocurrency industry since 2016. We've facilitated more than 21 billion USD worth of transactions on our exchange for customers in over 40 countries. Today, we're trusted by over 8 million customers around the world and have received praise for our easy-to-use app, secure wallet, and range of features.",
        },
        {
          title: 'How secure is NEFA?',
          description:
            "We're industry pioneers, having been in the cryptocurrency industry since 2016. We've facilitated more than 21 billion USD worth of transactions on our exchange for customers in over 40 countries. Today, we're trusted by over million customers around the world and have received praise for our easy-to-use app, secure wallet, and range of features.",
        },
        {
          title: 'Do I have to buy a whole Bitcoin?',
          description:
            "We're industry pioneers, having been in the cryptocurrency industry since 2016. We've facilitated more than 21 billion USD worth of transactions on our exchange for customers in over 40 countries. Today, we're trusted by over million customers around the world and have received praise for our easy-to-use app, secure wallet, and range of features.",
        },
        {
          title: 'How do I actually buy Bitcoin?',
          description:
            "We're industry pioneers, having been in the cryptocurrency industry since 2016. We've facilitated more than 21 billion USD worth of transactions on our exchange for customers in over 40 countries. Today, we're trusted by over million customers around the world and have received praise for our easy-to-use app, secure wallet, and range of features.",
        },
      ],
      steps: [
        {
          img: 'sign-up.png',
          title: 'Sign Up',
          description:
            'Sign up for your free NEFA Wallet on web, iOS or Android and follow our easy process to set up your profile',
        },
        {
          img: 'fund.png',
          title: 'Fund',
          description:
            'Choose your preferred payment method such as bank transfer or credit card to top up your NEFA Wallet',
        },
        {
          img: 'buy-crypto.png',
          title: 'Buy Crypto',
          description:
            'Buy Bitcoin or Ethereum, then securely store it in your Wallet or send it on easily to your friends anywhere',
        },
      ],
    }
  },
}
</script>
<style scoped>
.video {
  width: 500px;
  height: 400px;
}
.fishing-rod {
  position: absolute;
  z-index: -1;
  bottom: 0;
  right:-55%;
}
.text-header-gradient {
  background: rgb(57, 132, 244);
  background: linear-gradient(169.4deg, #3984f4 -6.01%, #0cd3ff 36.87%, #2f7cf0 78.04%, #0e65e8 103.77%);
  background-clip: text;
  -webkit-text-fill-color: transparent;
}
.bg-partner {
  background: url('../assets/img/partner/background.png');
  background-size: cover;
  background-position: center;

}
.bg-trading-tools {
  background: url('../assets/img/bg-trading-tools.webp');
  background-size: cover;
  background-position: center;
}
.max-h-0 {
  max-height: 0;
}
.bg-color {
  /* background: linear-gradient(180deg, #FFF 65%, #48C6E2 73%, #4AC5E2 77%, #89B4DB 83.5%,  #99AED9 100%) */
  background: linear-gradient(180deg, rgba(72, 198, 226, 0), rgba(74, 197, 226, 0.01), rgba(137, 180, 219, 0.34), rgba(153, 174, 217, 0.5))
}
.text-app-gradient {
  background: linear-gradient(0deg, rgba(167, 198, 226, 1), rgba(151, 194, 227, 1), rgba(112, 186, 228, 1), rgba(77, 181, 230, 1), rgba(43, 178, 231, 1), rgba(22, 177, 231, 1));
  background-clip: text;
  -webkit-background-clip: text;
  color: transparent;
}
.text-youtube-gradient {
  background: linear-gradient(0deg, rgba(23, 136, 202, 1) 50%, rgba(36, 64, 143, 1) 100%);
  background-clip: text;
  -webkit-background-clip: text;
  color: transparent;
}
</style>
