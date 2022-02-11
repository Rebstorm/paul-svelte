<script lang="ts">
    import { Route, Router} from "svelte-navigator";
    import Root from "./routes/root/Root.svelte";
    import Tech from "./routes/tech/Tech.svelte";
</script>

<div class="container">
<Router>
    <div>
        <Route path="" component="{Root}" />
        <Route path="tech" component="{Tech}" />
    </div>
</Router>
</div>
<style>
    .container {
        width: 100%;
    }
</style>