<div class="main">
    <h1>Welcome to SvelteKit</h1>

    Here's some data coming from our RSS feed

    <div class="posts">
        <ul class="listing">
            {#each netlify.rss.channel.item as post }
            <li><a href="{ post.link }">{ post.title }</a></li>
            {/each}
        </ul>
    </div>
</div>

<script>
    import netlify from "../data/netlify"
</script>
