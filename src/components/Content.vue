<template>
    <div class="con">
        <SelectBar></SelectBar>
        <Divider />
        <div class="chartcard">
            <Card class="card" style="width:240px">
                <div class="card-con">
                    <Icon type="md-person" size="48"/>
                </div>
                <div class="card-con">
                    <div style="font-size:large">
                        <span>Person</span>
                        <br>
                        <span style="color:blue;">567346</span>
                    </div>
                </div>
            </Card>

            <Card class="card" style="width:240px">
                <div class="card-con">
                    <Icon type="md-chatbubbles" size="48"/>
                </div>
                <div class="card-con">
                    <div style="font-size:large">
                        <span>Chat</span>
                        <br>
                        <span style="color:blue;">6547346</span>
                    </div>
                </div>
            </Card>
        </div>
    </div>
</template>
<script>
    import SelectBar from './contents/SelectBar'

    export default {
        components: {
            'SelectBar': SelectBar
        }
    }
</script>

<style scope>
    .con {
        padding-left: 16%;
        padding-right: 4%;
    }
    .chartcard {
        text-align: left;
    }
    .card {
        display: inline-block;
    }
    .card-con {
        display: inline-block;
    }
    .ivu-icon {
        vertical-align: sub;
    }
</style>
