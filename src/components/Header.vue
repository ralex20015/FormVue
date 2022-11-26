<template>
    <header>
        <nav>
            <h2><a href="#">Logo</a></h2>
            <ul>
                <li><a href="#">Home</a></li>
                <li><a href="#">About</a></li>
                <li><a href="#">Contact</a></li>
            </ul>
        </nav>
    </header>
</template>

<style>
*{
    box-sizing: border-box;
    margin: 0;
    padding: 0;
}

header nav{
    background-color: #efefef;
    color: #000;
    margin-bottom: 10px;
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    padding: 0.5rem;
}

header nav h2 a{
    text-decoration: none;
    color: #000;
}

header nav ul{
    display: flex;
    flex-direction: row;
    justify-content: space-around;
    align-items: center;
    list-style: none;
}

header nav ul li{
    margin-left: 1rem;
}

header nav ul li a{
    text-decoration: none;
    color: #000;
}

header nav ul li a:hover{
    border-bottom: 3px solid #0f4f0f;
}
</style>