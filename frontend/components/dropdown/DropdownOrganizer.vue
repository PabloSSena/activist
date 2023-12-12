<template>
    <Menu as="div" class="relative inline-block text-left">
      <div>
        <MenuButton
          v-slot="{ open }"
          class="inline-flex w-full px-4 py-2 font-semibold select-none rounded-md style-btn"
          :aria-label="$t('components.dropdown-organizer')"
        >
          <div class="flex items-center text-sm space-x-2">
            <p
              class="sr-only lg:not-sr-only"

            >
              Bridge over borders
            </p>
            <Icon
              class="right-3"
              :class="{
                'rotate-180 transform': open,
                absolute: location === 'sideMenu',
              }"
              name="bi:chevron-down"
            />
          </div>
        </MenuButton>
      </div>
      <transition
        enter-active-class="transition duration-100 ease-out"
        enter-from-class="opacity-0 transform scale-95"
        enter-to-class="opacity-100 transform scale-100"
        leave-active-class="transition duration-75 ease-in"
        leave-from-class="opacity-100 transform scale-100"
        leave-to-class="opacity-0 transform scale-95"
      >
        <MenuItems
          class="inline-flex w-full px-4 py-2 font-semibold select-none rounded-md style-btn"
        >
          <div class="px-2 py-2">
            <MenuItem v-slot="{ active }">
                <p class="pl-2 pr-2">
                  Organization example
                </p>
            </MenuItem>
          </div>
        </MenuItems>
      </transition>
    </Menu>
  </template>
  
  <script setup lang="ts">
  import { Menu, MenuButton, MenuItem, MenuItems } from "@headlessui/vue";
  
  defineProps<{
    location?: string;
  }>();
  </script>
  