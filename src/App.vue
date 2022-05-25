<template>
  <div
    class="flex h-[12.5vw] min-h-[40px] w-full min-w-[320px] items-center justify-center bg-[#F3F3F3] lg:hidden"
  >
    <div class="flex w-[68.1vw] min-w-[218px] justify-center lg:w-[27.77vw]">
      <img src="./assets/BestChoice.png" alt="" />
    </div>
  </div>
  <div
    class="flex h-[171.875vw] min-h-[550px] w-full min-w-[320px] flex-col items-center bg-[#EAD8CA] lg:h-[62.5vw] lg:flex-row lg:items-start lg:justify-center"
  >
    <div class="flex flex-col items-center lg:gap-y-5 lg:py-[85px]">
      <div class="hidden w-[27.77vw] justify-center lg:flex">
        <img src="./assets/BestChoice.png" alt="" />
      </div>
      <div
        class="mt-[5px] flex w-[78.125vw] min-w-[250px] justify-center lg:w-[41.66vw]"
      >
        <img src="./assets/title.PNG" alt="" />
      </div>
      <div>
        <p
          class="text-center font-sans text-[6.25vw] font-semibold text-[#402104] lg:hidden"
        >
          復興高中 X 實境解謎
        </p>
        <p
          class="hidden text-center font-sans font-semibold text-[#402104] lg:flex lg:text-[4.44vw]"
        >
          復興高中<br />
          X <br />
          實境解謎
        </p>
      </div>
    </div>

    <div class="flex w-full min-w-[320px] justify-center lg:w-[52.083vw]">
      <img src="./assets/school.PNG" alt="" />
    </div>
  </div>
  <div
    class="flex h-[140.625vw] min-h-[450px] w-full min-w-[320px] flex-col items-center bg-[#D9CFC5] lg:h-[41.66vw] lg:flex-row lg:justify-evenly"
  >
    <div class="flex w-full justify-center lg:w-[48.61vw]">
      <img src="./assets/ComingSoon.PNG" alt="" />
    </div>
    <div class="lg:flex lg:flex-col lg:justify-center">
      <div>
        <p
          class="text-center font-sans text-[4.6875vw] font-semibold text-[#402104] lg:text-[2.5vw]"
        >
          輸入電子郵件 獲取最新消息
        </p>
      </div>
      <div
        class="flex h-[25.625vw] min-h-[82px] w-[87.5vw] min-w-[280px] flex-row items-center justify-center lg:mx-auto lg:h-[11.18055vw] lg:w-[34.7vw]"
      >
        <form
          class="relative flex w-full rounded-full border-2 border-[#C6612B] align-middle"
          @submit.prevent="push"
        >
          <input
            class="peer h-[15.625vw] min-h-[50px] w-[80%] bg-inherit px-[9vw] placeholder-transparent outline-none lg:h-[5.31875vw] lg:px-[2vw] lg:text-[2.5vw]"
            type="email"
            placeholder="電子郵件地址"
            v-model="email"
          />
          <label
            class="absolute left-[9.375vw] -top-[2.5vw] justify-center bg-[#D9CFC5] font-sans text-[3vw] font-semibold text-[#3E3D3D] duration-150 peer-placeholder-shown:top-[4.6875vw] peer-placeholder-shown:text-[4.375vw] lg:left-[2.3vw] lg:-top-[1.3vw] lg:text-[1.66vw] lg:peer-placeholder-shown:top-[0.8vw] lg:peer-placeholder-shown:text-[2.5vw]"
          >
            電子郵件地址
          </label>
          <button
            @click="push()"
            class="absolute right-0 h-[15.625vw] min-h-[50px] w-[21.875vw] min-w-[70px] rounded-full bg-[#C6612B] lg:h-[5.31875vw] lg:w-[9.027777777vw]"
            type="submit"
          >
            <img
              class="mx-auto w-[10.9375vw] min-w-[35px] lg:w-[4.513888888vw]"
              src="./assets/arrow.png"
              alt=""
            />
          </button>
        </form>
      </div>
      <div class="hidden lg:flex lg:flex-col lg:items-center">
        <div class="lg:w-[10.625vw]">
          <img src="./assets/We_re.PNG" alt="" />
        </div>
        <div class="lg:w-[38.5vw]">
          <img src="./assets/ComingSoonEn.PNG" alt="" />
        </div>
      </div>
    </div>

    <div class="flex w-full justify-center lg:hidden">
      <img src="./assets/We'reComingSoon.PNG" alt="" />
    </div>
  </div>
  <footer
    class="flex h-[18.75vw] min-h-[60px] w-full min-w-[320px] items-end justify-center bg-[#A49375] text-center text-[4.0625vw] text-white lg:h-[10.416vw] lg:text-[2.22vw]"
  >
    <div class="flex flex-col lg:flex-row lg:gap-x-32">
      <a href="tel:+886-2-8914131#641" class="-mb-[4px]"
        >客服專線 (02)2891-4131 #641</a
      >
      <a href="mailto:fhsh-reality-puzzle@fhsh.tp.edu.tw" class=""
        >聯絡信箱 fhsh-reality-puzzle@fhsh.tp.edu.tw</a
      >
    </div>
  </footer>
  <div
    id="jump"
    class="fixed inset-0 hidden h-full w-full items-center justify-center bg-black/40"
  >
    <div
      class="flex h-[42.1875vw] min-h-[135px] w-[81.25vw] min-w-[260px] flex-col items-center justify-center rounded-3xl border-[5px] border-[#C6612B] bg-[#EAD8CA] lg:h-[21.63472vw] lg:w-[41.66vw]"
    >
      <div class="w-[17.1875vw] min-w-[55px] lg:w-[8.68vw]">
        <img src="./assets/done.png" alt="" />
      </div>
      <div class="text-center font-sans font-semibold">
        <p class="text-[6.25vw] text-[#5D9B84] lg:text-[2.77vw]">輸入成功</p>
        <p class="text-[3.75vw] text-[#402104] lg:text-[1.66vw]">
          敬請期待 消失的校慶
        </p>
      </div>
    </div>
  </div>
</template>

<script>
import { ref } from "vue";

document.onclick = function (e) {
  if (e.target.id == "jump") {
    document.getElementById("jump").classList.add("hidden");
    document.getElementById("jump").classList.remove("flex");
  }
};

export default {
  setup() {
    const email = ref("");
    const list = ref([]);
    const newList = JSON.parse(localStorage.getItem("List"));
    if (localStorage.getItem("List")) {
      list.value = newList;
    } else {
      list.value = [];
    }

    const push = function () {
      if (email.value == "") {
        return;
      }
      if (email.value.includes("@") & email.value.includes(".")) {
        document.getElementById("jump").classList.remove("hidden");
        document.getElementById("jump").classList.add("flex");
        list.value.push(email.value);
        localStorage.setItem("List", JSON.stringify(list.value));
        email.value = "";
      } else {
        return;
      }
    };
    return {
      email,
      list,
      newList,
      push,
    };
  },
};
</script>
