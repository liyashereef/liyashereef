
<template>
<div>
<section class="p-6  bg-gray-200">
    <header class="flex justify-between">
        <div class="flex item-center">
            <h1 class="font-bold text-lg">My App</h1>
            <p class="text-sm ml-4">
                Welcome back , {{$page.props.auth.user.username}}
            </p>            
        </div>

        <Nav/>
    </header>
    
    
</section>
<section class="p-6">
    <div class="max-w-4xl mx-auto">
        <slot/>
    </div>
</section>
</div>
</template>

<script>
import Nav from "./Nav";
export default {
    components:{Nav}
}
</script>

<style>

</style>