<template>
    <div>
        <h1>Hello World</h1>
        <div>
            <nav>
                <router-link to="/">Home</router-link>&nbsp; |
                <router-link to="/about">About</router-link>
            </nav>
        </div>
        <router-view></router-view>
    </div>
</template>

