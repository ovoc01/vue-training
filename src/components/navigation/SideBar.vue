<template>
    <aside>
        <div class="logo">
            RSTR+
        </div>
        <div class="account-balance">
            <div class="upper-content">
                <p>Account balance</p>
                <span class="net-worth">
                    $1,282,250
                </span>
                <p>
                    -$1,600 in pending transactions
                </p>
            </div>
            <div class="lower-content">
                <div class="button-container">
                    <div class="button">
                      <i class="bi bi-send-arrow-down"></i>
                    </div>
                    <p>Send</p>
                </div>

                <div class="button-container">
                    <div class="button">
                      <i class="bi bi-window"></i>
                    </div>
                    <p>Withdraw</p>
                </div>
                <div class="button-container">
                    <div class="button">
                      <i class="bi bi-bookmark-plus"></i>
                    </div>
                    <p>Statement</p>
                </div>


            </div>
        </div>
        <div class="account-card-container">
            <span class="title">Account card
                <p class="info">
                    For your company everyday expenses
                </p>
            </span>
            <div class="account-card">

            </div>
            <div class="account-card">

            </div>

            <button class="add-card">
                New card or product
            </button>
        </div>

    </aside>
</template>

<script setup>


</script>

<style lang="scss">
aside {
    background-color: white;
    width: 25%;
    height: 100vh;
    display: flex;
    flex-direction: column;
    align-items: center;
    row-gap: 20px;

    .logo {
        text-align: center;
        font-size: 30px;
        font-weight: 400;
        margin-top: 20px;
        margin-bottom: 20px;
        color: $color-secondary;
    }

    .account-balance {
        background-color: $color-primary;
        border-radius: 20px;
        width: 90%;
        height: 250px;
        

        display: flex;
        flex-direction: column;
        row-gap: 5px;
        align-items: center;

        .upper-content {
            margin-top: 20px;
            display: flex;
            flex-direction: column;
            row-gap: 10px;
            align-items: start;
            width: 90%;

            p {
                font-size: 11px;
                font-weight: 400;

            }

            .net-worth {
                font-size: 30px;
            }

        }

        .lower-content {
            margin-top: 40px;
            width: 100%;
            display: flex;
            flex-direction: row;

            justify-content: space-around;

            .button-container{
                text-align: center;
                display: flex;
                flex-direction: column;
                row-gap: 10px;
                p{
                    
                    font-size: 10px;
                    text-transform: capitalize;
                }
                .button {
                    border-radius: 50%;
                    width: 60px;
                    height: 60px;
                    background-color: white;
                    box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.1);
                    cursor: pointer;
                  display: flex;
                  align-items: center;
                  justify-content: center;

                  i{
                    font-size: 25px;
                    color: $color-secondary;
                  }
                }
            }
        }

    }

    .account-card-container {
        width: 90%;
        display: flex;
        flex-direction: column;
        row-gap: 20px;

        .account-card {
            width: 100%;
            height: 150px;
            background-color: $color-quaternary;
            border-radius: 25px;
            cursor: pointer;
        }

        .title {
            font-size: 20px;
            font-weight: 400;
            color: $color-secondary;
        }

        .info {
            font-size: 12px;
            font-weight: 400;
            color: $color-secondary;
        }

        .add-card {
            width: 100%;
            height: 60px;
            border-radius: 15px;
            background-color: white;
            border: 1px solid $color-secondary;
            font-size: 15px;
            font-weight: 600;
            cursor: pointer;


        }

        .add-card:hover {
            background-color: $color-secondary;
            color: white;
        }
    }
}
</style>