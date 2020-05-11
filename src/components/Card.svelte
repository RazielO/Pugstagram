<script>
  import Comments from "./Comments.svelte";
</script>

<div class="Card">
  <div class="container">
    <div class="header">
      <div class="user">
        <img src="https://arepa.s3.amazonaws.com/elmo002.jpg" alt="" />
        <h2>
          Elmo.pug
          <span>Bogotá, Colombia</span>
        </h2>
      </div>
      <div class="settings">
        <i class="fas fa-ellipsis-h" />
      </div>
      <div class="photo">
        <figure>
          <img src="https://arepa.s3.amazonaws.com/elmo002.jpg" alt="" />
        </figure>
      </div>
    </div>
    <div class="icons">
      <div class="icons-first">
        <i class="fas fa-heart" />
        <i class="fas fa-paper-plane" />
      </div>
      <div class="icons-last">
        <i class="fas fa-bookmark" />
      </div>
    </div>
    <div class="description">
      <h3>elmo.pug</h3>
      <span>Hi! It's Elmo</span>
    </div>
    <Comments />
  </div>
</div>
