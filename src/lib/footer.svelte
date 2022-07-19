<script lang="ts">
    const tools = [
        {
            tool: "svelte",
            woodmark: false
        },
        {
            tool: "jamstack",
            woodmark: false
        },
        {
            tool: "javascript",
            woodmark: false
        },
        {
            tool: "vscode",
            woodmark: false
        },
        {
            tool: "typescript",
            woodmark: false
        },
        {
            tool: "html5",
            woodmark: false
        },
        {
            tool: "css3",
            woodmark: false
        },
        {
            tool: "git",
            woodmark: false
        },
        {
            tool: "github",
            woodmark: false
        },
        {
            tool: "windows8",
            woodmark: false
        }
    ]

</script>

<footer>
    <h3>This site was built & deployed using:</h3>
    <div class="container">
        {#each tools as {tool, woodmark}}
                <i class={`${woodmark ? `devicon-${tool}-plain-woodmark` : `devicon-${tool}-plain`}`} title={tool} alt={tool} />
        {/each}
    </div>
</footer>

<style>
    footer {
        padding: 2rem 0;
        text-align: center;
    }
    .container {
        margin: 1rem auto;
    }
    i {
        font-size: 2rem;
    }
</style>