<template>
  <div class="content">
    <h3>
      Contact Us
    </h3>
    <p>
      The quick brown fox jumps over the lazy dog, creating a frenzy among the nearby crowd.
    </p>
    <img src="./../assets/img/contacts.png" alt="Image Webpack 5">
    <h4 class="h4">
      Address
    </h4>
    <p>
      The quick brown fox jumps over the lazy dog, creating a frenzy among the nearby crowd.
    </p>
    <h4 class="h4">
      Phone
    </h4>
    <ul>
      <li>
        <a href="tel:89222334410">
          89222334410
        </a>
      </li>
      <li>
        <a href="tel:89222334310">
          89222334310
        </a>
      </li>
    </ul>
    <h4 class="h4">
      Online service
    </h4>
    <ul>
      <li>
        <a href="mailto:koptevdeveloper@gmail.com">
          koptevdeveloper@gmail.com
        </a>
      </li>
      <li>
        <a href="https://kinf.agt72.ru/">
          kinf.agt72.ru
        </a>
      </li>
    </ul>
    <h4 class="h4">
      Send us message
    </h4>
    <form action="" class="contacts-form">
      <label for="full_name">
        Full Name
      </label>
      <input class="input"  id="full_name" type="text" placeholder="Full Name" name="full_name">
      <label for="email">
        Email
      </label>
      <input class="input"  id="email" type="email" placeholder="Email" name="email">
      <label for="message">
        Message
      </label>
      <textarea class="input" id="message" placeholder="Message" name="message"></textarea>
      <input class="submit custom-submit" type="submit" name="submit">
    </form>
  </div>
</template>

<script>
export default {
  name: "Contacts"
}
</script>

<style scoped>

</style>