<template>
    <v-container>
        <v-flex>
            <v-layout wrap row center>
                <v-flex md12 >
                    <img class="banner-image" :src="require('@/assets/img/featureEvent/cropped_kast_header.png')" align="center"/>
                </v-flex>
            </v-layout>
            <v-layout>
                <v-flex md12 class="text-md-center">
                    <h2 class="focus-bold">#CloudKasthiram Qwiklabs Guide</h2>
                    <h3 class="focus-plain">How to get one month access to Qwiklabs</h3>
                </v-flex>
            </v-layout>
            <v-layout>
                <v-flex md8>
                    <p class="step-header">Step 1  - Register yourself at gdgsrilanka.org/cloudkasthiram</p>
                    <p class="step-content">
                        You may skip this step if you have already registered
                    </p>
                </v-flex>
            </v-layout>
            <v-layout>
                <v-flex md8>
                    <p class="step-header">Step 2 - Go to google.qwiklabs.com using an incognito window and click join.
                        Create an account.
                    </p>
                    <p class="step-content">
                        Once logged in you should see a screen as below. Word “Cloud” will be replaced by your login name
                        --- image here---

                    </p>
                </v-flex>
            </v-layout>

            <v-layout>
                <v-flex md8>
                    <p class="step-header">Step 3 - Go to the email you received upon registration,
                        click on the link in step 1 in the email.
                    </p>
                    <p class="step-content">
                        --- image here
                        Once clicked on the link you’ll be on the page below.
                        --- image here---

                    </p>
                </v-flex>
            </v-layout>

            <v-layout>
                <v-flex md8>
                    <p class="step-header">Step 4 - Click on “Enroll in the Quest”.</p>
                    <p class="step-content">
                        Once clicked on the link you’ll be on the page below.
                        --- image here
                        Once clicked on the link you’ll be on the page below.
                        --- image here---

                    </p>
                </v-flex>
            </v-layout>

        </v-flex>
    </v-container>


</template>

<script>
  export default {
    name: "HowToKasthiram"
  }
</script>

<style scoped>
    .focus-bold {
        font-weight: bold;
        text-align: center;
    }

    .focus-plain {
        text-align: center;
    }
</style>