<div class="main">
    <Header />
    <div class="wrapper">
        <div class="tags">
            <SideNave />
        </div>
        <div class="feed">
            <div class="searchbar">
                <form class="searchform">
                    <!-- <i class="fa fa-user icon"></i> -->
                    <input class="form-input" type="text" placeholder="Search">
                </form>
            </div>
            <div>
                {#each data as post }
                    <FeedCards post={post} />
                {/each}
            </div>
        </div>
        <div class="ads">
        </div>
    </div>
    <!-- <div class="posts">
            {#each netlify.rss.channel.item as post }
            <li><a href="{ post.link }">{ post.title }</a></li>
            {/each}
    </div> -->
    <AppFooter />
</div>

<script>
    import netlify from "../data/netlify"
    import Header from "../components/Header.svelte";
    import FeedCards from "../components/FeedCards.svelte";
    import AppFooter from "../components/AppFooter.svelte";
    import SideNave from "../components/SideNav.svelte";
    

    const data = [
        {
            title: "Resource Title",
            description: "Roof party fashion axe mumblecore, readymade keytar fixie vegan McSweeney's kitsch salvia you probably haven't heard of them pickled messenger bag. Whatever Wes Anderson forage, skateboard ethnic 90's chia Bushwick iPhone.",
            author: "Ekene Eze",
            date: "2020-01-01",
        },
        {
            title: "Resource Title",
            description: "Roof party fashion axe mumblecore, readymade keytar fixie vegan McSweeney's kitsch salvia you probably haven't heard of them pickled messenger bag. Whatever Wes Anderson forage, skateboard ethnic 90's chia Bushwick iPhone.",
            author: "Ekene Eze",
            date: "2020-01-01",
        },
        {
            title: "Resource Title",
            description: "Roof party fashion axe mumblecore, readymade keytar fixie vegan McSweeney's kitsch salvia you probably haven't heard of them pickled messenger bag. Whatever Wes Anderson forage, skateboard ethnic 90's chia Bushwick iPhone.",
            author: "Ekene Eze",
            date: "2020-01-01",
        },
        {
            title: "Resource Title",
            description: "Roof party fashion axe mumblecore, readymade keytar fixie vegan McSweeney's kitsch salvia you probably haven't heard of them pickled messenger bag. Whatever Wes Anderson forage, skateboard ethnic 90's chia Bushwick iPhone.",
            author: "Ekene Eze",
            date: "2020-01-01",
        }
    ]
</script>

<style>
    .searchform {
        display: flex;
    }
    .form-input {
        width: 100%;
        height: 51px;
        border-radius: 6px;
        margin-top: 24px;
        border: 2px solid #E9EAEB;
    }
    .form-input::placeholder{
        font-family: SF Pro Text;
        font-weight: normal;
        padding: 8px;
    }
    .wrapper {
        display: grid;
        grid-template-columns: 1fr 2fr 1fr;
        gap: 2em;
        grid-auto-rows: minmax(300px, auto);
    }
    .tags {
        background-color: rgb(187, 36, 36);
    }
    .feed {
        margin-bottom: 30px;
        width: 100%;
    }
    .ads {
        background-color: orange;
    }
</style>