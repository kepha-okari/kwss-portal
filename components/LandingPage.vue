<template>
    <b-row class="d-flex">
        <!-- <div class="centered-container">
            <b-button class="card action-card" @click="handleSubmit">
                <img src="../assets/add-user.png" height="40px" width="40px" />
                <p>Action Customer</p>
            </b-button>
            <b-button class="card action-card" @click="handleSubmit">
                <img src="../assets/add.png" height="40px" width="40px" />
                <p>Add Readings</p>
            </b-button>
            <b-button class="card action-card" @click="handleSubmit">
                <img src="../assets/chatting.png" height="40px" width="40px" />
                <p>Send Bills</p>
            </b-button>
        </div> -->
        <ActionCard />
        <ActionCard />
        <ActionCard />
        <ActionCard />
    </b-row>
</template>
<script>
import ActionCard from './ActionCard.vue';

export default{
    methods: {
        handleSubmit() {
            return window.location.href = "/readings";
        }
    },
    components: { ActionCard }
}
</script>

<style>
.action-card{
    padding: 10px;
    background-color: #e6f0f8;
    color: #000;
    height: 160px;
    width: 120px;
    border: none;
    justify-content: center;
    text-align: center;
    align-items: center;
    display: flex;
    flex-wrap: wrap;
    margin-inline: 5px;
    border-radius: 10px;
}
.centered-container{
    justify-content: center;
    text-align: center;
    align-items: center;
    display: flex;
    margin-top: 20px;
    flex-direction: row;
}
</style>
