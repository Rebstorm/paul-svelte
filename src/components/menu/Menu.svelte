<script lang="ts">
    import { useNavigate } from "svelte-navigator";
    const navigate = useNavigate();
    const handleNavigation = (route: string) => {
        navigate(route)
    }
</script>


<div class="menu-container">
    <div on:click={() => handleNavigation('/')}>Home</div>
    <div on:click={() => handleNavigation('tech')}>Stuff I do</div>
    <div on:click={() => handleNavigation('more-stuff')} >Other stuff</div>
    <div on:click={() => handleNavigation('more-more-stuff')} >More stuff</div>
</div>

<style >
    .menu-container {
        background: #fff;
        box-shadow: 2px 2px 2px 0px rgba(50, 50, 50, 0.75);
        display: grid;
        grid-template-columns: repeat(4, 1fr);
        gap: 1rem;
        color: #000;
    }

</style>