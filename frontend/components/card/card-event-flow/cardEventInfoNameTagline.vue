<template>
  <div class="my-8">
    <div class="flex justify-center card-style md:justify-start">
      <div class="flex flex-col p-2 w-full sm:px-5 sm:py-3 h-fit">
        <div class="pb-1 space-y-4">
      <div class="flex items-center space-x-4">
      </div>
      <div class="flex flex-col lg:flex-row gap-4 lg:gap-8">
        <div class="flex flex-col w-full lg:w-1/2">
          <label for="name" class="font-bold responsive-h4"
            >{{
              $t("pages.events.create.name")
            }}
            *</label
          >
          <input
            id="name"
            class="peer border border-light-text rounded-sm bg-transparent py-1 px-3 dark:border-dark-text"
            :placeholder="
              $t('pages.events.create.enter-name')
            "
          />
        </div>
        <div class="flex flex-col w-full lg:w-1/2">
          <label for="tagline" class="font-bold responsive-h4"
            >{{
              $t("pages.events.create.tagline")
            }}
            </label
          >
          <input
            id="tagline"
            class="peer border border-light-text rounded-sm bg-transparent py-1 px-3 dark:border-dark-text"
            :placeholder="
              $t('pages.events.create.enter-tagline')
            "
          />
        </div>
      </div>
    </div>
    </div>
    </div>
  </div>

  </template>
  
  <script setup lang="ts">

  </script>
  