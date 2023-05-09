<template>
  <div class="">
    <div class="">
      <div class="max-w-2xl py-16">
        <h2 class="text-3xl font-bold tracking-tight text-gray-900 sm:text-4xl">
          Meet our Cool Squad
        </h2>
        <p class="mt-6 text-lg text-gray-600">
          We are cool people doing cool things about cool stuff on a cool
          framework.
        </p>
      </div>
      <ul
        role="list"
        class="grid gap-x-20 gap-y-12 grid-cols-1 md:grid-cols-2 lg:grid-cols-3 sm:gap-y-20 xl:col-span"
      >
        <li v-for="person in people" :key="person.name">
          <div class="flex flex-col items-center gap-x-5 gap-y-3">
            <img class="h-40 w-40 rounded-full" :src="person.imageUrl" alt="" />
            <h3
              class="text-base font-semibold leading-7 tracking-tight text-gray-900"
            >
              {{ person.name }}
            </h3>
            <p class="text-sm leading-6 text-gray-500">{{ person.role }}</p>
            <div class="grid content-center grid-cols-3 gap-x-5">
              <svg
                class="h-5 w-5 text-gray-400"
                width="24"
                height="24"
                viewBox="0 0 24 24"
                stroke-width="2"
                stroke="currentColor"
                fill="none"
                stroke-linecap="round"
                stroke-linejoin="round"
              >
                <path stroke="none" d="M0 0h24v24H0z" />
                <rect x="4" y="4" width="16" height="16" rx="4" />
                <circle cx="12" cy="12" r="3" />
                <line x1="16.5" y1="7.5" x2="16.5" y2="7.501" />
              </svg>
              <svg
                class="h-5 w-5 text-gray-400"
                viewBox="0 0 24 24"
                fill="none"
                stroke="currentColor"
                stroke-width="2"
                stroke-linecap="round"
                stroke-linejoin="round"
              >
                <path
                  d="M23 3a10.9 10.9 0 0 1-3.14 1.53 4.48 4.48 0 0 0-7.86 3v1A10.66 10.66 0 0 1 3 4s-4 9 5 13a11.64 11.64 0 0 1-7 2c9 5 20 0 20-11.5a4.5 4.5 0 0 0-.08-.83A7.72 7.72 0 0 0 23 3z"
                />
              </svg>
              <svg
                class="h-5 w-5 text-gray-400"
                viewBox="0 0 24 24"
                fill="none"
                stroke="currentColor"
                stroke-width="2"
                stroke-linecap="round"
                stroke-linejoin="round"
              >
                <path
                  d="M16 8a6 6 0 0 1 6 6v7h-4v-7a2 2 0 0 0-2-2 2 2 0 0 0-2 2v7h-4v-7a6 6 0 0 1 6-6z"
                />
                <rect x="2" y="9" width="4" height="12" />
                <circle cx="4" cy="4" r="2" />
              </svg>
            </div>
          </div>
        </li>
      </ul>
    </div>
  </div>
</template>

<script setup>
const people = [
  {
    name: "Mina Ali",
    role: "Cool CEO",
    imageUrl:
      "https://images.unsplash.com/photo-1683322001857-f4d932a40672?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=684&q=80",
  },
  {
    name: "Mena Ale",
    role: "Lit Lead Designer",
    imageUrl:
      "https://images.unsplash.com/photo-1683322001857-f4d932a40672?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=684&q=80",
  },
  {
    name: "Meena Alee",
    role: "Sick Lead Developer",
    imageUrl:
      "https://images.unsplash.com/photo-1683322001857-f4d932a40672?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=684&q=80",
  },
  {
    name: "Meana Alei",
    role: "Savage CTO",
    imageUrl:
      "https://images.unsplash.com/photo-1683322001857-f4d932a40672?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=684&q=80",
  },
  {
    name: "Meina Alii",
    role: "Rad Junior Designer",
    imageUrl:
      "https://images.unsplash.com/photo-1683322001857-f4d932a40672?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=684&q=80",
  },
  {
    name: "Minea Alli",
    role: "Slammin' Junior Developer",
    imageUrl:
      "https://images.unsplash.com/photo-1683322001857-f4d932a40672?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=684&q=80",
  },
  // More people...
];
</script>