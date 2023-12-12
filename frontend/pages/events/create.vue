<template>
  <div class="w-full text-light-text dark:text-dark-text">
    <ProgressBar type="default" :progress="1" :start="1" :end="1" />
    <div class="flex flex-col px-4 xl:px-8">
      <PageBreadcrumbs class="mt-2" :breadcrumbs="breadcrumbs" />
      <div class="mt-4">
        <h1 class="font-bold responsive-h2">
          {{ $t("pages._global.information") }}
        </h1>
      </div>
      <p>
        {{ $t("pages.events.create.information") }}
      </p>
      <CardEventInfoNameTagline></CardEventInfoNameTagline>
      <CardEventInfoOrganizer></CardEventInfoOrganizer>
      <CardEventInfoConnect></CardEventInfoConnect>
      <div class="pt-3 pb-6 space-y-6 md:pt-4 w-1/2">
        <CardDatePicker />
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
import CardEventInfo from '~/components/card/card-event-flow/cardEventInfo.vue';
import CardEventInfoNameTagline from '~/components/card/card-event-flow/cardEventInfoNameTagline.vue';
import CardEventInfoOrganizer from '~/components/card/card-event-flow/CardEventInfoOrganizer.vue';
import CardEventInfoConnect from '~/components/card/card-event-flow/CardEventInfoConnect.vue';
definePageMeta({
  layout: "sidebar",
});
</script>
