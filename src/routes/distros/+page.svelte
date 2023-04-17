<script lang="ts">
	import { enhance } from '$app/forms';

</script>

<svelte:head>
	<title>Distros</title>
	<meta name="description" content="Linux distros rated." />
</svelte:head>

<div>
    <h1>Linux Distros Rated by Tiers</h1>
    <div>         
        <form
            method="POST"
            action="?/enter"
            use:enhance={() => {
                // prevent default callback from resetting the form
                return ({ update }) => {
                    update({ reset: false });
                };
            }}
        >
    </div>


</div>
