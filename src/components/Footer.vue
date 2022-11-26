<template>
    <footer>
        <div>
            <ul>
                <li><a href="#"><img src="../assets/facebook.png"></a></li>
                <li><a href="#"><img src="../assets/instagram.png"></a></li>
                <li><a href="#"><img src="../assets/twitter.png"></a></li>
            </ul>
        </div>
        <div>
            <p>Vue Form ©️ Todos los derechos reservados</p>
        </div>
    </footer>
</template>

<style>
footer{
    position: absolute;
    bottom: 0;
    padding: 10px;
    justify-content: center;
    color: #000;
    background-color: #efefef;
    width: 100%;
}

footer ul{
    width: 50%;
    list-style: none;
    display: flex;
    flex-direction: row;
    justify-content: space-evenly;
    align-items: center;
    padding: auto;
    margin: auto;
}

footer p{
    text-align: center;
}

footer img{
    width: 32px;
    height: 32px;
}
</style>