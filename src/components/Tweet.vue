<template>
  <div className="tweet">
    <ProfileImage :image="user.image"/>

    <div className="body">
      <div className="top">
        <User :user="user" />
        <TimeStamp :timestamp="timestamp" />
      </div>
      <div className="message">
        <Message :message="message" />
      </div>
      

      <div>
        <Actions />
      </div>
    </div>

    <i class="fas fa-ellipsis-h"></i>
  </div>
</template>

<script>
import ProfileImage from './ProfileImage.vue';
import User from './User.vue';
import TimeStamp from './TimeStamp.vue';
import Message from './Message.vue';
import Actions from './Actions.vue';

export default {
    props: ["timestamp", "message", "user"],
    components: { ProfileImage, User, TimeStamp, Message, Actions }
};
</script>

<style scoped>
a {
  color: #42b983;
}
</style>
