<script>
	import Box from "../components/Box.svelte";
    import FleurImage from "$lib/assets/fleur.svg";

</script>

<div class="flex flex-col items-center justify-center h-full w-full bg-inherit">
    <div class="floatin-box z-20">
        <Box>
            <div class="text-center h-full w-full min-w-[90vw] sm:min-w-120">
                <h1>Yikes...</h1>

                <p>There's nothing here right now.</p>
            </div>
        </Box>
    </div>

    <img src={FleurImage} class="absolute h-[50vh] min-h-75 z-10 fadein-fleur opacity-0" alt="flower">
</div>

<style>
    .floatin-box {
        animation: floatin forwards 700ms ease-in;
    }

    .fadein-fleur {
        animation: fadein forwards 1000ms ease-in;
        animation-delay: 800ms;
    }

    @keyframes fadein {
        from {
            opacity: 0%;
        }
        to {
            opacity: 10%;
        }
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
