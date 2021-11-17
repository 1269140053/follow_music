<template>
  <div class="f_container">
  <div class="f_left-icon">
    <img class="music_img" src="https://p2.music.126.net/UV7LczgG7Jd6ZXc5WLHVWg==/109951165177553168.jpg?param=50y50">
  </div>
  <div class="f_right_tool">
    <div class="tool_display">
      <div class="display_title">疑心病</div>
      <div class="display_cotent"></div>
    </div>
    <div class="tool_btn">
      <div class="last_btn btn">
        <button></button>
      </div>
      <div class="stop_btn btn"><button></button></div>
      <div class="next_btn btn"><button></button></div>
    </div>
    <div class="tool_progress"></div>
  </div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.tool_btn .btn{
  flex: 1;
  text-align: center;
}
.tool_display{
  display: flex;
}
.tool_display .display_title{
   font-size: 8px;
   text-align: center;
   color: #336666;
   font-weight: bold;
   width: 40px; 
}
.tool_btn .btn button{
   border-radius: 50%;
   outline: none;
   border: none;
   cursor: pointer;
   background-color: #6666CC;
   width: 24px;
   height: 24px;
   background-position: center;
   background-repeat: no-repeat;
}
.stop_btn button{
   background-image: url("./icon/stop.svg");
}
.next_btn button{
   transform: rotate(180deg);
}
.last_btn button,.next_btn button{
   background-image: url("./icon/1.svg");
}
.f_container{
  width: 100%;
  height: 60px;
  display: flex;
  justify-content: space-between;
  padding: 1px;
}
.f_left-icon{
  width: 60px;
  height: 100%;
}
.f_right_tool{
 flex: 1;
 display: flex;
 flex-flow: column;
}
.tool_btn{
  display: flex;
}
.music_img{
  height: 100%;
  width: 100%;
}
.tool_display{
  flex: 1;
}
.tool_progress{
  margin-top:1px ;
  height: 2px;
  width: 100%;
  background-color: #6666CC;
}
</style>
