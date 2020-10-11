<template>
    <!DOCTYPE html>
    <html>

    <head>
        <meta charset="utf-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0, shrink-to-fit=no">
        <title>Untitled</title>
        <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/twitter-bootstrap/4.5.2/css/bootstrap.min.css">
        <link rel="stylesheet" href="assets/css/styles.css">
    </head>

    <body>
    <div data-bs-parallax-bg="true" style="height: 243px;background-image: url(&quot;http://lh3.googleusercontent.com/wbNRV8hJiAU1W7Mkok8RZKYQV4hzXiJPBqK5TyzJKiC2FKp0tX1De4rOWrptf7-Dh0bHohjpdk9l8Jt4yhYQJQ=w0&quot;);background-position: center;background-size: cover;width: 1161px;margin: 3px;"><img style="background-image: url(&quot;https://storage.googleapis.com/djfiles/google_developers_logo.png&quot;);width: 374px;margin: 27px;"></div>
    <div>
        <div class="container">
            <div class="row">
                <div class="col-md-6 d-table">
                    <p style="font-size: 20px;"><strong>Hello Developers in Sri Lanka</strong></p>
                    <p>Welcome to #CloudKasthiram.</p>
                    <p>Cloud Kasthiram is a Google Cloud Platform based challenge which you can participate and test your cloud knowledge</p>
                    <p>In Season 1 you get an opportunity to self study Google Cloud Platform starting with one month free access to Qwiklabs and receive a cool swag pack upon completion. Sounds interesting? Follow the steps below.<br>&nbsp;<br></p>
                </div>

                <div class="col-md-6">
                    <p style="font-size: 20px;"><strong>Why should you be a part of #CloudKasthiram?</strong></p>
                    <p>You get to learn about the Google Cloud Platform and its operation from ground up. Then you can test your skills with the Qwiklabs platform.
                    You also get 1 month free access to Qwiklabs so that you can continue to do labs and learn even more...</p>
                    <p>Complete the quests within the given time period and win cool rewards.</p>


                    Spread the word by sharing this link: gdgsrilanka.org/cloudkasthiram and use&nbsp;<strong>#CloudKasthiram</strong>&nbsp;on
                    social media. Follow&nbsp;<a href="https://twitter.com/GDGLK">@gdglk</a>&nbsp;for all updates!
                    <p>&nbsp;Let's dance the #CloudKasthiram</p>
                </div>
            </div>
            <div class="row">
                <div class="col-md-12">
                    <p style="font-size: 20px;"><strong>This is how you do it...</strong></p>
                    <v-stepper v-model="e1">
                        <v-stepper-header>
                            <v-stepper-step
                                    :complete="e1 > 1"
                                    step="1"
                            >
                                Register
                            </v-stepper-step>

                            <v-divider></v-divider>

                            <v-stepper-step
                                    :complete="e1 > 2"
                                    step="2"
                            >
                                Do the labs
                            </v-stepper-step>

                            <v-divider></v-divider>

                            <v-stepper-step step="3">
                                Dance the Kasthiram, and claim the swags
                            </v-stepper-step>
                        </v-stepper-header>

                        <v-stepper-items>
                            <v-stepper-content step="1">
                                <v-card
                                        class="mb-12"

                                        height="200px"
                                >
                                    <p>In order to participate in the #CloudKasthiram challenge, you must first register.</p>
                                    <p><button class="btn btn-primary" onClick="location.href='http://bit.ly/cloud-registration'" type="button">REGISTER NOW</button></p>
                                    <p>Want to know how to get one month Qwiklab access? Check out this video&nbsp;<a href="https://youtu.be/R3_A4gFHT2A">tutorial</a></p>
                                </v-card>

                                <v-btn
                                        color="success"
                                        @click="e1 = 2"
                                >
                                    Done! I Registered
                                </v-btn>

                            </v-stepper-content>

                            <v-stepper-content step="2">
                                <v-card
                                        class="mb-12"
                                >
                                    <h4>Great.! Now all you have to do, is complete six quests. </h4>
                                    <p>Here's a list of qwiklabs which you can do.</p>
                                    <h5 class="text-left">Fundamental Quests</h5>
                                    <p class="text-left">
                                        <a href="https://google.qwiklabs.com/quests/120">Getting Started: Create and Manage Cloud Resources</a><br>
                                        <a href="https://www.qwiklabs.com/quests/90">Understanding Your Google Cloud Costs</a><br>
                                        <a href="https://google.qwiklabs.com/quests/118">Perform Foundational Infrastructure Tasks in Google Cloud</a><br>
                                        <a href="https://google.qwiklabs.com/quests/121">Deploy and Manage Cloud Environments with Google Cloud</a><br>
                                        <a href="https://google.qwiklabs.com/quests/128?">Build and Secure Networks in Google Cloud</a><br>
                                        <a href="https://www.qwiklabs.com/quests/143">Monitor and Log with Google Cloud Operations Suite</a><br>
                                        <a href="https://google.qwiklabs.com/quests/115">Build a Website on Google Cloud</a><br>
                                        <a href="https://google.qwiklabs.com/quests/141">Implement DevOps in Google Cloud</a><br>
                                        <a href="https://google.qwiklabs.com/quests/116?">Deploy to Kubernetes in Google Cloud</a><br>
                                        <a href="https://google.qwiklabs.com/quests/142?">Secure Workloads in Google Kubernetes Engine</a><br>
                                        <a href="https://www.qwiklabs.com/quests/32">Intro to ML: Image Processing</a>
                                    </p>
                                    <h5 class="text-left">Machine Learning</h5>
                                    <p class="text-left">
                                        <a href="https://www.qwiklabs.com/quests/85">Intro to ML: Image Processing</a><br>
                                        <a href="https://www.qwiklabs.com/quests/82">Intro to ML: Language Processing</a><br>
                                        <a href="https://www.qwiklabs.com/quests/83">Intermediate ML: TensorFlow on GCP</a><br>
                                        <a href="https://www.qwiklabs.com/quests/38">Google Cloud Solutions II: Data and Machine Learning</a><br>
                                        <a href="https://www.qwiklabs.com/quests/126">Explore Machine Learning Models with Explainable AI</a><br>
                                        <a href="https://www.qwiklabs.com/quests/84">Advanced ML: ML Infrastructure</a><br>
                                        <a href="https://www.qwiklabs.com/quests/71">BigQuery for Machine Learning</a><br>
                                        <a href="https://www.qwiklabs.com/quests/136">Integrate with Machine Learning APIs</a><br><br>
                                    </p>
                                </v-card>

                                <v-btn
                                        color="success"
                                        @click="e1 = 3"
                                >
                                    I did the labs too.!
                                </v-btn>

                                <v-btn
                                        @click="e1 = 1"
                                        text>
                                    Back
                                </v-btn>
                            </v-stepper-content>

                            <v-stepper-content step="3">
                                <v-card
                                        class="mb-12"
                                >
                                    <h5>Congratulations! You've danced the dance. Now you can claim the reward.</h5>
                                    <p>Go to your Qwiklabs profile page, and submit that link to the form below</p>
                                    <p>For the completion of the five labs <b>before 20th November 2020</b>, you are eligible for</p>
                                    <ul>
                                        <li>T-Shirt</li>
                                        <li>Cap</li>
                                        <li>Google sticker card</li>
                                    </ul>
                                    <button class="btn btn-primary" onClick="location.href='http://bit.ly/lab-completed'" type="button">CLAIM MY REWARD</button>
                                 </br>
                                </v-card>
                                <v-btn
                                        @click="e1 = 2"
                                        text>
                                    Back
                                </v-btn>
                            </v-stepper-content>
                        </v-stepper-items>
                    </v-stepper>
                </div>
            </div>
        </div>
    </div>
    </body>

    </html>

</template>
<script>
  export default {
    data () {
      return {
        e1: 1,
      }
    },
  }
</script>
