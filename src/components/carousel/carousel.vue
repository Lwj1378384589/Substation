<template>
    <div class="fz-lunbo"> 
        <!-- Hover触发-->
        <div class="fz-lbbutton">
            <div >
                <el-carousel height="200px">
                    <el-carousel-item  v-for="data in list " :key="data.src">
                        <img v-bind:src="data.src">
                    </el-carousel-item>
                </el-carousel>
            </div>
        </div>
    </div>
</template>
<script>
export default { 
    data(){
        return{
            list:[
                { src:'static/img/fz_carousel1.jpg' },
                { src:'static/img/fz_carousel2.jpg' },
                { src:'static/img/fz_carousel3.jpg' },
                { src:'static/img/fz_carousel4.jpg' },
                { src:'static/img/fz_carousel5.jpg' }
            ]
        }
    }  
}
</script>
<style >
.fz-lunbo { float: right; height: 200px; width: 330px;border: #ddd 1px solid; }
/* .fz-lunbo img{ height: 200px; width: 330px; } */
.el-carousel__indicators{
    left: 42%;
}
.el-carousel__button{
    height: 4px;
    border-radius: 3px;
}
.fz-lunbo img{
     height: 200px; width: 330px;
}
</style>
