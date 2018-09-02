<template>
    <div class='select'>
        <Row>
            <Col span="12" style="width:80%;">
                <label>OS</label>
                <Select v-model="model1" style="width:18%;">
                    <Option v-for="item in cityList" :value="item.value" :key="item.value">{{ item.label }}</Option>
                </Select>
                <label>platform</label>
                <Select v-model="model1" style="width:18%;">
                    <Option v-for="item in cityList" :value="item.value" :key="item.value">{{ item.label }}</Option>
                </Select>
                <label>serverid</label>
                <Select v-model="model1" style="width:18%;">
                    <Option v-for="item in cityList" :value="item.value" :key="item.value">{{ item.label }}</Option>
                </Select>
                <label>channel</label>
                <Select v-model="model1" style="width:18%;">
                    <Option v-for="item in cityList" :value="item.value" :key="item.value">{{ item.label }}</Option>
                </Select>
            </Col>
            <Col span="12" style="width:10%;">
                <DatePicker type="date" placeholder="Select date" style="width: 200px"></DatePicker>
            </Col>
        </Row>
    </div>
</template>
<script>
    export default {
        data () {
            return {
                cityList: [
                    {
                        value: 'New York',
                        label: 'New York'
                    },
                    {
                        value: 'London',
                        label: 'London'
                    },
                    {
                        value: 'Sydney',
                        label: 'Sydney'
                    },
                    {
                        value: 'Ottawa',
                        label: 'Ottawa'
                    },
                    {
                        value: 'Paris',
                        label: 'Paris'
                    },
                    {
                        value: 'Canberra',
                        label: 'Canberra'
                    }
                ],
                model1: ''
            }
        }
    }
</script>

<style scope>
    .select {
        padding-top: 1%;
        text-align: left;
    }
    label {
        padding: 0.5%;
    }
</style>
