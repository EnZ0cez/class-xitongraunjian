<template>
  <div class="personal-page">
    <img :src="avatar" alt="Avatar" class="avatar">
    <h2 class="nickname">{{ nickname }}</h2>
    <p class="student-id">学号：{{ studentId }}</p>
    <!-- 其他个人信息 -->
  </div>
</template>

<script>
export default {
  data() {
    return {
      avatar: '../bocci.jpg', // 头像图片的路径
      nickname: 'Enzo', // 昵称
      studentId: '2310273083' // 学号
      // 其他个人信息的数据
    };
  }
};
</script>

<style scoped>
.personal-page {
  text-align: center;
}

.avatar {
  width: 150px;
  height: 150px;
  border-radius: 50%;
}

.nickname {
  margin-top: 20px;
  font-size: 24px;
}

.student-id {
  margin-top: 10px;
  font-size: 16px;
}
</style>