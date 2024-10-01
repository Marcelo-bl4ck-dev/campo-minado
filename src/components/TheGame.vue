<script setup>

const rows = 16;
const cols = 16;

async function sendInfo () {
  
}

</script>

<template>
  <v-container class="board">
    <v-responsive>
      <div class="row" v-for="r in rows">
        <div class="col" v-for="c in cols">
          <button class="cell" @click="sendInfo"></button>
        </div>
      </div>
    </v-responsive>
  </v-container>
</template>

<style scoped>
.board {
  display: block;
  width: 370px;
  height: 370px;
  margin: auto;
}
.row {
  display: inline-block;
}
.row,
.col {
  display: flex;
}

.row,
.col,
.cell {
  padding: 0;
  margin: 0;
  border-radius: 0;
}
.col,
.cell {
  width: 23.1px;
  height: 23.1px;
}
</style>