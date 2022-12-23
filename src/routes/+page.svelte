<svelte:head>
    <div class="navBar">
        <ul>
            <div class="navBar_logo">
                <a href="/">
                    <img src="/src/images/AniPlay.png" alt="logo" />
                    <h1>AniPlay</h1>
                </a>
            </div>
            <li><a href="/anime">Anime</a></li>
            <li><a href="/manga">Manga</a></li>
        </ul>
    </div>
    <style>
        h1 {
            color: #e3e3e3;
        }
        p {
            color: #e3e3e3;
        }
        a {
            color: #95c4e3;
        }
        ul {
            list-style-type: none;
            margin: 0;
            padding: 0;
            overflow: hidden;
            background-color: #000;
            position: fixed;
            top: 0;
            width: 100%;
        }

        li {
            float: left;
        }

        li a {
            display: block;
            color: white;
            text-align: center;
            padding: 14px 16px;
            text-decoration: none;
        }

        li a:hover:not(.active) {
            background-color: #111;
        }

        .active {
            background-color: #04AA6D;
        }

        .navBar {
            padding: 0px 0px;
            background-color: #000;
            position: fixed;
            top: 0;
            width: 100%;
        }
        
        .navBar_logo a img {
            float: left;
            padding: 14px 20px;
            height: 50px;
            width: 50px;
        }

        .navBar_logo a h1 {
            float: left;
            padding: 14px 0px;
            font-size: 20px;
        }

    </style>
</svelte:head>





<br>
<br>
<h1>Welcome to SvelteKit</h1>