<template>
  <WishTree />
  <Interactive />
  <Subject />
  <EventDes />
  <Reward />
  <Question />
  <BtnSignUp />
  <FooterView />
</template>

<script>
import WishTree from '@/components/WishTree.vue';
import Interactive from '@/components/Interactive.vue';
import Subject from '@/components/Subject.vue';
import EventDes from '@/components/EventDes.vue';
import Reward from '@/components/Reward.vue';
import Question from '@/components/Question.vue';
import BtnSignUp from '@/components/BtnSignUp.vue';
import FooterView from '@/components/FooterView.vue';

export default {
  components: {
    WishTree,
    Interactive,
    Subject,
    EventDes,
    Reward,
    Question,
    BtnSignUp,
    FooterView,
    WishTree
}
}
</script>
