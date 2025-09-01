<template>
  <div class="home">
    <nav>
      <ul>
        <li><a href="#home-section">Home</a></li>
        <li><a href="#about-section">About</a></li>
        <li><a href="#contact-section">Contact Us</a></li>
      </ul>
    </nav>

    <section id="home-section">
      <h1>Welcome to Our Website</h1>
      <p>This is the homepage. Explore to learn more about us!</p>
    </section>

    <section id="about-section">
      <h2>About Us</h2>
      <p>This section provides information about our application or organization.</p>
    </section>

    <section id="contact-section">
      <h2>Contact Us</h2>
      <p>If you have any questions, feel free to reach out!</p>
      <form>
        <label for="name">Name:</label>
        <input type="text" id="name" name="name" required>
        
        <label for="email">Email:</label>
        <input type="email" id="email" name="email" required>
        
        <label for="message">Message:</label>
        <textarea id="message" name="message" required></textarea>
        
        <button type="submit">Send</button>
      </form>
    </section>
  </div>
</template>

<script>
export default {
  name: 'Home',
}
</script>

<style scoped>
.home {
  padding: 20px;
  max-width: 600px;
  margin: 0 auto;
}

nav ul {
  display: flex;
  gap: 20px;
  list-style: none;
  padding: 0;
  margin-bottom: 30px;
  justify-content: center;
}

nav a {
  text-decoration: none;
  color: #007BFF;
  font-weight: bold;
}

nav a:hover {
  text-decoration: underline;
}

section {
  margin-bottom: 30px;
}

form {
  display: flex;
  flex-direction: column;
}

label {
  margin-top: 10px;
}

input, textarea {
  margin-top: 5px;
  padding: 10px;
  border: 1px solid #ccc;
  border-radius: 4px;
}

button {
  margin-top: 10px;
  padding: 10px;
  background-color: #007BFF;
  color: white;
  border: none;
  border-radius: 4px;
  cursor: pointer;
}

button:hover {
  background-color: #0056b3;
}
</style>