<template>
    <div class="main_header">
        <div class="left_head">
            <h1>{{fullName}}, {{group}}</h1>
        </div>
        <div class="right_head">
            <h1>  №: {{variant}}</h1>
        </div>
    </div>
</template>

<script>
export default {
    name: "Header",
    props: {
        variant: String,
        group: String,
        firstName: String,
        lastName: String
    },
    computed: {
        fullName() {
            return this.firstName + ' ' + this.lastName;
        }
    }
}
</script>

<style scoped>

.main_header{
    color: #ffffff;
    background-color: #5469d4;
    overflow: hidden;
    width: 100%;
    padding: 0 0 20px;
    /*background: white;*/
    border-radius: 4px;
    box-shadow: rgba(60, 66, 87, 0.12) 0px 7px 14px 0px, rgba(0, 0, 0, 0.12) 0px 3px 6px 0px;
}

.left_head{
    width: 50%;
    float: left;
    padding: 1%;

}

.right_head{
    width: 43%;
    float: right;
    text-align: right;
    padding: 1%;
}

</style>