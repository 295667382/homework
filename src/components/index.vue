<template lang="html">
  <div class="box">
      <div class="user-info">
          <h3>信息录入系统</h3>
          <div class="info">
            <div class="line">
              <span>姓&nbsp;&nbsp;&nbsp;名：</span>
              <p><input type="text" name="username" value="" class="user-input"></p>
            </div>
            <div class="line">
              <span>手机号：</span>
              <p><input type="text" name="phone" value="" class="user-input"></p>
            </div>
            <div class="line">
              <span>性别：</span>
              <p>
                <label class="radio_label"><input type="radio" name='a'> 男</label>
                <label class="radio_label"><input type="radio" name='a'> 女</label>
                <label class="radio_label"><input type="radio" name='a'> 保密</label>
              </p>
            </div>
            <div class="line">
              <span>爱好：</span>
              <p>
                <label class="checkbox_label"><input type="checkbox" name='a'> 音乐 </label>
                <label class="checkbox_label"><input type="checkbox" name='a'> K歌 </label>
                <label class="checkbox_label"><input type="checkbox" name='a'> 游泳 </label>
              </p><p>
                <label class="checkbox_label"><input type="checkbox" name='a'> 电影 </label>
                <label class="checkbox_label"><input type="checkbox" name='a'> 运动 </label>
                <label class="checkbox_label"><input type="checkbox" name='a'> 游戏 </label>
              </p>
            </div>
            <div class="line">
              <span>城市：</span>
              <p class="select_box">
                  <select class="city" name="aa">
                      <option value="1">北京</option>
                      <option value="1">北京</option>
                      <option value="1">北京</option>
                      <option value="1">北京</option>
                      <option value="1">北京</option>
                      <option value="1">北京</option>
                      <option value="1">北京</option>
                      <option value="1">北京</option>
                      <option value="1">北京</option>
                      <option value="1">北京</option>
                      <option value="1">北京</option>
                      <option value="1">北京</option>
                  </select>
                  <select class="city" name="aa">
                      <option value="1">区域</option>
                      <option value="1">北京</option>
                      <option value="1">北京</option>
                      <option value="1">北京</option>
                      <option value="1">北京</option>
                      <option value="1">北京</option>
                      <option value="1">北京</option>
                      <option value="1">北京</option>
                      <option value="1">北京</option>
                      <option value="1">北京</option>
                      <option value="1">北京</option>
                      <option value="1">北京</option>
                  </select>
                  <select class="city" name="aa">
                      <option value="1">朝阳</option>
                      <option value="1">北京</option>
                      <option value="1">北京</option>
                      <option value="1">北京</option>
                      <option value="1">北京</option>
                      <option value="1">北京</option>
                      <option value="1">北京</option>
                      <option value="1">北京</option>
                      <option value="1">北京</option>
                      <option value="1">北京</option>
                      <option value="1">北京</option>
                      <option value="1">北京</option>
                  </select>
              </p>

            </div>
            <div class="line">
              <span>简介：</span>
              <p class="textarea_box">
                  <textarea class="text-box"></textarea>
              </p>

            </div>
            <div class="line">
              <button class="sub_btn">提交</button>
              <button class="sub_btn">重置</button>
            </div>
          </div>
      </div>
  </div>
</template>

<script>
export default {
}
</script>

<style lang="less" scoped>
  @base-color: #26c6da;
.box{
  position: fixed;
  top: 0;
  right: 0;
  bottom: 0;
  left: 0;
  background: url(../assets/img/background.jpg);
  background-repeat: no-repeat;
  background-size: 100% 100%;
  min-width: 1200px;
  text-align: left;
  font-size: 14px;
  h3{
    text-align: center;
  }
  .user-info{
    position: absolute;
    width: 500px;
    height: 600px;
    left: 50%;
    top: 50%;
    margin-left: -250px;
    margin-top: -300px;
    background-color: rgba(255,255,255,.7);
    border-radius: 4px;
    .info{
      .line{
        display: block;
        position: relative;
        width: 80%;
        margin: 0 auto;
        padding-left: 80px;
        margin-top: 30px;
        &:hover{
          span{
            color: @base-color;
          }
        }

        span{
          display: inline-block;
          position: absolute;
          left:10px;
          font-size: 14px;
          line-height:30px;
          transition: all .2s linear;
        }
        p{
          display: block;
          input.user-input{
            display: block;
            width: 100%;
            height: 30px;
            margin: 0 auto;
            padding-left: 10px;
            border-radius: 2px;
            border: 1px solid #ddd;
            line-height: 28px;
            font-size: 14px;
            transition: all .2s linear;
            &:hover{
              border-color: @base-color;
            }
            &:focus{
              border-radius: 20px;
            }
          }
        }
        .radio_label{
          margin-right: 20px;
        }
        .checkbox_label{
          margin-right: 20px;
        }
        .select_box{
          select{
            margin-right: 15px;
            min-width: 80px;
            height: 30px;
            border-color: #ddd;
            background-color: #fff;
            text-align: center;
          }
        }
        .textarea_box{
          textarea{
            width: 320px;
            height: 100px;
            resize: none;
            padding: 8px;
            border: 1px solid #ddd;
            transition: all .2s linear;
            &:hover, &:focus{
              border-color: @base-color;
            }
          }
        }
        button{
          width: 120px;
          height: 30px;
          background-color: #fff;
          border-radius: 20px;
          border: 1px solid #ddd;
          transition: all .2s linear;
          margin-right: 35px;
          &:nth-child(1){
            background-color: @base-color;
            color: #fff;
            border-color: transparent;
            &:hover{
              background-color: #fff;
              border-color: @base-color;
              color: @base-color;
            }
          }
          &:nth-child(2){
            background-color: #fff;
            border-color: @base-color;
            color: @base-color;
            &:hover{
              background-color: @base-color;
              border-color: transparent;
              color: #fff;
            }
          }
        }
      }
    }
  }
}
</style>
