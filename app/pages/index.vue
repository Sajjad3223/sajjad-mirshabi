<template>
  <div class="w-full flex flex-col relative">
    <header class="container py-5 flex items-center justify-between" dir="rtl">
      <div class="flex items-center gap-2">
        <img src="/logo.png" alt="logo" class="max-w-4">
        <div class="flex flex-col -space-y-1">
          <strong class="leading-[14px] flex items-center gap-1">
            <b>سجاد</b>
            <b>میرشبی</b>
          </strong>
          <span class="text-xs opacity-50 font-bold -z-[1] font-montserrat uppercase">Developer</span>
        </div>
      </div>
      <div class="flex items-center gap-4 text-sm">
        <a href="" class="opacity-70 hover:opacity-100 transition-opacity duration-200">مهارت ها</a>
        <a href="" class="opacity-70 hover:opacity-100 transition-opacity duration-200">پروژه ها</a>
        <a href="" class="opacity-70 hover:opacity-100 transition-opacity duration-200">تماس با من</a>
      </div>
    </header>
    <div class="container mx-auto flex items-center justify-center " dir="rtl">
      <div class="flex-1 flex flex-col gap-5">
        <div class="flex flex-col items-start gap-5">
          <div class="flex flex-col items-start">
            <div class="grid place-items-center relative">
              <SplitText
                  dir="ltr"
                  text="Sajjad Mirshabi"
                  class-name="text-5xl font-black text-center p-2 uppercase font-montserrat"
                  :delay="100"
                  :duration="0.6"
                  ease="power3.out"
                  split-type="chars"
                  :from="{ opacity: 0, y: 40 }"
                  :to="{ opacity: 1, y: 0 }"
                  :threshold="0.1"
                  root-margin="-100px"
                  text-align="center"
                  @animation-complete="handleAnimationComplete"
              />
              <!--            <ShinyText
                              text="برنامه نویس و طراح سایت"
                              :disabled="false"
                              :speed="3"
                              class-name="text-2xl font-black absolute"
                          />-->
            </div>
            <TextType dir="rtl"
                      :text="['برنامه نویس  Net.', 'برنامه نویس و طراح سایت', 'مدرس و فعال حوزه بازی سازی']"
                      :typingSpeed="75"
                      :pauseDuration="1500"
                      :showCursor="true"
                      cursorCharacter="|"
                      class-name="text-4xl font-bold opacity-60"
            />
          </div>
          <p class="w-2/3 opacity-60 line-clamp-3">
            لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت چاپ، و با استفاده از طراحان گرافیک است، چاپگرها و متون بلکه روزنامه و مجله در ستون و سطرآنچنان که لازم است، و برای شرایط فعلی تکنولوژی مورد نیاز، و کاربردهای متنوع با هدف بهبود ابزارهای کاربردی می باشد، کتابهای زیادی در شصت و سه درصد گذشته حال و آینده، شناخت فراوان جامعه و متخصصان را می طلبد، تا با نرم افزارها شناخت بیشتری را برای طراحان رایانه ای علی الخصوص طراحان خلاقی، و فرهنگ پیشرو در زبان فارسی ایجاد کرد، در این صورت می توان امید داشت که تمام و دشواری موجود در ارائه راهکارها، و شرایط سخت تایپ به پایان رسد و زمان مورد نیاز شامل حروفچینی دستاوردهای اصلی، و جوابگوی سوالات پیوسته اهل دنیای موجود طراحی اساسا مورد استفاده قرار گیرد.
          </p>
          <div class="flex items-center gap-4">
            <button class="bg-white text-black rounded-full px-6 py-2.5">تماس با من</button>
            <button class="bg-white/20 rounded-full px-6 py-2.5">پروژه ها</button>
          </div>
          <hr class="w-full opacity-20">
          <div class="w-full flex flex-col gap-2">
            <div class="flex items-center gap-2">
              <span class="opacity-60 w-1/3">تلفن تماس:</span>
              <span class="text-xl font-bold">09154222478</span>
            </div>
            <div class="w-full flex items-center gap-2">
              <span class="opacity-60 w-1/3">ایمیل:</span>
              <span class="text-xl font-montserrat" dir="ltr">m.sajjad1378@gmail.com</span>
            </div>
            <div class="w-full flex items-center gap-2">
              <span class="opacity-60 w-1/3">آیدی تلگرام:</span>
              <span class="text-xl font-montserrat" dir="ltr">@Sajjad3223</span>
            </div>
          </div>
        </div>
      </div>
      <div class="relative h-[500px] aspect-square grid place-items-center">
        <Orb :hoverIntensity="0.1" :rotateOnHover="true" :hue="0" :forceHoverState="false" class="scale-110"/>
        <img src="/avatar.jpg" alt="avatar" class="w-[400px] rounded-full aspect-square object-cover absolute -z-[1]">

        <div class="w-20 aspect-square grid font-bold place-items-center hover:-rotate-12 transition-all duration-300 rounded-2xl bg-white/20 backdrop-blur-lg border-2 border-white/30 absolute left-0 top-0 font-montserrat translate-full" dir="ltr">
          .NET
        </div>
        <div class="w-20 aspect-square grid font-bold place-items-center hover:-rotate-12 transition-all duration-300 rounded-2xl bg-white/20 backdrop-blur-lg border-2 border-white/30 absolute right-0 top-0 font-montserrat -translate-x-full translate-y-full" dir="ltr">
          Nuxt
        </div>
        <div class="w-20 aspect-square grid font-bold place-items-center hover:-rotate-12 transition-all duration-300 rounded-2xl bg-white/20 backdrop-blur-lg border-2 border-white/30 absolute left-0 bottom-0 font-montserrat -translate-y-full translate-x-full" dir="ltr">
          SQL
        </div>
        <div class="w-20 aspect-square grid font-bold place-items-center hover:-rotate-12 transition-all duration-300 rounded-2xl bg-white/20 backdrop-blur-lg border-2 border-white/30 absolute right-0 bottom-0 font-montserrat -translate-full" dir="ltr">
          UE5
        </div>
      </div>
    </div>
    <hr class="my-20 container opacity-20">
    <div class="container mx-auto flex items-center justify-center " dir="rtl">

    </div>

  </div>
</template>

<script setup lang="ts">

const handleAnimationComplete = () => {
  console.log('All letters have animated!');
};
</script>