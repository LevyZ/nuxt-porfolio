<template>
  <section class="section is-medium">
    <div class="container has-text-centered">
      <h1 class="title">My Projects</h1>
      <div class="row" >
          <div v-for="(item, index) in allProjects" :key="index"
            class="col-4"
          >
            <card
              :projectTitle="item.title"
              :projectSubtitle="item.subtitle"
              :projetDescription="item.description"
              :projectLink="item.link"
            >
            </card>
          </div>
         
      </div>
    </div>
  </section>
</template>

<script>
  import Card from '../components/Card'

  export default {
    components: {
      Card
    },
    data () {
      return {
        allProjects: [
          {
            title: "Projet 1",
            subtitle: "Projet sous-titre",
            description: "Voici une rapide descrition du projet",
            link: "https://gitlab.com/levy225"
          },
          {
            title: "Projet 2",
            subtitle: "Projet sous-titre",
            description: "Voici une rapide descrition du projet",
            link: "https://gitlab.com/levy225"
          },
          {
            title: "Projet 3",
            subtitle: "Projet sous-titre",
            description: "Voici une rapide descrition du projet",
            link: "https://gitlab.com/levy225"
          },
        ]
      }
    }
  }
</script>