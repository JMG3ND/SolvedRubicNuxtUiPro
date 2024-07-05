<template>
  <div>
    <div class="hpf">
      <div class="hpf__container">
        <div class="hpf__form">
          <div class="hpf__background-rotate">
            <AssetsCubeCard />
          </div>
          <div class="hpf__title">
            <UColorModeImage
              alt="Título Solved Rubik"
              dark="/images/logo-solvedrubik-hom-page-presentation-dark-640.png"
              light="/images/logo-solvedrubik-hom-page-presentation-light-640.png"
            />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
//hpf (home-page-finder)
.hpf {
  box-shadow: 2px;

  &__form {
    position: relative;
    display: flex;
    flex-direction: column;
    width: 100%;
    height: 100%;
    justify-content: space-evenly;
    gap: 20px;
    padding: 1rem;
    align-items: center;
  }

  &__title {
    width: 640px;
    max-width: 100%;
    z-index: 1;
  }

  &__background-rotate {
    width: 30%;
    max-width: 200px;
    aspect-ratio: 1/1;
    position: absolute;
    top: 10%;
    left: 50%;
    animation: infiniterotation 60s infinite cubic-bezier(0.45, 0.43, 1, 1);

    @keyframes infiniterotation {
      from {
        transform: rotate(0);
      }

      to {
        transform: rotate(360deg);
      }
    }
  }
}
</style>
