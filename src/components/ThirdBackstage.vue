<template>
   
    <div class="img-container" :class="{'parent': true, 'hovered': isHovered}">
        <div class="cover-img" @mouseover="isHovered = true" @mouseleave="isHovered = false" >
            <img src="../assets/backstagetalks_cover_issue_6.png" alt="img" height="500px" width="400px">
        </div>
    </div>
</template>

<script>
   export default {
  data() {
    return {
      isHovered: false
    };
  }
};
</script>

<style scoped>
.img-container {
    display: grid;
    place-items: center;
    height: 100vh;
    background-color: white;
    transition: background-color 0.3s ease;
}

.img-container.hovered {
    background-color: #FFF;
}

</style>