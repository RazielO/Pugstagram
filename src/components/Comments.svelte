<script>
  export let comments = [];

  function addComment(event) {
    const text = event.target.commentInput.value;
    if (text.length > 0) {
      const message = {
        id: Date.now(),
        text: text,
        username: "RazielO"
      };
      comments = [...comments, message];
      event.target.commentInput.value = "";
    }
  }
</script>

<style>
  .Comments h3 {
    font-size: 14px;
    color: black;
    font-weight: bold;
    margin: 0;
    padding: 0;
  }
  .Comments span {
    font-size: 14px;
    margin: 0 0 0 0.5em;
    font-weight: normal;
    color: rgba(black, 0.9);
  }
  .add {
    padding: 1em 1em 1em 1em;
    border-top: 1px solid rgba(219, 219, 219, 0.8);
  }
  .add form {
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
  .container {
    padding: 0 1em 0.5em 1em;
  }
  .user-comments {
    margin: 0 0 0.5em 0;
    display: flex;
  }

  input {
    border: solid 1px #e9e9e9;
    border-radius: 5px;
    color: #696969;
    border: 1px solid transparent;
    font-size: 12px;
    outline: none;
    width: 100%;
    display: flex;
  }
  button {
    border: none;
    color: #3897f0;
    font-size: 12px;
    outline: none;
    cursor: pointer;
    background: transparent;
  }
</style>

<div class="Comments">
  <div class="container">
    {#each comments as comment (comment.id)}
      <div class="user-comments">
        <h3>{comment.username}</h3>
        <span>{comment.text}</span>
      </div>
    {/each}
    <div class="add">
      <form on:submit|preventDefault={addComment}>
        <input
          type="text"
          id="commentInput"
          class="input"
          placeholder="Add comment..." />
        <button type="submit">Post</button>
      </form>
    </div>
  </div>
</div>
