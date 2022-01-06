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

        header: 'Drei einfache Schritte',
        h2: 'zu deinem neuen Job',
        labels: ['Erstellen dein Lebenslauf', 'Erstellen dein Lebenslauf', 'Mit nur einem Klick bewerben'],
        images: ['/1.1.png', '/1.2.png', '/1.3.png'],
      },
      {
        header: 'Drei einfache Schritte',
        h2: 'zu deinem neuen Mitarbeiter',
        labels: ['Erstellen dein Unternehmensprofil', 'Erstellen ein Jobinserat', 'Wähle deinen neuen Mitarbeiter aus'],
        images: ['/1.1.png', '/2.2.png', '/2.3.png'],
      },
      {
        header: 'Drei einfache Schritte zur',
        h2: 'Vermittlung neuer Mitarbeiter',
        labels: ['Erstellen dein Unternehmensprofil', 'Erhalte Vermittlungs- angebot von Arbeitgeber', 'Vermittlung nach Provision oder Stundenlohn'],
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
