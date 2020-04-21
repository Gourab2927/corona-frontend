<template>
  <main class="container">
    <div class="w-full bg-gray-300 rounded p-4">
      <h1 class="text-2xl font-bold text-center">
        {{ $t('about_coronatracker') }}
      </h1>
      <p class="pt-4">
        {{ $t('whats_coronatracker') }}
      </p>

      <p class="pt-4">
        {{ $t('whats_coronatracker_2') }}
      </p>

      <p class="pt-4">
        {{ $t('whats_coronatracker_3') }}
      </p>

      <p class="pt-4">
        {{ $t('whats_coronatracker_4') }}
      </p>

      <p class="pt-4">
        {{ $t('whats_coronatracker_5') }}
      </p>

      <p class="pt-4 pb-4">
        {{ $t('whats_coronatracker_6') }}
      </p>

      <em class="pt-4">
        {{ $t('whats_coronatracker_7') }}
      </em>
    </div>
    <div class="flex flex-wrap -mx-2 my-4">
      <div class="w-full px-2">
        <h1 class="text-2xl font-bold mb-4 text-center text-primary">
          {{ $t('sources') }}
        </h1>
        <div>
          {{ $t('sources_handpicked') }}
        </div>

        <table class="table-auto mt-4 mb-4">
          <thead>
          <tr>
            <th class="px-4 py-2 w-1/3">{{ $t('title') }}</th>
            <th class="px-4 py-2 w-1/2">{{ $t('description') }}</th>
            <th class="px-4 py-2">{{ $t('source') }}</th>
          </tr>
          </thead>
          <tbody>
          <tr>
            <td class="border px-4 py-2">
              <a
                class="hover:underline"
                target="_blank"
                rel="noopener"
                href="https://www.thelancet.com/journals/lancet/article/PIIS0140-6736(20)30185-9/fulltext"
              >{{ $t('report_1_title') }}</a
              >
            </td>
            <td class="border px-4 py-2">
              {{ $t('report_1_description') }}
            </td>
            <td class="border px-4 py-2">The Lancet</td>
          </tr>
          <tr class="bg-gray-100">
            <td class="border px-4 py-2">
              <a
                class="hover:underline"
                target="_blank"
                rel="noopener"
                href="https://www.nejm.org/doi/full/10.1056/NEJMe2001126"
              >{{ $t('report_2_title') }}</a
              >
            </td>
            <td class="border px-4 py-2">
              {{ $t('report_2_description') }}
            </td>
            <td class="border px-4 py-2">
              The New England Journal of Medicine
            </td>
          </tr>
          <tr>
            <td class="border px-4 py-2">
              <a
                class="hover:underline"
                target="_blank"
                rel="noopener"
                href="https://gisanddata.maps.arcgis.com/apps/opsdashboard/index.html#/bda7594740fd40299423467b48e9ecf6"
              >{{ $t('report_3_title') }}</a
              >
            </td>
            <td class="border px-4 py-2">
              {{ $t('report_3_description') }}
            </td>
            <td class="border px-4 py-2">
              John Hopkins University
            </td>
          </tr>
          </tbody>
        </table>
        <div class="mt-8">
          {{ $t('report_inaccuracies') }}
          <a
            class="underline"
            href="https://docs.google.com/forms/d/1A5Sw_gdJ6tsHA74Bz2_2uVMKqf9k_APRMQIAEoSXSNY/viewform?edit_requested=true"
          >{{ $t('form') }}</a
          >.
        </div>
      </div>
    </div>

    </div>
   </div>
      </div>
    </div>
  </main>
</template>
<script>
  export default {
    head() {
      const title = this.$t('about_coronatracker');
      const description = this.$t('about_coronatracker_meta_description');

      return {
        title,
        meta: [
          { hid: 'title', name: 'title', content: title },
          { hid: 'description', name: 'description', content: description },
          { hid: 'og-title', property: 'og:title', content: title },
          { hid: 'og-description', property: 'og:title', content: description },
          { hid: 'twitter-title', property: 'twitter:title', content: title },
          { hid: 'twitter-description', property: 'twitter:title', content: description },
        ],
      };
    },
  };
</script>
<style scoped>
  li a:hover {
    color: #38a169;
  }

  .hero {
    display: flex;
    justify-content: center;
  }

  .hero img {
    border-radius: 50%;
    display: block;
    height: 100px;
    width: 100px;
    margin: 0 auto;
  }

  .hero .hero-info {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }

  .member {
    text-align: center;
  }
</style>
