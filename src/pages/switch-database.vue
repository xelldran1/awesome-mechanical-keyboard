<template>
  <Layout>
    <div class="w-full mx-auto py-16">
      <h2 class="text-4xl font-bold mb-16">Mechanical Keyboard Switch Database</h2>

      <form class="w-full max-w-lg" name="addSwitch" data-netlify="true">
        <div class="flex flex-wrap -mx-3 mb-6">
          <div class="w-full md:w-1/2 px-3 mb-6 md:mb-0">
            <label
              class="block uppercase tracking-wide text-gray-700 text-xs font-bold mb-2"
              for="grid-brand"
            >Brand</label>
            <input
              class="appearance-none block w-full bg-gray-200 text-gray-700 border rounded py-3 px-4 mb-3 leading-tight focus:outline-none focus:bg-white"
              id="grid-brand"
              type="text"
              placeholder="Kailh"
            />
          </div>
          <div class="w-full md:w-1/2 px-3">
            <label
              class="block uppercase tracking-wide text-gray-700 text-xs font-bold mb-2"
              for="grid-model"
            >Model</label>
            <input
              class="appearance-none block w-full bg-gray-200 text-gray-700 border border-gray-200 rounded py-3 px-4 leading-tight focus:outline-none focus:bg-white focus:border-gray-500"
              id="grid-model"
              type="text"
              placeholder="Box Jade"
            />
          </div>
        </div>
        <div class="flex flex-wrap -mx-3 mb-6">
          <div class="w-full px-3">
            <label
              class="block uppercase tracking-wide text-gray-700 text-xs font-bold mb-2"
              for="grid-action"
            >Action</label>
            <div class="relative">
              <select
                class="block appearance-none w-full bg-gray-200 border border-gray-200 text-gray-700 py-3 px-4 pr-8 rounded leading-tight focus:outline-none focus:bg-white focus:border-gray-500"
                id="grid-action"
              >
                <option>Linear</option>
                <option>Tactile</option>
                <option>Clicky</option>
              </select>
              <div
                class="pointer-events-none absolute inset-y-0 right-0 flex items-center px-2 text-gray-700"
              >
                <svg
                  class="fill-current h-4 w-4"
                  xmlns="http://www.w3.org/2000/svg"
                  viewBox="0 0 20 20"
                >
                  <path
                    d="M9.293 12.95l.707.707L15.657 8l-1.414-1.414L10 10.828 5.757 6.586 4.343 8z"
                  />
                </svg>
              </div>
            </div>
          </div>
        </div>

        <div class="flex flex-wrap -mx-3 mb-6">
          <div class="w-full px-3">
            <label
              class="block uppercase tracking-wide text-gray-700 text-xs font-bold mb-2"
              for="grid-keycap-mount"
            >Keycap Mount</label>
            <div class="relative">
              <select
                class="block appearance-none w-full bg-gray-200 border border-gray-200 text-gray-700 py-3 px-4 pr-8 rounded leading-tight focus:outline-none focus:bg-white focus:border-gray-500"
                id="grid-keycap-mount"
              >
                <option>MX</option>
                <option>Alps</option>
              </select>
              <div
                class="pointer-events-none absolute inset-y-0 right-0 flex items-center px-2 text-gray-700"
              >
                <svg
                  class="fill-current h-4 w-4"
                  xmlns="http://www.w3.org/2000/svg"
                  viewBox="0 0 20 20"
                >
                  <path
                    d="M9.293 12.95l.707.707L15.657 8l-1.414-1.414L10 10.828 5.757 6.586 4.343 8z"
                  />
                </svg>
              </div>
            </div>
          </div>
        </div>

        <div class="flex flex-wrap -mx-3 mb-6">
          <div class="w-full px-3">
            <label
              class="block uppercase tracking-wide text-gray-700 text-xs font-bold mb-2"
              for="grid-stem-color"
            >Stem Color</label>
            <input
              class="appearance-none block w-full bg-gray-200 text-gray-700 border border-gray-200 rounded py-3 px-4 mb-3 leading-tight focus:outline-none focus:bg-white focus:border-gray-500"
              id="grid-stem-color"
              type="text"
            />
            <p class="text-gray-600 text-xs italic">Blue, White, Jade, ...</p>
          </div>
        </div>

        <div class="flex flex-wrap -mx-3 mb-6">
          <div class="w-full px-3">
            <label
              class="block uppercase tracking-wide text-gray-700 text-xs font-bold mb-2"
              for="grid-spring-color"
            >Spring Color</label>
            <div class="relative">
              <select
                class="block appearance-none w-full bg-gray-200 border border-gray-200 text-gray-700 py-3 px-4 pr-8 rounded leading-tight focus:outline-none focus:bg-white focus:border-gray-500"
                id="grid-spring-color"
              >
                <option>Silver</option>
                <option>Gold</option>
              </select>
              <div
                class="pointer-events-none absolute inset-y-0 right-0 flex items-center px-2 text-gray-700"
              >
                <svg
                  class="fill-current h-4 w-4"
                  xmlns="http://www.w3.org/2000/svg"
                  viewBox="0 0 20 20"
                >
                  <path
                    d="M9.293 12.95l.707.707L15.657 8l-1.414-1.414L10 10.828 5.757 6.586 4.343 8z"
                  />
                </svg>
              </div>
            </div>
          </div>
        </div>

        <div class="flex flex-wrap -mx-3 mb-6">
          <div class="w-full md:w-1/2 px-3 mb-6 md:mb-0">
            <label
              class="block uppercase tracking-wide text-gray-700 text-xs font-bold mb-2"
              for="grid-color-top"
            >Housing Top Color</label>
            <input
              class="appearance-none block w-full bg-gray-200 text-gray-700 border border-gray-200 rounded py-3 px-4 mb-3 leading-tight focus:outline-none focus:bg-white focus:border-gray-500"
              id="grid-color-top"
              type="text"
            />
          </div>
          <div class="w-full md:w-1/2 px-3 mb-6 md:mb-0">
            <label
              class="block uppercase tracking-wide text-gray-700 text-xs font-bold mb-2"
              for="grid-color-bottom"
            >Housing Bottom Color</label>
            <input
              class="appearance-none block w-full bg-gray-200 text-gray-700 border border-gray-200 rounded py-3 px-4 mb-3 leading-tight focus:outline-none focus:bg-white focus:border-gray-500"
              id="grid-color-bottom"
              type="text"
            />
          </div>
        </div>

        <div class="flex flex-wrap -mx-3 mb-6">
          <div class="w-full px-3">
            <label
              class="block uppercase tracking-wide text-gray-700 text-xs font-bold mb-2"
              for="grid-switch-mount"
            >Switch Mount</label>
            <div class="relative">
              <select
                class="block appearance-none w-full bg-gray-200 border border-gray-200 text-gray-700 py-3 px-4 pr-8 rounded leading-tight focus:outline-none focus:bg-white focus:border-gray-500"
                id="grid-switch-mount"
              >
                <option>Plate</option>
                <option>PCB</option>
              </select>
              <div
                class="pointer-events-none absolute inset-y-0 right-0 flex items-center px-2 text-gray-700"
              >
                <svg
                  class="fill-current h-4 w-4"
                  xmlns="http://www.w3.org/2000/svg"
                  viewBox="0 0 20 20"
                >
                  <path
                    d="M9.293 12.95l.707.707L15.657 8l-1.414-1.414L10 10.828 5.757 6.586 4.343 8z"
                  />
                </svg>
              </div>
            </div>
          </div>
        </div>

        <div class="flex flex-wrap -mx-3 mb-6">
          <div class="w-full px-3">
            <label
              class="block uppercase tracking-wide text-gray-700 text-xs font-bold mb-2"
              for="grid-sense-method"
            >Sense Method</label>
            <input
              class="appearance-none block w-full bg-gray-200 text-gray-700 border border-gray-200 rounded py-3 px-4 mb-3 leading-tight focus:outline-none focus:bg-white focus:border-gray-500"
              id="grid-sense-method"
              type="text"
              placeholder="Metal leaf"
            />
          </div>
        </div>

        <div class="flex flex-wrap -mx-3 mb-6">
          <div class="w-full px-3">
            <label
              class="block uppercase tracking-wide text-gray-700 text-xs font-bold mb-2"
              for="grid-led-style"
            >Led Style</label>
            <input
              class="appearance-none block w-full bg-gray-200 text-gray-700 border border-gray-200 rounded py-3 px-4 mb-3 leading-tight focus:outline-none focus:bg-white focus:border-gray-500"
              id="grid-led-style"
              type="text"
            />
            <p class="text-gray-600 text-xs italic">SMD, 2 pin,...</p>
          </div>
        </div>

        <div class="flex flex-wrap -mx-3 mb-6">
          <div class="w-full mb-4 mx-3 border-b-2 block text-gray-500 font-bold">Travel</div>
          <div class="w-full md:w-1/2 px-3 mb-6 md:mb-0">
            <label
              class="block uppercase tracking-wide text-gray-700 text-xs font-bold mb-2"
              for="grid-travel-actuation"
            >Actuation (mm)</label>
            <input
              class="appearance-none block w-full py-3 px-4 mb-3 bg-gray-200 text-gray-700 border rounded leading-tight focus:outline-none focus:bg-white"
              id="grid-travel-actuation"
              type="number"
            />
            <p
              class="text-gray-600 text-xs italic"
            >The actuation travel is the distance at which the switch registers a key press.</p>
          </div>
          <div class="w-full md:w-1/2 px-3">
            <label
              class="block uppercase tracking-wide text-gray-700 text-xs font-bold mb-2"
              for="grid-travel-bottom-out"
            >Bottom out (mm)</label>
            <input
              class="appearance-none block w-full py-3 px-4 mb-3 bg-gray-200 text-gray-700 border rounded leading-tight focus:outline-none focus:bg-white"
              id="grid-travel-bottom-out"
              type="number"
            />
            <p
              class="text-gray-600 text-xs italic"
            >The total travel of a switch is the distance between the key's resting position, and its position when fully depressed, i.e. how far down you can press the key.</p>
          </div>
        </div>

        <div class="flex flex-wrap -mx-3 mb-6">
          <div class="w-full mb-4 mx-3 border-b-2 block text-gray-500 font-bold">Force</div>
          <div class="w-full md:w-1/2 px-3 mb-6 md:mb-0">
            <label
              class="block uppercase tracking-wide text-gray-700 text-xs font-bold mb-2"
              for="grid-force-actuation"
            >Actuation (gf)</label>
            <input
              class="appearance-none block w-full py-3 px-4 mb-3 bg-gray-200 text-gray-700 border rounded leading-tight focus:outline-none focus:bg-white"
              id="grid-force-actuation"
              type="number"
            />
            <p
              class="text-gray-600 text-xs italic"
            >In gf (Gram-force), without tolerance. The force required to actuate the switch, i.e. to cause it to register a key press.</p>
          </div>
          <div class="w-full md:w-1/2 px-3">
            <label
              class="block uppercase tracking-wide text-gray-700 text-xs font-bold mb-2"
              for="grid-force-peak"
            >Peak (gf)</label>
            <input
              class="appearance-none block w-full py-3 px-4 mb-3 bg-gray-200 text-gray-700 border rounded leading-tight focus:outline-none focus:bg-white"
              id="grid-travel-peak"
              type="number"
            />
            <p
              class="text-gray-600 text-xs italic"
            >In gf (Gram-force), without tolerance. The highest force encountered in the travel of the switch, before the switch bottoms out.</p>
          </div>
        </div>

        <div class="flex flex-wrap -mx-3 mb-6">
          <div class="w-full px-3">
            <label
              class="block uppercase tracking-wide text-gray-700 text-xs font-bold mb-2"
              for="grid-led-style"
            >Image URL</label>
            <input
              class="appearance-none block w-full bg-gray-200 text-gray-700 border border-gray-200 rounded py-3 px-4 mb-3 leading-tight focus:outline-none focus:bg-white focus:border-gray-500"
              id="grid-led-style"
              type="url"
            />
          </div>
        </div>

        <div class="flex flex-wrap -mx-3 mb-6">
          <div class="w-full px-3">
            <label
              class="block uppercase tracking-wide text-gray-700 text-xs font-bold mb-2"
              for="grid-led-style"
            >Datasheet URL</label>
            <input
              class="appearance-none block w-full bg-gray-200 text-gray-700 border border-gray-200 rounded py-3 px-4 mb-3 leading-tight focus:outline-none focus:bg-white focus:border-gray-500"
              id="grid-led-style"
              type="url"
            />
          </div>
        </div>

        <div class="flex flex-wrap -mx-3 mb-6">
          <div class="w-full px-3">
            <label
              class="block uppercase tracking-wide text-gray-700 text-xs font-bold mb-2"
              for="grid-led-style"
            >Notes</label>
            <textarea
              class="appearance-none block w-full bg-gray-200 text-gray-700 border border-gray-200 rounded py-3 px-4 mb-3 leading-tight focus:outline-none focus:bg-white focus:border-gray-500"
              id="grid-led-style"
              type="url"
            />
          </div>
        </div>

        <div class="flex flex-wrap -mx-3 mb-6">
          <div class="w-full px-3">
            <button
              class="w-full py-2 px-4 bg-blue-500 hover:bg-blue-700 text-white font-bold rounded focus:outline-none focus:shadow-outline"
              type="submit"
            >Send</button>
          </div>
        </div>
      </form>

      <div>
        <ClientOnly>
          <vuetable
            ref="vuetable"
            :api-mode="false"
            :fields="fields"
            :per-page="perPage"
            :data-manager="dataManager"
            pagination-path="pagination"
            :detail-row-component="detailRow"
            :css="css.table"
            @vuetable:row-clicked="toggleDetailRow($event)"
          ></vuetable>
        </ClientOnly>
      </div>
    </div>
  </Layout>
</template>

<page-query>

</page-query>

<script>
import _ from "lodash";
import axios from "axios";
import Vuetable from "vuetable-2";
import SwitchDetailRow from "~/components/SwitchDetailRow.vue";

export default {
  metaInfo: {
    title: "Mechanical Keyboard Switch Database"
  },
  components: {
    Vuetable
  },
  data() {
    return {
      perPage: 3,
      data: [],
      detailRow: SwitchDetailRow,
      fields: [
        { name: "id", visible: false },
        { name: "brand", sortField: "brand", titleClass: "text-left" },
        { name: "model", sortField: "model", titleClass: "text-left" },
        { name: "action", titleClass: "text-left" },
        {
          name: "keycap_mount",
          title: "Keycap Mount",
          titleClass: "text-left"
        },
        {
          name: "switch_mount",
          title: "Switch Mount",
          titleClass: "text-left"
        },
        {
          name: "force.actuation",
          sortField: "force.actuation",
          dataClass: "text-center",
          formatter: value => `${value} gf`
        },
        {
          name: "force.peak",
          sortField: "force.peak",
          dataClass: "text-center",
          formatter: value => `${value} gf`
        }
      ],
      sortOrder: [
        {
          field: "brand",
          direction: "asc"
        }
      ],
      css: {
        table: {
          tableBodyClass: "block overflow-x-auto w-full"
        }
      }
    };
  },
  watch: {
    data(newVal, oldVal) {
      this.$refs.vuetable.refresh();
    }
  },
  mounted: function() {
    axios
      .get(
        "https://benroe.github.io/switch-database/mechanical-keyboard-switches.json"
      )
      .then(response => (this.data = response.data));
  },
  methods: {
    toggleDetailRow(event) {
      this.$refs.vuetable.toggleDetailRow(event.data.id);
    },
    dataManager(sortOrder, pagination) {
      if (this.data.length < 1) return;

      let local = this.data;

      // sortOrder can be empty, so we have to check for that as well
      if (sortOrder.length > 0) {
        // console.log("orderBy:", sortOrder[0].sortField, sortOrder[0].direction);
        local = _.orderBy(
          local,
          sortOrder[0].sortField,
          sortOrder[0].direction
        );
      }

      pagination = this.$refs.vuetable.makePagination(
        local.length,
        this.perPage
      );
      // console.log('pagination:', pagination)
      let from = pagination.from - 1;
      let to = from + this.perPage;

      return {
        pagination: pagination,
        data: _.slice(local, from, to)
      };
    }
  }
};
</script>

