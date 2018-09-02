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
        <div>
          <div id="container" style="height: 400px; padding-right: 3%"></div>
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

   $(document).ready(function() {
   var title = {
      text: '城市平均气温'
   };
   var subtitle = {
      text: 'Source: runoob.com'
   };
   var xAxis = {
      categories: ['Jan', 'Feb', 'Mar', 'Apr', 'May', 'Jun',
         'Jul', 'Aug', 'Sep', 'Oct', 'Nov', 'Dec']
   };
   var yAxis = {
      title: {
         text: 'Temperature (\xB0C)'
      },
      plotLines: [{
         value: 0,
         width: 1,
         color: '#808080'
      }]
   };

   var tooltip = {
      valueSuffix: '\xB0C'
   }

   var legend = {
      layout: 'vertical',
      align: 'right',
      verticalAlign: 'middle',
      borderWidth: 0
   };

   var series =  [
      {
         name: 'New York',
         data: [-0.2, 0.8, 5.7, 11.3, 17.0, 22.0, 24.8,
            24.1, 20.1, 14.1, 8.6, 2.5]
      }
   ];

   var json = {};

   json.title = title;
   json.subtitle = subtitle;
   json.xAxis = xAxis;
   json.yAxis = yAxis;
   json.tooltip = tooltip;
   json.legend = legend;
   json.series = series;

   $('#container').highcharts(json);
});
</script>

<style scope>
    .con {
        padding-left: 16%;
        padding-right: 4%;
    }
    .chartcard {
        text-align: left;
        background: white;
        margin-right: 3%;
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
