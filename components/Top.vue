<template>
  <header>
    <img src="~/assets/image/logo.svg" class="top-logo">
    <div class="header-right">
      <a href="#about" class="header-right__about">
        About
      </a>
      <a href="#bicycle" class="header-right__bicycle">
        Bicycle
      </a>
    </div>
  </header>
</template>

<style lang="scss" scoped>
header{
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: space-between;
}
.top-logo{
  width: 120px;
  height: 40px;
  padding: 10px 0 10px 230px;
  @media screen and (max-width: 599px) {  
    padding-left: 10px;
  }
}

.header-right{
  display: flex;
  flex-direction: row;
  padding: 0 230px 0 0;
  text-align: left;
  font: normal normal normal 14px/21px Meiryo;
  letter-spacing: 0px;
  color: #24292E;
  opacity: 1;
  cursor: pointer;
  :hover{
    opacity: 0.5;
  }
  @media screen and (max-width: 599px) {
    padding: 0 10px 0 0;
  }
  &__about{
    padding-right: 30px;
    text-decoration: none;
    color: #24292E;
  }
  &__bicycle{
    text-decoration: none;
    color: #24292E;
  }
}
</style>