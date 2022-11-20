<script setup lang="ts"></script>

<template>
  <div class="mx-auto max-w-960">
    <header class="">
      <nav>
        <ul class="flex">
          <li class="mr-32 py-20 text-2 font-semibold text-letters-primary">
            Converter
          </li>
          <li class="mr-32 py-20 text-2 font-semibold text-letters-primary">
            Prices
          </li>
        </ul>
      </nav>
      <span
        class="absolute left-0 right-0 border-b border-solid border-surface-secondary-03"
      ></span>
    </header>

    <main>
      <article>
        <h1 class="mt-64 text-title-1 font-semibold text-letters-primary">
          Bitcoin to US Dollar
        </h1>
        <h2
          class="mt-16 mb-32 text-title-2 font-medium text-letters-secondary-01"
        >
          1 BTC equals $16,607.04 USD
        </h2>

        <form class="flex w-full gap-64">
          <div class="flex w-full flex-col gap-8">
            <input
              type="number"
              class="rounded-4 border border-solid border-surface-secondary-03 p-16 pt-20 text-title-2 font-medium text-letters-secondary-01"
            />

            <input
              class="rounded-4 border border-solid border-surface-secondary-03 p-8 text-title-2 font-medium text-letters-secondary-01"
            />
          </div>

          <div class="flex w-full flex-col gap-8">
            <input
              type="number"
              class="rounded-4 border border-solid border-surface-secondary-03 p-16 pt-20 text-title-2 font-medium text-letters-secondary-01"
            />

            <input
              class="rounded-4 border border-solid border-surface-secondary-03 p-8 text-title-2 font-medium text-letters-secondary-01"
            />
          </div>
        </form>
      </article>
    </main>
  </div>
</template>
