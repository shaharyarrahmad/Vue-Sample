<template>
  <div>
<tabs :selected="selected" :curr="selectedTab"/>
<tabInfo :tabInfo="tabData[selectedTab-1]"  />
  </div>
</template>

<script>
import tabs from '../components/tabs.vue'
import tabInfo from '../components/tabInfo.vue'
export default {
  components: {
    tabs,
    tabInfo
  },
  data () {

    return {
      selectedTab: 1,
      tabData : [{

        header: '3 Easy Steps ',
        h2: 'To get Hired for your next job',
        labels: ['Create Your Resume', 'Apply with just one Click', 'Get Hired'],
        images: ['/1.1.png', '/1.2.png', '/1.3.png'],
      },
      {
        header: '3 Easy Steps to Hire Talent',
        h2: 'For empty seats in your company',
        labels: ['Create Company Profile', 'Create Job posting from Templetes', 'Hire Best Talent'],
        images: ['/1.1.png', '/2.2.png', '/2.3.png'],
      },
      {
        header: '3 Easy Steps',
        h2: 'For Remote Talent',
        labels: ['Create Your Profile', 'Apply for Remote Job Posting', 'Bet Paid by Hours or Fixed Salary'],
        images: ['/1.1.png', '/3.2.png', '/3.3.png'],
      }]
    }
  },

  methods: {
    selected (selectedTab) {
       this.selectedTab = selectedTab
    }
  },

}
</script>

<style>

</style>
