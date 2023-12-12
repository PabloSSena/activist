<template>
    <div class="my-8">
      <div class="flex justify-center card-style md:justify-start">
        <div class="flex flex-col p-2 w-full sm:px-5 sm:py-3 h-fit">
          <div class="pb-1 space-y-4">
        <div class="flex items-center space-x-4">
        </div>
        <div class="flex flex-col lg:flex-row gap-4 lg:gap-8">
          <div class="flex flex-col w-full lg:w-1/1">
            <label for="name" class="font-bold responsive-h4"
              >{{
                $t("pages.events.create.connect")
              }}
              </label
            >
            <p>
              {{
                $t("pages.events.create.subheader")
              }}
            </p>
            <div class="flex items-center break-all cursor-pointer gap-3 transition-all">
              <Icon name="cib:instagram" size="1em" />
            <p class="sr-only sm:not-sr-only">
              testeaiai
            </p>
            <Icon name="bi:envelope" size="1.2em" />
            </div>

          </div>
      </div>
      </div>
      </div>
      </div>
    </div>
  
    </template>
    
    <script setup lang="ts">
    </script>
    