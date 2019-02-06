<template>
    <nav>
        <ul>
            <li>
                <router-link to="/">AboutMe</router-link>
            </li>
            <li>
                <router-link to="/about">jobs</router-link>
            </li>
            <li>
                <router-link to="/works">Works</router-link>
            </li>
            <li>
                <router-link to="/contact">Contact</router-link>
            </li>
        </ul>
    </nav>
</template>

<style>
ul{
    list-style: none;
}
li{
    display: inline;
    margin: 0 20px;
}
a{
        text-decoration: none;
        color: black;
}
a:hover{
    color: rgb(255, 81, 0);
}

</style>
