<template>
  <header>
    <div class="container">
      <font-awesome-icon :icon="['fas', 'calculator']" />
      <h1>Counter</h1>
    </div>
  </header>
</template>

<style scoped>
header {
  border-bottom: 1px solid #007e7a;
  height: 50px;
}

.container {
  display: flex;
  gap: 20px;
  align-items: center;
  height: 100%;
}

svg {
  font-size: 38px;
  color: #007e7a;
}

h1 {
  font-size: 30px;
  font-weight: bold;
}
</style>
