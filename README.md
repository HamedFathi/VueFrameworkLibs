![Vue Logo](https://i.ibb.co/dKxqx0m/logo.png)

# Vue 3

The Progressive JavaScript Framework.

---
### Framework

[Vue 3](https://v3.vuejs.org/)

[JSX for Vue 3](https://github.com/vuejs/jsx-next)

---
### Compiler

[Vue Template Compiler](https://www.npmjs.com/package/vue-template-compiler)

[Vue Component Compiler](https://github.com/vuejs/vue-component-compiler)

[Vue Component Compiler Utils](https://github.com/vuejs/component-compiler-utils)

[Vue Loader](https://vue-loader.vuejs.org/)

---
### Router

[Vue Router 4](https://next.router.vuejs.org/)

---
### State Management

[Vuex 4](https://next.vuex.vuejs.org/)

[Vuex Persistedstate](https://github.com/robinvdvleuten/vuex-persistedstate)

[Vuex Pathify](https://github.com/davestewart/vuex-pathify)

[Pinia](https://github.com/posva/pinia)

---
### Scaffolding

[Vue CLI](https://cli.vuejs.org/)

[Vue CLI Plugin for Vuetify](https://github.com/vuetifyjs/vue-cli-plugins)

[Vue CLI Plugin for Apollo](https://github.com/Akryum/vue-cli-plugin-apollo)

[Vue CLI Plugin SSR](https://github.com/Akryum/vue-cli-plugin-ssr)

[Create Nuxt App](https://github.com/nuxt/create-nuxt-app)

---
### SSR

[Nuxt.js](https://nuxtjs.org/) with [Nuxt Composition API](https://composition-api.nuxtjs.org/)

---
### Testing

[Vue Test Utils 2](https://vuejs.github.io/vue-test-utils-next-docs)

[Vuex Mock Store](https://github.com/posva/vuex-mock-store)

[Vue Router Mock](https://github.com/posva/vue-router-mock)

---
### E2E Testing

[Cypress Vue](https://github.com/cypress-io/cypress/tree/master/npm/vue)

---
### Build Tool

[Vite](https://github.com/vitejs/vite)

---
### Dev Tools

[Vue DevTools](https://github.com/vuejs/vue-devtools)

---
### Static Site Generator

[VuePress 2](https://github.com/vuepress/vuepress-next)

[VitePress](https://vitepress.vuejs.org/)

[Gridsome](https://gridsome.org/)

---
### User Interface

[Vuetify](https://vuetifyjs.com/en/)

[BootstrapVue](https://bootstrap-vue.org/)

[Quasar](https://quasar.dev/)

[Element](https://element.eleme.io/)

[Vuesax](https://vuesax.com/)

[Ant Design Vue](https://www.antdv.com/)

[PrimeVue](https://www.primefaces.org/primevue/)

[VueTailwind](https://www.vue-tailwind.com/)

---
### Visual Studio Code

[Vetur](https://github.com/vuejs/vetur)

---
### Mobile

[NativeScript Vue](https://github.com/rigor789/nativescript-vue-next)

[Ionic Vue](https://ionicframework.com/docs/vue/overview)

[Framework7 Vue](https://framework7.io/vue/)

---
### HTTP

[Vue-Axios](https://github.com/imcvampire/vue-axios)

* [Axios](https://github.com/axios/axios)

* [Axios Retry](https://github.com/softonic/axios-retry)

* [Axios Mock Adapter](https://github.com/ctimmerm/axios-mock-adapter)

* [Axios Cache Adapter](https://github.com/RasCarlito/axios-cache-adapter)

* [Axios Logger](https://github.com/hg-pyun/axios-logger)

* [Axios Extensions](https://github.com/kuitos/axios-extensions)

* [Axios Debug Log](https://github.com/Gerhut/axios-debug-log)

* [Mocha Axios](https://github.com/jdrydn/mocha-axios)

* [Jest Mock Axios](https://github.com/knee-cola/jest-mock-axios)

---
### Validation

[Vuelidate 2](https://vuelidate.js.org/) with [vNext Doc](https://vuelidate-next.netlify.app) - Recommended

[VeeValidate 4](https://vee-validate.logaretm.com/v4/)

---
### Authentication 

[Vue Auth 4](https://websanova.com/docs/vue-auth/home)

---
### Internationalization

[Vue I18n 9](https://github.com/intlify/vue-i18n-next) with [vNext Doc](https://vue-i18n-next.intlify.dev/)

---
### GraphQL 

[Vue Apollo 4](https://v4.apollo.vuejs.org/)

---
### SEO 

[Vue Meta 3](https://vue-meta.nuxtjs.org/)

---
### Documentation Generator

[Vue Styleguidist](https://vue-styleguidist.github.io/)

---
### Firebase

[Vuefire](https://vuefire.vuejs.org/)

---
### Miscellaneous

[Vue Rx](https://github.com/NOPR9D/vue-next-rx)

[VuePromised](https://github.com/posva/vue-promised)

[Vue Local Scope](https://github.com/posva/vue-local-scope)

[Vue 3 Logger](https://github.com/MarcSchaetz/vuejs3-logger)

---
### Vuetify Supplements

The following completes the Vuetify components.

[Snackbar Queue](https://github.com/ajanes93/vuetify-snackbar-queue)

[Vuetify Confirm Dialog](https://github.com/yariksav/vuetify-confirm)

[Vuetify Dialog Service](https://github.com/yariksav/vuetify-dialog)

[Vuetify Currency Field](https://github.com/phiny1/v-currency-field)

**PopOver**

```html
<div id="app">
  <v-app id="inspire">
    <v-menu offset-y :close-on-content-click="false">
      <v-btn primary dark slot="activator">Dropdown</v-btn>
      <v-card>
        <v-card-text>
          <p>Blah blupp <v-btn>Foobar</v-btn></p>
          <v-text-field label="Enter some text"></v-text-field>
        </v-card-text>
      </v-card>
    </v-menu>
  </v-app>
</div>
```

```js
new Vue({
  el: '#app'
})
```

**Discovery**

```html
<div id="app">
  <v-app id="inspire">
    <v-container fluid grid-list-xl>
      <v-layout wrap align-center>
        <v-btn color="primary" @click="discover = !discover">Discover</v-btn>
        <feature-discovery v-model="discover" color="primary" right bottom size="400" class="white--text">
          <h2 slot="title">Hey! New feature...</h2>
          <p slot="text" class="mb-0">
            There's all sorts of new things that you can do with the great new features. Just click the buttons to check them out!
          </p>
          <div slot="actions">
            <v-btn color="white" depressed>Action</v-btn>
            <v-btn outline color="white" @click="discover = false">Lesser action</v-btn>
          </div>
        </feature-discovery>
      </v-layout>
    </v-container>
  </v-app>
</div>

<script type="text/x-template" id="featureDiscovery">
	<div class="featureDiscovery" :class="[positionClass, color, {'animateIn': value}]" :style="{width: `${size}px`, height: `${size}px`}">
    <v-layout row wrap :class="`justify-${left ? 'start' : 'end'} align-${top ? 'baseline' : 'end'}`" fill-height>
      <v-flex fill-height :style="{maxWidth: `${size - (size * 0.15)}px`, maxHeight: `${size - (size * 0.2)}px`}">

        <v-layout column fill-height class="pa-2">
          <v-flex d-flex text-xs-center :class="`${left && !top ? 'mr-4' : !left && !top ? 'ml-4 mt-3' : ''} align-${top ? 'baseline' : 'end'}`">
            <slot name="title"></slot>
          </v-flex>
          <v-flex d-flex text-xs-center align-center>
            <slot name="text"></slot>
          </v-flex>
          <v-flex d-flex text-xs-center :class="`${left && top ? 'mr-4' : !left && top ? 'ml-4' : ''}`" align-baseline>
            <slot name="actions"></slot>
          </v-flex>
        </v-layout>

      </v-flex>
    </v-layout>
  </div>
</script>
```

```css
.featureDiscoveryTitle {
  margin-top: 30%;
  padding-left: 30%;
}
.featureDiscoveryContainer {
  padding: 20px;
  width: fit-content;
}
.animateIn {
  transform: translate3d(0, 0, 0)!important;
}
.featureDiscovery {
  overflow: hidden;
  transition: 300ms cubic-bezier(0.16, 0.61, 0.5, 1);
  position: fixed;
  height: 400px;
  width: 400px;
  z-index: 10;
}
.featureDiscoverybottomright {
  transform: translate3d(100%, 100%, 0);
  border-radius: 100% 0 0 0;
  bottom: 0;
  right: 0;
}
.featureDiscoverybottomleft {
  transform: translate3d(-100%, 100%, 0);
  border-radius: 0 100% 0 0;
  bottom: 0;
  left: 0;
}
.featureDiscoverytopright {
  transform: translate3d(100%, -100%, 0);
  border-radius: 0 0 0 100%;
  top: 0;
  right: 0;
}
.featureDiscoverytopleft {
  transform: translate3d(-100%, -100%, 0);
  border-radius: 0 0 100% 0;
  top: 0;
  left: 0;
}
```

```js
const featureDiscovery = {
  template: '#featureDiscovery',
  props: {
    value: {
      type: Boolean,
      default: false
    },
    top: {
      type: Boolean,
      default: false
    },
    bottom: {
      type: Boolean,
      default: false
    },
    right: {
      type: Boolean,
      default: false
    },
    left: {
      type: Boolean,
      default: false
    },
    size: {
      default: 400
    },
    color: {
      type: String,
      default: 'primary'
    }
  },
  model: {
    prop: 'value',
    event: 'update'
  },
  data () {
    return {
      animateIn: false
    }
  },
  computed: {
    positionClass () {
      let {top, left} = this
      let y = top ? 'top' : 'bottom'
      let x = left ? 'left' : 'right'
      return `featureDiscovery${y}${x}`
    }
  }
}

new Vue({
  el: '#app',
  components: {featureDiscovery},
  data: () => ({
    discover: false
  })
})
```

**Nested Expansion Panel**

```html
<div id="app">
  <v-app>
    <v-content>
      <v-container grid-list-xl>
        <v-switch label="Nested Panels - Accordion" v-model="accordion"></v-switch>
        <v-expansion-panels>
          <v-expansion-panel>
            <v-expansion-panel-header>Panel 1</v-expansion-panel-header>
            <v-expansion-panel-content>Panel 1 content</v-expansion-panel-content>
          </v-expansion-panel>
          <v-expansion-panel>
            <v-expansion-panel-header>Panel 2</v-expansion-panel-header>
            <v-expansion-panel-content>
              <p>This panel has a nested expansion panel.</p>
              <v-expansion-panels :accordion="accordion">
                <v-expansion-panel>
                  <v-expansion-panel-header>Nested Panel 1</v-expansion-panel-header>
                  <v-expansion-panel-content>Nested Panel 1 content.</v-expansion-panel-content>
                </v-expansion-panel>
                <v-expansion-panel>
                  <v-expansion-panel-header>Nested Panel 2</v-expansion-panel-header>
                  <v-expansion-panel-content>Nested Panel 2 content.</v-expansion-panel-content>
                </v-expansion-panel>
              </v-expansion-panels>
            </v-expansion-panel-content>
          </v-expansion-panel>
        </v-expansion-panels>
      </v-container>
    </v-content>
  </v-app>
</div>
```
```js
new Vue({
  el: '#app',
  vuetify: new Vuetify(),
  data: () => ({
    accordion: false
  })
})
```

**Expandable List**

```html
<div id="app">
  <v-app id="inspire">
    <v-layout row>
      <v-flex mt-3 xs12 sm6 offset-sm3>
        <v-card>
          <v-toolbar color="teal" dark>
            <v-toolbar-side-icon></v-toolbar-side-icon>
            <v-toolbar-title>Topic: {{ selected }}</v-toolbar-title>
            <v-spacer></v-spacer>
            <v-btn icon>
              <v-icon>more_vert</v-icon>
            </v-btn>
          </v-toolbar>
          <v-list>
            <v-list-group
              v-for="item in items"
              v-model="item.active"
              :key="item.title"
              :prepend-icon="item.action"
              no-action
              @input="onItemClick($event, item.title)"
            >
              <v-list-tile slot="activator">
                <v-list-tile-content>
                  <v-list-tile-title>{{ item.title }}</v-list-tile-title>
                </v-list-tile-content>
              </v-list-tile>
              <v-list-tile v-for="subItem in item.items" :key="subItem.title" @click="">
                <v-list-tile-content>
                  <v-list-tile-title>{{ subItem.title }}</v-list-tile-title>
                </v-list-tile-content>
                <v-list-tile-action>
                  <v-icon>{{ subItem.action }}</v-icon>
                </v-list-tile-action>
              </v-list-tile>
            </v-list-group>
          </v-list>
        </v-card>
      </v-flex>
    </v-layout>
  </v-app>
</div>
```
```js
new Vue({
  el: '#app',
  methods: {
    onItemClick(event, item) {
      if(event) {
        this.selected = item
      }
    }
  },
  data () {
    return {
      selected: '',
      items: [
        {
          action: 'local_activity',
          title: 'Attractions',
          items: [
            { title: 'List Item' }
          ]
        },
        {
          action: 'restaurant',
          title: 'Dining',
          active: true,
          items: [
            { title: 'Breakfast & brunch' },
            { title: 'New American' },
            { title: 'Sushi' }
          ]
        },
        {
          action: 'school',
          title: 'Education',
          items: [
            { title: 'List Item' }
          ]
        },
        {
          action: 'directions_run',
          title: 'Family',
          items: [
            { title: 'List Item' }
          ]
        },
        {
          action: 'healing',
          title: 'Health',
          items: [
            { title: 'List Item' }
          ]
        },
        {
          action: 'content_cut',
          title: 'Office',
          items: [
            { title: 'List Item' }
          ]
        },
        {
          action: 'local_offer',
          title: 'Promotions',
          items: [
            { title: 'List Item' }
          ]
        }
      ]
    }
  }
})
```
