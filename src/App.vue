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

            <ul>
              <li v-for="coin in coinsMockData" :key="coin.ticker">
                {{ coin.ticker }}
              </li>
            </ul>
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

<script setup lang="ts">
interface coinData {
  rate_change: number;
  name: string;
  ticker: string;
  sparkline: string;
  current_rate: {
    cents: number;
    currency_iso: string;
  };
}

const coinsMockData: coinData[] = [
  {
    rate_change: -2.755663101537995,
    name: "Bitcoin",
    ticker: "BTC",
    sparkline:
      "https://cpay-sparklines.s3.eu-west-2.amazonaws.com/sparklines/day/BTCUSD.svg",
    current_rate: {
      cents: 1633363,
      currency_iso: "USD",
    },
  },
  {
    rate_change: 0.44354624334891557,
    name: "Tether USD",
    ticker: "USDT",
    sparkline:
      "https://cpay-sparklines.s3.eu-west-2.amazonaws.com/sparklines/day/USDTUSD.svg",
    current_rate: { cents: 100, currency_iso: "USD" },
  },
  {
    rate_change: 0.4763729562043007,
    name: "USD Coin",
    ticker: "USDC",
    sparkline:
      "https://cpay-sparklines.s3.eu-west-2.amazonaws.com/sparklines/day/USDCUSD.svg",
    current_rate: { cents: 100, currency_iso: "USD" },
  },
  {
    rate_change: -6.835321065542208,
    name: "Ethereum",
    ticker: "ETH",
    sparkline:
      "https://cpay-sparklines.s3.eu-west-2.amazonaws.com/sparklines/day/ETHUSD.svg",
    current_rate: { cents: 114406, currency_iso: "USD" },
  },
  {
    rate_change: -12.322191079590691,
    name: "NEAR Protocol",
    ticker: "NEAR",
    sparkline:
      "https://cpay-sparklines.s3.eu-west-2.amazonaws.com/sparklines/day/NEARUSD.svg",
    current_rate: { cents: 154, currency_iso: "USD" },
  },
  {
    rate_change: -3.7218406540561966,
    name: "Litecoin",
    ticker: "LTC",
    sparkline:
      "https://cpay-sparklines.s3.eu-west-2.amazonaws.com/sparklines/day/LTCUSD.svg",
    current_rate: { cents: 6131, currency_iso: "USD" },
  },
  {
    rate_change: -8.70581943386463,
    name: "XRP",
    ticker: "XRP",
    sparkline:
      "https://cpay-sparklines.s3.eu-west-2.amazonaws.com/sparklines/day/XRPUSD.svg",
    current_rate: { cents: 36, currency_iso: "USD" },
  },
  {
    rate_change: -9.105792413621606,
    name: "Solana",
    ticker: "SOL",
    sparkline:
      "https://cpay-sparklines.s3.eu-west-2.amazonaws.com/sparklines/day/SOLUSD.svg",
    current_rate: { cents: 1195, currency_iso: "USD" },
  },
  {
    rate_change: -5.667857219672152,
    name: "Aave",
    ticker: "AAVE",
    sparkline:
      "https://cpay-sparklines.s3.eu-west-2.amazonaws.com/sparklines/day/AAVEUSD.svg",
    current_rate: { cents: 5705, currency_iso: "USD" },
  },
];
</script>
