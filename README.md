<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <script src="./vue.js"></script>
</head>
<body>
    <div id="app">
        <div v-bind:style="{backgroundColor:pink,width:width,height:height}">
            <div v-bind:style="myDiv"></div>
        </div>
    </div>
    <script>
        var vm=new Vue({
            el:'#app',
            data:{
                myDiv:{backgroundColor:'red',width:'100px',height:'100px'},
                pink:'pink',
                width:'100%',
                height:'200px'
            }
        })
    </script>
</body>
</html>
