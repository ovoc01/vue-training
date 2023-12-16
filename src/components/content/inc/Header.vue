<script>
export default {
  name: 'custom-header'
}
</script>

<template>
  <header>
    <div class="navigation">
      <span class="element">
            Accounts
      </span>
      <span class="element">
            Payments
      </span>
      <span class="element">
            Employees
      </span>
      <span class="element">
            Analytics
      </span>
      <span class="element">
            Loans
      </span>

    </div>
    <div class="icon-container">
        <span class="icon element">
            <i class="bi bi-bell"></i>
        </span>
      <span class="solution element">
          <span>
            Paper Solutions LLC
          </span>
        <span class="color">
              P
        </span>
      </span>

    </div>

  </header>
</template>

<style scoped lang="scss">
header {
  width: 100%;
  height: 10%;
  display: flex;
  justify-content: space-around;
  align-items: center;

  .navigation {
    width: 60%;
    height: 50%;
    display: flex;
    justify-content: space-evenly;
    align-items: center;

    .element {
      width: 100%;
      height: 100%;
      display: flex;
      justify-content: center;
      align-items: center;
      font-size: 16px;
      font-weight: bold;
      color: $color-secondary;
      cursor: pointer;

      &:hover {
        color: white;
        background-color: black;
        border-radius: 20px;

      }
    }
  }

  .icon-container {
    width: 25%;
    height: 60%;
    display: flex;
    justify-content: space-around;
    align-items: center;
    margin-right: 20px;

    .element{
      background-color: #e8e8e8;
      border-radius: 20px;
      cursor: pointer;
    }

    .icon {
      width: 20%;
      height: 100%;
      display: flex;
      justify-content: center;
      align-items: center;
      i {
        font-size: 25px;
        color: black;
        font-weight: bold;
      }
    }

    .solution {
      width: 70%;
      height: 100%;
      display: flex;
      justify-content: space-evenly;
      align-items: center;
      font-size: 16px;
      font-weight: bold;
      color: black;
      cursor: pointer;
      .color{
        background-color: rgb(234,73,107);
        display: flex;
        justify-content: center;
        align-items: center;
        color: white;
        border-radius: 15px;
        font-size: 25px;
        width: 40px;
        height: 40px;
      }
    }
  }
}

</style>