<template>
  <div>
    Formページ
    <HeadComp></HeadComp>
    <TextareaComp></TextareaComp>
    <StringComp></StringComp>
    <button v-on:click="buttonAction">{{ button }}</button>
  </div>
</template>

<script>
import HeadComp from "@/components/modules/HeadComp";
import TextareaComp from "@/components/modules/TextareaComp";
import StringComp from "@/components/modules/StringComp";
//mapActins→VuexのActionを使うためのもの
import { mapActions, mapGetters } from "vuex";
export default {
  name: "form",
  data() {
    return {
      button: "確認"
    };
  },
  methods: mapActions("Form", {
    buttonAction: "buttonAction"
  }),
  components: {
    HeadComp,
    TextareaComp,
    StringComp
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped></style>
