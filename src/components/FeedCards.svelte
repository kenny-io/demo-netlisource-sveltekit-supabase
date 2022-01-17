<div class="card">
    <div class="container">
      <h4><b>{post.title}</b></h4> 
      <p class="author">by {post.author} - Published on {post.date}</p> 
      <p class="desc">{post.description}</p>
      <a href="/">Read more &rarr; </a>
    </div>
  </div>

  <script>
      // defin props for the component
    export let post
  </script>
<style>
.card {
  box-shadow: 0 4px 8px 0 rgba(0,0,0,0.2);
  transition: 0.3s;
  width: 100%;
  max-width: 100%;
  border-radius: 5px;
  margin-top: 30px;
  height: auto;
  padding: 20px;
}

.author {
  font-size: 14px;
}

.desc {
  max-width: 473px;
}

.card:hover {
  box-shadow: 0 8px 16px 0 rgba(0,0,0,0.2);
}

h4 {
  font-family: SF Pro;
  font-size: 24px;
  font-weight: 700;
  color: #2D3B41;
}

p {
  font-family: SF Pro Text;
  font-size: 16px;
  line-height: 24px;
  color: #646F73;
}

a {
font-family: SF Pro Text;
  font-size: 16px;
  line-height: 19px;
  color: #148077;
  font-weight: 700;
  text-decoration: none;
}
  </style>