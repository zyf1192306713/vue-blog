<template>
  <div class="error-wrapper">
    <div class="error-content">
      <el-row :gutter="15">
        <el-col :xs="24" :sm="24" :md="12" :lg="12" :xl="12">
          <div class="pic-error">
            <img src="@/assets/404.png" alt="404">
          </div>
        </el-col>
        <el-col :xs="24" :sm="24" :md="12" :lg="12" :xl="12">
          <div class="bullshit">
            <div class="bullshit-oops">抱歉!</div>
            <div class="bullshit-headline">当前页面不存在...</div>
            <div class="bullshit-info">请检查您输入的网址是否正确，或点击下面的按钮返回！</div>
            <a class="bullshit-return-home" href="/">返回首页</a>
          </div>
        </el-col>
      </el-row>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Page404'
}
</script>

<style scoped lang="less">
	.error-wrapper {
	  position: absolute;
	  top: 40%;
	  left: 50%;
	  transform: translate(-50%, -50%);
	  .error-content {
	    .pic-error {
	      float: left;
	      width: 120%;
	      overflow: hidden;
	      opacity: 0;
	      animation-name: slideUp;
	      animation-duration: 0.5s;
	      animation-delay: 0.3s;
	      animation-fill-mode: forwards;
	      img {
	        width: 100%;
	        height: 100%;
	      }
	    }
	    .bullshit {
	      position: relative;
	      float: left;
	      width: 300px;
	      padding: 30px 0;
	      overflow: hidden;
	      &-oops {
	        margin-bottom: 20px;
	        font-size: 32px;
	        font-weight: bold;
	        line-height: 40px;
	        color: #409eff;
	        opacity: 0;
	        animation-name: slideUp;
	        animation-duration: 0.5s;
	        animation-fill-mode: forwards;
	      }
	      &-headline {
	        margin-bottom: 10px;
	        font-size: 20px;
	        font-weight: bold;
	        line-height: 24px;
	        color: #222;
	        opacity: 0;
	        animation-name: slideUp;
	        animation-duration: 0.5s;
	        animation-delay: 0.1s;
	        animation-fill-mode: forwards;
	      }
	      &-info {
	        margin-bottom: 30px;
	        font-size: 13px;
	        line-height: 21px;
	        color: rgba(0, 0, 0, 0.65);
	        opacity: 0;
	        animation-name: slideUp;
	        animation-duration: 0.5s;
	        animation-delay: 0.2s;
	        animation-fill-mode: forwards;
	      }
	      &-return-home {
	        display: block;
	        float: left;
	        width: 110px;
	        height: 36px;
	        font-size: 14px;
	        line-height: 36px;
	        color: #fff;
	        text-align: center;
	        cursor: pointer;
	        background: #409eff;
	        border-radius: 100px;
	        opacity: 0;
	        animation-name: slideUp;
	        animation-duration: 0.5s;
	        animation-delay: 0.3s;
	        animation-fill-mode: forwards;
	      }
	    }
	    @keyframes slideUp {
	      0% {
	        opacity: 0;
	        transform: translateY(60px);
	      }
	      100% {
	        opacity: 1;
	        transform: translateY(0);
	      }
	    }
	  }
	}
	
</style>
