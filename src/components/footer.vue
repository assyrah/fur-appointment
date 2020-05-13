<template>
    <b-container id="app-footer" class="footer-container" fluid>
      <b-container class="container pt-5 pb-5">
        <b-row align-h="center">
            <b-col cols="12" lg="6">
                <h4>Extra hands?</h4>
                <p class="content">YES please! Be a volunteer today:
                </p>
            </b-col>
            <b-col cols="12" lg="6">
                <b-form inline>
                  <b-input
                    id="inline-form-input-name"
                    class="mb-2 mr-sm-2 mb-sm-0"
                    placeholder="Date & Time"
                    ></b-input>
                  <b-button class="button" variant="primary">Save</b-button>
                </b-form>
            </b-col>
        </b-row>
        <b-row align-h="between" class="disclaimer pt-3">
          <b-col cols="12" lg="8">
            <p><small>&copy; 2019 THE CATASTROPHE</small></p>
          </b-col>
          <b-col cols="12" lg="4">
            <b-nav>
              <b-nav-item right>FAQS</b-nav-item>
              <b-nav-item right>PRIVACY POLICY</b-nav-item>
              <b-nav-item right>LEGAL NOTICES</b-nav-item>
            </b-nav>
          </b-col>
        </b-row>
      </b-container>
    </b-container>
</template>

<script>
    export default {
        
    }
</script>

<style lang=scss scoped>
    .footer-container {
      background-color: $dark-blue;
    }
    .content {
        font-size: $font-size-lg;
        color: $orange;
    }
    .disclaimer {
      border-top: 2px solid $blue;
      color: $blue;
    }
</style>