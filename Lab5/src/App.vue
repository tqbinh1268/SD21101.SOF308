<script setup>
import { ref } from "vue";
import PostList from "./components/PostList.vue";

const posts = [
  {
    title: "Sài Gòn Xưa",
    content:
      'Sài Gòn xưa trong ký ức nhiều thế hệ là "Hòn ngọc Viễn Đông" đầy hoa lệ nhưng cũng rất đỗi bình dị. Đó là hình ảnh những chiếc xe bát phố chạy thênh thang dưới hàng dầu cổ thụ, là tiếng chuông nhà thờ Đức Bà vang vọng trong buổi chiều tà. Người Sài Gòn xưa thanh lịch với tà áo dài thướt tha trên đường Tự Do, hay những quý ông chỉn chu bên ly cà phê vợt nghi ngút khói. Không chỉ có vẻ đẹp kiến trúc Pháp cổ kính, cái hồn của Sài Gòn còn nằm ở nhịp sống hào sảng, trọng nghĩa khinh tài. Dẫu thời gian đã phủ lớp bụi mờ, nhưng vẻ đẹp duyên dáng và cái chất "vừa Tây vừa Ta" ấy vẫn mãi là một hoài niệm đẹp trong lòng người lữ thứ.',
    author:'AI OMG'
  },
];
</script>

<template>
  <PostList :posts="posts" />
</template>
