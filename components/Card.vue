<template>
    <div class="card" style="width: 18rem;">
        <div class="card-body">
            <h5 class="card-title">{{projectTitle}}</h5>
            <h6 class="card-subtitle mb-2 text-muted">{{ projectSubtitle}}</h6>
            <p class="card-text">{{projetDescription}}</p>
            <a v-bind:href="projectLink" target="_blank" class="card-link">GIT project link</a>
        </div>
    </div>
</template>

<script>
export default {
    props: ["projectTitle","projectSubtitle","projetDescription","projectLink"]
}
</script>