<template>
  <f7-views>
    <f7-view>
      <f7-pages>
        <f7-page>
          <f7-navbar type="fixed">
            <a class="link" slot="left" v-link="'/'">
              <f7-icon class="icon-back"></f7-icon>
            </a>
            <span slot="center">Picker Modal</span>
          </f7-navbar>
          <f7-page-content>
            <f7-content-block>
              <a target="_blank"
                 href="https://github.com/lmk123/vue-framework7/blob/master/dev-website/pages/picker.vue">Code
                is
                here.</a>
            </f7-content-block>
            <f7-picker-modal v-ref:picker>
              <f7-picker-modal-inner>
                <f7-content-block>
                  Hi.
                </f7-content-block>
              </f7-picker-modal-inner>
            </f7-picker-modal>

            <f7-content-block title="normal row">
              <p>
                <f7-button @click="$refs.picker.show">Show Picker</f7-button>
              </p>
              <f7-button @click="$refs.picker.hide">Hide Picker</f7-button>
            </f7-content-block>
          </f7-page-content>
        </f7-page>
      </f7-pages>
    </f7-view>
  </f7-views>
</template>
