<template>
  <div class="profiles-page">
      <h1>Profile Page</h1>
      <div class="profile-list">
        <div class="profile-item" v-for="(item,index) in profiles" :key="index">
            <img :src="item.avatar" alt="">
            <span>{{ item.name }}</span>
        </div>
      </div>
  </div>
</template>

<script>
export default {
    name: "profiles",
    data: () => {
        return {
            profiles: [
                {   
                    id: 1,
                    name: "Nguyễn Thị A",
                    avatar: "https://i.pravatar.cc/300",
                    gender: "female",
                },
                {
                    id: 2,
                    name: "Nguyễn Văn B",
                    avatar: "https://cdn.icon-icons.com/icons2/1736/PNG/512/4043260-avatar-male-man-portrait_113269.png",
                    gender: "male",
                },
                {
                    id: 3,
                    name: "Nguyễn Thị C",
                    avatar: "https://www.w3schools.com/howto/img_avatar2.png",
                    gender: "female",
                },
                {
                    id: 4,
                    name: "Nguyễn Văn D",
                    avatar: "https://ict-imgs.vgcloud.vn/2020/09/01/19/huong-dan-tao-facebook-avatar.jpg",
                    gender: "male",
                },
            ]
        }
    }
}
</script>

<style>
h1{
    margin-bottom: 30px;
}
.profile-list{
    width: 800px;
    margin: auto;
}
.profile-item{
    display: inline-block;
    margin: 20px;
    width: 300px;
    height: 300px;
    background-color: #c0bebe;
    cursor: pointer;
}
img{
    width: 100%;
    height: 100%;
}
</style>