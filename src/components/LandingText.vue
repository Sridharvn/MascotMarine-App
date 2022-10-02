<template>
  <div class="body">
    <p class="body__text">
      Melbourne-based Marine Consultancy Company, providing marine expertise to the
      shipping community. Independent surveys. Authorised surveyor for Honduran and
      Bolivian Flag vessels. Authorised PMDS surveyor for Geelong and Melbourne
      (Panamanian Maritime documentation services). Authorised Technical/Engineering
      surveyor for Intertek Australia.
    </p>
    <div class="body__card">
      <ul>
        <li>Independent surveys</li>
        <li>Authorised survyor for Honduran and Bolivian Flag vessels</li>
        <li>Authorised PMDS surveyor for Geelong and Melbourne</li>
        <li>Authorised Technical/Engineering surveyor for Intertek Australia</li>
      </ul>
    </div>
  </div>
</template>
<style lang="scss" scoped>
.body {
  display: flex;
  justify-content: center;
  flex-direction: column;
  &__text {
    width: 50vw;
    font-size: x-large;
    padding: 10px;
  }
  &__card {
    background-color: $secondary;
    font-size: x-large;
    border-radius: 10px;
    padding: 10px;
    margin: 10px;
    width: fit-content;
  }
}
</style>
