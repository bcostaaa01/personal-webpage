<template>
  <div class="flex flex-col items-start h-screen ml-10">
    <h1 class="text-8xl italic">Bruno Costa</h1>

    <h2 class="text-4xl mt-10">
      Meet me, a passionate developer with an affinity for:
      <ul class="list-disc ml-12 my-4 italic">
        <li><span class="text-blue-500">the web</span></li>
        <li><span class="text-blue-500">beautiful design</span></li>
        <li><span class="text-blue-500">smooth user experiences</span></li>
      </ul>
    </h2>

    <div class="flex flex-col lg:flex-row items-start h-screen mr-10">
      <HomePageContainer class="lg:w-1/2 w-full">
        <Card title="A little bit about me" date="2022-10-10" formattedDate="20th of January 2025" content="Hi!👋🏻I am Bruno Costa, a passionate software and web developer from Portugal. I am also a computer
              science student and when I am not studying or working, I am either enjoying time with friends, hobbies,
              music, or
              just building new things.🏗️" imageSrc="https://avatars.githubusercontent.com/u/72168158?v=4"
          imageAlt="My Image" class="w-full">

          <div class="">
            <p class="mt-2 line-clamp-3 text-xl/relaxed text-gray-500">
              Hi!👋🏻I am Bruno Costa, a passionate software and web developer from Portugal. I am also a computer
              science student and when I am not studying or working, I am either enjoying time with friends, hobbies,
              music, or
              just building new things.🏗️
            </p>

            <h3 class="text-2xl mt-4">Some of my favourite technologies</h3>

            <ul class="list-disc ml-4 mt-4 text-xl list-inside">
              <div class="flex items-center">
                <span class="text-blue-500 mr-2">🖥️ </span>
                <span class="italic">JavaScript, TypeScript</span>
              </div>
              <div class="flex items-center">
                <span class="text-blue-500 mr-2">⚙️</span>
                <span class="italic">Vue.js, Vue-Router, Pinia</span>
              </div>
              <div class="flex items-center">
                <span class="mr-2">⚛️</span>
                <span class="italic">React, React/Tanstack-Query</span>
              </div>
              <div class="flex items-center">
                <span class="mr-2">🎨</span>
                <span class="italic">CSS, Tailwind CSS</span>
              </div>
              <div class="flex items-center">
                <span class="text-blue-500 mr-2">🧪</span>
                <span class="italic">Vite, Vitest, Storybook, Chromatic</span>
              </div>
            </ul>
          </div>
        </Card>
      </HomePageContainer>

      <HomePageContainer class="lg:w-1/2 w-full lg:ml-10 lg:mr-0">
        <Card title="Contact me" content="I am always open to new opportunities and collaborations. If you have any questions or want to work
                together, please don't hesitate to contact me." class="w-full">

          <div>
            <p class="mt-2 line-clamp-3 text-xl/relaxed text-gray-500">
              I am always open to new opportunities and collaborations. If you have any questions or want to work
              together, please don't hesitate to contact me.
            </p>

            <span class="text-xl mt-4 flex flex-row items-center">
              <span>You can also download my resume ⬇️</span>
            </span>

            <a href="https://drive.google.com/file/d/1R3qXv7ukgp8lQbOtL4FAmxTEZeLt72B3/view?usp=sharing"
              class="text-blue-500 underline">Download</a>
          </div>

          <div class="flex flex-row items-center justify-center m-4">
            <a href="https://www.linkedin.com/in/bruno-miguel-alves-costa/"
              class="text-blue-500 underline mr-4">LinkedIn</a>
            <a href="https://github.com/bcostaaa01" class="text-blue-500 underline mr-4">GitHub</a>
            <a href="https://dev.to/bcostaaa01" class="text-blue-500 underline">My articles</a>
            <a href="mailto:bcostaaa01@gmail.com" class="text-blue-500 underline ml-4">Email</a>
          </div>
        </Card>
      </HomePageContainer>
    </div>
  </div>
</template>

<script setup lang="ts">
import Card from '../components/UI/Card.vue';
</script>
