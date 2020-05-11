<style>
  .Stories {
    border: 1px solid rgba(219, 219, 219, 1);
    border-radius: 4px;
    margin: 1em 0;
    padding: 0.5em 1em;
    background-color: white;
  }
  .item img {
    width: 32px;
    height: 32px;
    border-radius: 50%;
  }
  .item {
    display: flex;
    align-items: center;
    margin: 0 0 0.5em 0;
  }
  .item h2 {
    font-size: 14px;
    color: black;
    margin: 0 0 0 0.5em;
  }
  .item h2 span {
    display: block;
    font-size: 9px;
    text-transform: uppercase;
    color: gray;
  }
  .head {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 0.5em 0 0 0;
  }
  .head h2 {
    font-size: 12px;
    font-weight: 600;
  }
  .head span {
    font-size: 12px;
    font-weight: normal;
    color: black;
  }
  .items {
    margin: 0.5em 0 0.5em 0;
  }
  .item-box {
    width: 32px;
    height: 32px;
    border: double 2px transparent;
    border-radius: 100%;
    background-image: linear-gradient(#fff, #fff),
      radial-gradient(circle at top left, #f09433, #bc1888);
    background-origin: border-box;
    background-clip: content-box, border-box;
  }
</style>

<div class="Stories">
  <div class="container">
    <div class="head">
      <h2>Stories</h2>
      <span>See all</span>
    </div>
    <div class="items">
      <div class="item">
        <div class="item-box">
          <img src="https://arepa.s3.amazonaws.com/oscar.png" alt="User" />
        </div>
        <h2>
          RazielO
          <span>10 hours ago</span>
        </h2>
      </div>
    </div>
  </div>
</div>
