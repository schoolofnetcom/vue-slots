<template>
    <a class="e-btn">
        <slot></slot>
    </a>
</template>
<style>
.e-btn {
  display: inline-block;
  padding: 10px 15px;
  background: #e74c3c;
  color: white;
  text-decoration: none;
  border-radius: 6px;
  border-right: 2px #2c3e50 solid;
  border-bottom: 2px #2c3e50 solid;
  transition: background ease .5s;
}

.e-btn:hover {
  background: #c0392b;
}
</style>
