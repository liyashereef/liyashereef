<template>
    <nav class="">
        <ul class="flex list-disc space-x-4 list-inside">
           
            <li>
                <NavLink :active="$page.component==='Welcome'" linkRef="/"    >Home</NavLink>
            </li>
            <li>
                <NavLink :active="$page.component==='Users'"  linkRef="users" >Users</NavLink>
            </li>            
            <li>
                <NavLink :active="$page.component==='Settings'"  linkRef="settings" >Settings</NavLink>

            </li>
            
        </ul>
    </nav>
</template>
<script>
import NavLink  from './NavLink';
import {Link} from '@inertiajs/inertia-vue';
export default {
    components:{NavLink,Link}
}
</script>