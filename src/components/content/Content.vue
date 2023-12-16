<template>
  <div class="content">
    <custom-header />
    <main>
      <header>

            <span class="element register">
                  <span class="label">
                   <span class="text">Register #284</span>
                    <span class="pending">Pending</span>
                  </span>
              <span class="count">
                $103,450.50
              </span>
              <span class="btn-container">
                <button class="btn send">
                  <i class="bi bi-send-arrow-down"></i>
                  Send Payouts
                </button>
                <button class="btn option">
                 <i class="bi bi-three-dots"></i>
                </button>
              </span>
            </span>
        <span class="element new-register">
            <span class="label">
              <span class="text">New Register</span>
              <span class="text">Payout register to select employees</span>
              <span class="btn-container">

              </span>
            </span>

            </span>
        <span class="element schedules">

            </span>

      </header>
      <div class="content">

      </div>
      <footer>

      </footer>

    </main>
  </div>
</template>

<style scoped lang="scss">
.content {
  width: 100%;
  height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;


  main {
    width: 95%;
    height: 85%;
    background-color: white;
    border-radius: 20px;
    border: solid 1px rgb(223, 225, 227);

    header {
      width: 100%;
      height: 25%;
      border-top-left-radius: 20px;
      border-top-right-radius: 20px;
      border-bottom: solid 1px rgb(223, 225, 227);
      display: flex;
      justify-content: space-between;
      align-items: center;

      .register {
        width: 35%;
        height: 80%;

        display: flex;
        flex-direction: column;
        align-items: center;

        .label{
          width: 80%;
          height: 20%;
          display: flex;
          gap:10px ;
          justify-content: flex-start;
          align-items: center;
          font-size: 15px;
          color: $color-secondary;
          .pending{
            color: $color-tertiary;
          }
        }

        .count{
          width: 80%;
          height: 40%;
          display: flex;
          justify-content: flex-start;
          align-items: center;
          font-size: 30px;
          color: $color-secondary;

        }

        .btn-container{
          width: 80%;
          height: 40%;
          display: flex;
          justify-content: flex-start;
          align-items: center;
          gap: 10px;
          .btn{
            border-radius: 15px;

            border: none;
            height: 50px;
            font-size: 15px;
            font-weight: bold;
            cursor: pointer;
          }
          .send{
            width: 250px;
            background-color: $color-tertiary;
            color: $color-primary;
            i{
              font-size: 20px;

            }
          }

          .option{
            width: 50px;
            background-color: white;
            color: $color-secondary;
            border: solid 1px $color-secondary;
          }

        }

      }

      .new-register {
        width: 40%;
        height: 100%;
        border-right: solid 1px rgb(223, 225, 227);
        border-left: solid 1px rgb(223, 225, 227);
        display: flex;
        flex-direction: column;
        align-items: center;
        .label{
          width: 80%;
          height: 20%;
          display: flex;
          gap:10px ;
          align-items: center;
          font-size: 15px;
          text-align: start;
          color: $color-secondary;
          .pending{
            color: $color-tertiary;
          }
        }
      }

      .schedules {
        width: 25%;
        height: 100%;

      }


    }

    .content {
      width: 100%;
      height: 60%;

    }

    footer {
      width: 100%;
      height: 15%;
      border-bottom-left-radius: 20px;
      border-bottom-right-radius: 20px;
      border-top: solid 1px rgb(223, 225, 227);
    }


  }
}
</style>
<script setup>
import CustomHeader from '@/components/content/inc/Header.vue'
</script>