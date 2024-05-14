<template>
  <div>
    <div class="freeback-container">
      <div class="freeback-img-box">
        <img src="static/img/freeback.png">
      </div>
      <div class="freeback-box-border">
        <div class="freeback-box">
          <div class="freeback-title">
            <h1>商家入驻</h1>
            <h2>请留下您的联系方式，我们将及时与您联系。</h2>
          </div>
          <div class="freeback-content">
            <div class="freeback-form">
              <Form :model="formItem" :label-width="80">
                <FormItem label="联系电话">
                  <i-input v-model="formItem.title" placeholder="+86"></i-input>
                </FormItem>
                <FormItem label="邮箱地址">
                  <i-input v-model="formItem.content" placeholder="请输入邮箱地址"></i-input>
                </FormItem>
                <FormItem>
                  <Button type="primary">提交</Button>
                  <Button type="ghost">清空信息</Button>
                </FormItem>
              </Form>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Freeback',
  data () {
    return {
      formItem: {
        title: '',
        content: ''
      }
    };
  }
};
</script>

<style scoped>
.freeback-container {
  margin: 15px auto;
  width: 80%;
  height: 600px;
  display: flex;
  align-items: center;
  /* background-color: #ccc; */
}
.freeback-img-box {
  width: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
}
.freeback-img-box img {
  width: 80%;
}
.freeback-box-border {
  width: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
}
.freeback-box {
  width: 480px;
}
.freeback-content {
  margin: 15px auto;
  border: 1px #ccc dotted;
}
.freeback-form {
  margin: 30px auto;
  width: 90%;
}
</style>
