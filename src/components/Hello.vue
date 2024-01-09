<script setup>
import { Typed } from "@duskmoon/vue3-typed-js";
import {
  PhoneOutlined,
  FacebookOutlined,
  MailOutlined,
  LinkedinOutlined,
  GithubOutlined,
} from "@ant-design/icons-vue";
import moment from "moment";

import Skill from "./Skill.vue";

const options = {
  strings: [
    "FrontEnd Developer",
    "BackEnd Developer",
    "Full Stack Developer",
    "person, who learns knowledge to be a Devops Engineer",
    "Technical Leader, it's joke",
  ],
  loop: true,
  typeSpeed: 50,
};
</script>

<template>
  <div class="p-8 hello__background h-screen flex flex-col justify-between">
    <div>
      <div class="bg-white p-4">
        Hello, I'm
        <h1 class="text-2xl font-semibold my-2">Vương Toàn Thắng</h1>
        find me on the internet with nickname
        <span class="font-semibold text-green-600">Desod</span>
      </div>

      <div class="my-4">
        <p class="font-bold mb-1">Summary</p>
        <div class="hidden md:block">
          <p>
            - With knowledge, creation and passion, I always find, learn and work to be an
            expert in major, which i follow.
          </p>
          <p>
            - Keep curiosity will lead me to discover and grow on career path and self
            growth, better and better.
          </p>
        </div>
        <br />
        <Typed :options="options">
          <span
            >Now, I'm working as a
            <h1 class="typing inline text-green-400"></h1
          ></span>
        </Typed>
      </div>

      <ul class="list-disc border-t mt-10 px-6">
        
        <li>&#127969; Ha Noi, Viet Nam</li>
        <li>&#128266; Languages: Vietnamese, English</li>
      </ul>
    </div>

    <Skill />

    <div class="mt-2 flex justify-center gap-x-4">
      <a
        href="tel:+84389064540"
        target="_blank"
        class="bg-white flex justify-center items-center p-3 rounded-full"
      >
        <PhoneOutlined />
      </a>

      <a
        href="mailto:thangdotpro@gmail.com"
        target="_blank"
        class="bg-white flex justify-center items-center p-3 rounded-full"
      >
        <MailOutlined />
      </a>

      <a
        href="https://www.facebook.com/desod.profile/"
        target="_blank"
        class="bg-white flex justify-center items-center p-3 rounded-full"
      >
        <FacebookOutlined />
      </a>

      <a
        href="https://www.linkedin.com/in/desod/"
        target="_blank"
        class="bg-white flex justify-center items-center p-3 rounded-full"
      >
        <LinkedinOutlined />
      </a>

      <a
        href="https://github.com/desod-vn"
        target="_blank"
        class="bg-white flex justify-center items-center p-3 rounded-full"
      >
        <GithubOutlined />
      </a>
    </div>
  </div>
</template>
<style scoped lang="scss">
.hello {
  &__background {
    background: linear-gradient(
      to right,
      rgba(255, 255, 255, 0.2) 0%,
      rgba(102, 95, 95, 0.4) 100%
    );
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
  }
}
</style>
