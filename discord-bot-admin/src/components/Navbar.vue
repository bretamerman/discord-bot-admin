<template>
    <div class="topnavbar">
        <div class="row">
            <div class="left column">
                <div class="hamburger">
                    hello
                </div>
            </div>
            <div class="middle column">b</div>
            <div class="right column">c</div>
        </div>
    </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'Navbar',
  props: {
    msg: String,
  },
});
</script>


<style scoped>
.topnavbar {
    width: calc(100%-10px);
    height: 50px;
    border: #000;
    /* border-style: solid; */
    background-color: lightskyblue;

}

/* Clear floats after the columns */
.row:after {
  content: "";
  display: table;
  clear: both;
}

.column {
  float: left;
  padding: 0px;
  height: 50px; /* Should be removed. Only for demonstration */
  display: flex;
}

.left, .right {
  width: 24%;
}

.middle {
  width: 49%;
}

.hamburger {
    padding: 5px;
    border-style: solid;
}

</style>