<template>
    <v-container class="pa-0">
        <v-layout wrap align-center justify-center row fill-height >
           <v-flex xs12 md3 lg3 class="pa-2">
               <p class="google-font" style="font-size:180%">What we do?</p>
               <p class="google-font" style="font-size:110%">Google Developer Groups (GDGs) are for developers who are interested in Google's developer technology.</p>

               <p class="google-font" style="font-size:110%">About different Google technologies</p>

                <span v-for="(item,i) in whatWeDoData" :key="i">
                    <v-tooltip bottom>
                        <template v-slot:activator="{ on }" >
                            <a :href="item.link" target="_blank" flat class="ma-0">
                                <img :src="getImgUrl(item.image)" width="30vh" alt="" srcset="" dark v-on="on">
                            </a> 
                            &nbsp;&nbsp;&nbsp;
                        </template>
                        <span>{{item.TechName}}</span>
                    </v-tooltip>
                </span>
                
                <br><br>

            </v-flex> 
            <v-flex xs12 md9 lg9 class="">
                <v-layout row wrap>

                    <v-flex xs6 sm6 md3 lg3 class="text-xs-center pa-2">
                        <v-icon large style="font-size:300%">chat_bubble</v-icon>
                        <p class="google-font" style="font-size:130%">Talks</p>
                        <p class="google-font" style="font-size:110%">Get updated with the latest news and announcements</p>
                    </v-flex>

                    <v-flex xs6 sm6 md3 lg3 class="text-xs-center pa-2">
                        <v-icon large style="font-size:300%">code</v-icon>
                        <p class="google-font" style="font-size:130%">Codelabs</p>
                        <p class="google-font" style="font-size:110%">Get hands-on experience and guidance from the community members</p>
                    </v-flex>

                    <v-flex xs6 sm6 md3 lg3 class="text-xs-center pa-2">
                        <v-icon large style="font-size:300%">school</v-icon>
                        <p class="google-font" style="font-size:130%">GDG at Campus</p>
                        <p class="google-font" style="font-size:110%">Share knowledge in your college or university with GDG</p>
                    </v-flex>

                    <v-flex xs6 sm6 md3 lg3 class="text-xs-center pa-2">
                        <v-icon large style="font-size:300%">airplay</v-icon>
                        <p class="google-font" style="font-size:130%">Live Viewing Parties</p>
                        <p class="google-font" style="font-size:110%">Get to know the latest technology as it is unveiled</p>
                    </v-flex>
                    <v-flex xs6 sm6 md3 lg3 class="text-xs-center pa-2">
                        <v-icon large style="font-size:300%">memory</v-icon>
                        <p class="google-font" style="font-size:130%">ML Boot Camps </p>
                        <p class="google-font" style="font-size:110%">Helping build a strong ML community in Sri Lanka</p>
                    </v-flex>
                    <v-flex xs6 sm6 md3 lg3 class="text-xs-center pa-2">
                        <v-icon large style="font-size:300%">book</v-icon>
                        <p class="google-font" style="font-size:130%">CodeLanka</p>
                        <p class="google-font" style="font-size:110%">Lets solve tech problems, one line at a time</p>
                    </v-flex>

                    <v-flex xs6 sm6 md3 lg3 class="text-xs-center pa-2">
                        <v-icon large style="font-size:300%">laptop</v-icon>
                        <p class="google-font" style="font-size:130%">Study Jams</p>
                        <p class="google-font" style="font-size:110%">Focusing on learning a new technology, together</p>
                    </v-flex>

                </v-layout>
            </v-flex>
        </v-layout>

    </v-container>
</template>

<script>
import whatWeDoData from '@/assets/data/whatWeDoComponentData.json'
import ChapterDetails from '@/assets/data/chapterDetails.json'
export default {
    data() {
        return {
            chapterDetails: ChapterDetails,
            whatWeDoData: whatWeDoData
        }
    },
    methods:{
        getImgUrl(url) {
            if(url.length>0){
                return require('@/assets/img/what-we-do/'+url)
            }else{
                return require('@/assets/img/what-we-do/notFound.png')
            }
        },
    }
}
</script>