<script>
	import Box from "../components/Box.svelte";

</script>

<div class="flex flex-col items-center justify-center h-full w-full bg-inherit">
    <div class="floatin-box">
        <Box>
            <div class="text-center h-full w-full min-w-120">
                <h1>Yikes...</h1>

                <p>There's nothing here right now.</p>
            </div>
        </Box>
    </div>
</div>

<style>
    .floatin-box {
        animation: floatin forwards 700ms ease-in;
    }

    @keyframes floatin {
        from {
            opacity: 0%;
            transform: translateY(1rem);
        }
        to {
            opacity: 100%;
            transform: translateY(0rem);
        }
    }
</style>
