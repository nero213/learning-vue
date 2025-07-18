<template>
  <div class="container">
    <img :src="icon" alt="Brand Icon" class="brand-icon" />
    <div class="mybrand">{{ brandText }}</div>
  </div>
</template>

<script>
import icon from '../assets/icon.svg'

export default {
  name: 'Mybrand',
  data() {
    return {
      icon,
      brandText: 'My Brand', // Replace with dynamic brand name if needed
    };
  },
}
</script>

<style scoped>
.container {
  display: flex;
  align-items: center;
  gap: 1rem;
  padding: 1rem;
  background-color: #2c3e50;
  border-radius: 8px;
  box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
  transition: transform 0.3s ease;
}

.container:hover {
  transform: scale(1.05);
}

.brand-icon {
  width: 3rem;
  height: 3rem;
  object-fit: contain;
  transition: transform 0.3s ease;
}

.container:hover .brand-icon {
  transform: rotate(10deg);
}

.mybrand {
  color: #fff;
  font-size: 1.8rem;
  font-weight: bold;
  letter-spacing: 1px;
  transition: color 0.3s ease;
}

.container:hover .mybrand {
  color: #ecf0f1;
}

@media (max-width: 600px) {
  .container {
    flex-direction: column;
    align-items: center;
  }

  .mybrand {
    font-size: 1.5rem;
  }
}
</style>
