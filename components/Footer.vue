<script>
export default {
  name: "Footer"
}
</script>

<template>
<!--  <footer class="p-4 bg-grey rounded-lg shadow md:flex md:items-center md:justify-between md:p-6 dark:bg-gray-800">
    <span class="text-sm text-gray-500 sm:text-center dark:text-gray-400">© 2022 <a href="https://flowbite.com/" class="hover:underline">Flowbite™</a>. All Rights Reserved.
    </span>
    <ul class="flex flex-wrap items-center mt-3 text-sm text-gray-500 dark:text-gray-400 sm:mt-0">
      <li>
        <a href="#" class="mr-4 hover:underline md:mr-6 ">About</a>
      </li>
      <li>
        <a href="#" class="mr-4 hover:underline md:mr-6">Privacy Policy</a>
      </li>
      <li>
        <a href="#" class="mr-4 hover:underline md:mr-6">Licensing</a>
      </li>
      <li>
        <a href="#" class="hover:underline">Contact</a>
      </li>
    </ul>
  </footer>-->
  <footer class="text-center lg:text-left bg-gray-100 text-gray-600 mt-4 lg:mt-0 lg:relative lg:bottom-0 lg:left-0">
    <div class="flex justify-center items-center lg:justify-between p-6 border-b border-gray-300">
      <div class="mr-12 hidden lg:block">
        <span>Get connected with me on social networks:</span>
      </div>
      <div class="flex justify-center">
        <a href="https://www.linkedin.com/in/nicolai-driga-21b76a229/" target="_blank" class="mr-6 text-gray-600">
          <svg aria-hidden="true" focusable="false" data-prefix="fab" data-icon="linkedin-in"
               class="w-3.5" role="img" xmlns="http://www.w3.org/2000/svg"
               viewBox="0 0 448 512">
            <path fill="currentColor"
                  d="M100.28 448H7.4V148.9h92.88zM53.79 108.1C24.09 108.1 0 83.5 0 53.8a53.79 53.79 0 0 1 107.58 0c0 29.7-24.1 54.3-53.79 54.3zM447.9 448h-92.68V302.4c0-34.7-.7-79.2-48.29-79.2-48.29 0-55.69 37.7-55.69 76.7V448h-92.78V148.9h89.08v40.8h1.3c12.4-23.5 42.69-48.3 87.88-48.3 94 0 111.28 61.9 111.28 142.3V448z">
            </path>
          </svg>
        </a>
        <a href="https://github.com/DrigaNicolai" target="_blank" class="text-gray-600">
          <svg aria-hidden="true" focusable="false" data-prefix="fab" data-icon="github"
               class="w-4" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 496 512">
            <path fill="currentColor"
                  d="M165.9 397.4c0 2-2.3 3.6-5.2 3.6-3.3.3-5.6-1.3-5.6-3.6 0-2 2.3-3.6 5.2-3.6 3-.3 5.6 1.3 5.6 3.6zm-31.1-4.5c-.7 2 1.3 4.3 4.3 4.9 2.6 1 5.6 0 6.2-2s-1.3-4.3-4.3-5.2c-2.6-.7-5.5.3-6.2 2.3zm44.2-1.7c-2.9.7-4.9 2.6-4.6 4.9.3 2 2.9 3.3 5.9 2.6 2.9-.7 4.9-2.6 4.6-4.6-.3-1.9-3-3.2-5.9-2.9zM244.8 8C106.1 8 0 113.3 0 252c0 110.9 69.8 205.8 169.5 239.2 12.8 2.3 17.3-5.6 17.3-12.1 0-6.2-.3-40.4-.3-61.4 0 0-70 15-84.7-29.8 0 0-11.4-29.1-27.8-36.6 0 0-22.9-15.7 1.6-15.4 0 0 24.9 2 38.6 25.8 21.9 38.6 58.6 27.5 72.9 20.9 2.3-16 8.8-27.1 16-33.7-55.9-6.2-112.3-14.3-112.3-110.5 0-27.5 7.6-41.3 23.6-58.9-2.6-6.5-11.1-33.3 2.6-67.9 20.9-6.5 69 27 69 27 20-5.6 41.5-8.5 62.8-8.5s42.8 2.9 62.8 8.5c0 0 48.1-33.6 69-27 13.7 34.7 5.2 61.4 2.6 67.9 16 17.7 25.8 31.5 25.8 58.9 0 96.5-58.9 104.2-114.8 110.5 9.2 7.9 17 22.9 17 46.4 0 33.7-.3 75.4-.3 83.6 0 6.5 4.6 14.4 17.3 12.1C428.2 457.8 496 362.9 496 252 496 113.3 383.5 8 244.8 8zM97.2 352.9c-1.3 1-1 3.3.7 5.2 1.6 1.6 3.9 2.3 5.2 1 1.3-1 1-3.3-.7-5.2-1.6-1.6-3.9-2.3-5.2-1zm-10.8-8.1c-.7 1.3.3 2.9 2.3 3.9 1.6 1 3.6.7 4.3-.7.7-1.3-.3-2.9-2.3-3.9-2-.6-3.6-.3-4.3.7zm32.4 35.6c-1.6 1.3-1 4.3 1.3 6.2 2.3 2.3 5.2 2.6 6.5 1 1.3-1.3.7-4.3-1.3-6.2-2.2-2.3-5.2-2.6-6.5-1zm-11.4-14.7c-1.6 1-1.6 3.6 0 5.9 1.6 2.3 4.3 3.3 5.6 2.3 1.6-1.3 1.6-3.9 0-6.2-1.4-2.3-4-3.3-5.6-2z">
            </path>
          </svg>
        </a>
      </div>
    </div>
    <div class="mx-6 py-10 text-center md:text-left">
      <div class="grid grid-1 md:grid-cols-2 lg:grid-cols-4 gap-8">
        <div class="">
          <h6 class="
            uppercase
            font-semibold
            mb-4
            flex
            items-center
            justify-center
            md:justify-start
          ">
            Info
          </h6>
          <p>
            This is my try to implement my knowledge about Nuxt.js and Tailwind in one simple project.
          </p>
          <p>
            This project has not so many pages or functions, but it is like an example and practical task to cope with new framework and CSS styles library.
          </p>
        </div>
        <div class="">
          <h6 class="uppercase font-semibold mb-4 flex justify-center md:justify-start">
            Frameworks & Libraries
          </h6>
          <p class="mb-4">
            <a href="https://nuxtjs.org/" target="_blank" class="text-gray-600">NuxtJS</a>
          </p>
          <p>
            <a href="https://tailwindcss.com/" target="_blank" class="text-gray-600">Tailwind</a>
          </p>
        </div>
        <div class="">
          <h6 class="uppercase font-semibold mb-4 flex justify-center md:justify-start">
            Useful links
          </h6>
          <p class="mb-4">
            <a href="https://tailwind-elements.com/" target="_blank" class="text-gray-600">Tailwind Elements</a>
          </p>
          <p class="mb-4">
            <a href="https://flowbite.com" target="_blank" class="text-gray-600">Flowbite</a>
          </p>
          <p class="mb-4">
            <a href="https://www.pinterest.com/" target="_blank" class="text-gray-600">Pinterest</a>
          </p>
        </div>
        <div class="">
          <h6 class="uppercase font-semibold mb-4 flex justify-center md:justify-start">
            Contact
          </h6>
          <p class="flex items-center justify-center md:justify-start mb-4">
            <svg aria-hidden="true" focusable="false" data-prefix="fas" data-icon="envelope"
                 class="w-4 mr-4" role="img" xmlns="http://www.w3.org/2000/svg"
                 viewBox="0 0 512 512">
              <path fill="currentColor"
                    d="M502.3 190.8c3.9-3.1 9.7-.2 9.7 4.7V400c0 26.5-21.5 48-48 48H48c-26.5 0-48-21.5-48-48V195.6c0-5 5.7-7.8 9.7-4.7 22.4 17.4 52.1 39.5 154.1 113.6 21.1 15.4 56.7 47.8 92.2 47.6 35.7.3 72-32.8 92.3-47.6 102-74.1 131.6-96.3 154-113.7zM256 320c23.2.4 56.6-29.2 73.4-41.4 132.7-96.3 142.8-104.7 173.4-128.7 5.8-4.5 9.2-11.5 9.2-18.9v-19c0-26.5-21.5-48-48-48H48C21.5 64 0 85.5 0 112v19c0 7.4 3.4 14.3 9.2 18.9 30.6 23.9 40.7 32.4 173.4 128.7 16.8 12.2 50.2 41.8 73.4 41.4z">
              </path>
            </svg>
            drigans_22@mail.ru
          </p>
          <p class="flex items-center justify-center md:justify-start mb-4">
            <svg aria-hidden="true" focusable="false" data-prefix="fas" data-icon="envelope"
                 class="w-4 mr-4" role="img" xmlns="http://www.w3.org/2000/svg"
                 viewBox="0 0 512 512">
              <path fill="currentColor"
                    d="M502.3 190.8c3.9-3.1 9.7-.2 9.7 4.7V400c0 26.5-21.5 48-48 48H48c-26.5 0-48-21.5-48-48V195.6c0-5 5.7-7.8 9.7-4.7 22.4 17.4 52.1 39.5 154.1 113.6 21.1 15.4 56.7 47.8 92.2 47.6 35.7.3 72-32.8 92.3-47.6 102-74.1 131.6-96.3 154-113.7zM256 320c23.2.4 56.6-29.2 73.4-41.4 132.7-96.3 142.8-104.7 173.4-128.7 5.8-4.5 9.2-11.5 9.2-18.9v-19c0-26.5-21.5-48-48-48H48C21.5 64 0 85.5 0 112v19c0 7.4 3.4 14.3 9.2 18.9 30.6 23.9 40.7 32.4 173.4 128.7 16.8 12.2 50.2 41.8 73.4 41.4z">
              </path>
            </svg>
            just.whyme7@gmail.com
          </p>
          <p class="flex items-center justify-center md:justify-start mb-4">
            <svg aria-hidden="true" focusable="false" data-prefix="fas" data-icon="envelope"
                 class="w-4 mr-4" role="img" xmlns="http://www.w3.org/2000/svg"
                 viewBox="0 0 512 512">
              <path fill="currentColor"
                    d="M502.3 190.8c3.9-3.1 9.7-.2 9.7 4.7V400c0 26.5-21.5 48-48 48H48c-26.5 0-48-21.5-48-48V195.6c0-5 5.7-7.8 9.7-4.7 22.4 17.4 52.1 39.5 154.1 113.6 21.1 15.4 56.7 47.8 92.2 47.6 35.7.3 72-32.8 92.3-47.6 102-74.1 131.6-96.3 154-113.7zM256 320c23.2.4 56.6-29.2 73.4-41.4 132.7-96.3 142.8-104.7 173.4-128.7 5.8-4.5 9.2-11.5 9.2-18.9v-19c0-26.5-21.5-48-48-48H48C21.5 64 0 85.5 0 112v19c0 7.4 3.4 14.3 9.2 18.9 30.6 23.9 40.7 32.4 173.4 128.7 16.8 12.2 50.2 41.8 73.4 41.4z">
              </path>
            </svg>
            driga.nicolai@powerit.md
          </p>
        </div>
      </div>
    </div>
    <div class="text-center p-6 bg-gray-200">
      <span>© 2022 Copyright: </span>
      <a class="text-gray-600 font-semibold" href="https://github.com/DrigaNicolai/nuxt_little_test_project" target="_blank">Nuxt & Tailwind Project</a>
    </div>
  </footer>
</template>

<style scoped></style>
