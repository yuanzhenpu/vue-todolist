<template>
    <footer class="footer">
        <p>待完成：{{$store.getters.getToDo.length}}件</p>
        <p>已完成：{{$store.getters.getDone.length}}件</p>
        <p>已取消：{{$store.getters.getCancel.length}}件</p>
        <p>共  计：{{$store.state.event.event.length}}件</p>
    </footer>
</template>

<style>
    .footer{
        position: fixed;
        bottom: 0;
        width: 100%;
        /* height: 50px; */
        line-height: 50px;
        background: #f8f8f8;
        text-align: center;
        font-size: 14px;
        color: #666;
        border-top: 1px solid #ddd;
    }
    .footer a{
        color: #666;
    }
</style>