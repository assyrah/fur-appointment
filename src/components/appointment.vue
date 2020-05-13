<template>
    <b-container id="app-appointment" class="appointment-container d-flex" fluid>
        <b-container>
            <b-row class="mt-5" align-h="center">
                <b-col cols="12" lg="8">
                    <h4>Make an Appointment</h4>
                    <p class="content">Time is gold! Make appointment to prevent disappointment!
                    </p>
                    <b-form class="mb-3" inline>
                        <b-input
                            id="inline-form-input-name"
                            class="mb-2 mr-sm-2 mb-sm-0"
                            placeholder="Date & Time"
                            ></b-input>
                        <b-form-select
                        id="inline-form-custom-select-pref"
                        class="mb-2 mr-sm-2 mb-sm-0"
                        :options="[{ text: 'Choose...', value: null }, 'One', 'Two', 'Three']"
                        :value="null"
                        ></b-form-select>
                        <b-form-select
                        id="inline-form-custom-select-pref"
                        class="mb-2 mr-sm-2 mb-sm-0"
                        :options="[{ text: 'Choose...', value: null }, 'One', 'Two', 'Three']"
                        :value="null"
                        ></b-form-select>
                    </b-form>
                    
                    <a class="button" href="#app-appointment">MAKE APPOINTMENT NOW</a>
                </b-col>
            </b-row>
        </b-container>
    </b-container>
</template>

<script>
    export default {
        data: function() {
            return {
                selectedBranch: [''],
                BranchA: ['Branch A','Branch A1'],
                BranchB: ['Branch B','Branch B1', 'Branch B2', 'Branch B3'],
                BranchC: ['Branch C'],
                BranchD: ['Branch D','Branch D1', 'Branch D2', 'Branch D3']
            }
        },
        computed: {
            
        }
    }
</script>

<style lang=scss scoped>
    .appointment-container {
        background-image: url("./../assets/bg_appointment.jpg");
        background-size: cover;
        min-height: 48rem;
    }
    .content {
        color: $orange-light;
        font-size: $font-size-lg;
    }
</style>