<style>
    :global(body),
    :global(html)
    :global(main) {
        display: block !important;
        height: auto !important;
        width: auto !important;
        position: static !important;
        margin: 0 !important;
        padding: 0 !important;
        overflow-x: hidden !important;
        font-family: 'Poppins', sans-serif !important;
    }

    :global(main) {
        word-break: normal;
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        height: 100vh;
        width: 100vw;
    }

    :global(::-webkit-scrollbar) {
        width: 0.5rem;
        height: 0.5rem;
    }

    :global(::-webkit-scrollbar-thumb) {
        border-radius: 3px;

        background-color: #ffffff40;
    }

    :global(::-webkit-scrollbar-thumb:hover) {
        background-color: #ffffff80
    }

    :global(.center-layout) {
        width: 100vw; padding: 3rem; padding-left: 0; padding-right: 0; text-align: center;
    }
</style>
<script lang="ts">
    import TopAppBar, { Row, Section, Title } from '@smui/top-app-bar';
</script>
<main>
    <TopAppBar variant="standard" dense>
        <Row>
            <Section align="start" toolbar>
                <Title>Welcome to My Portfolio.</Title>
            </Section>
        </Row>
    </TopAppBar>
    <div style="margin-top: 48px; padding: 48px">
        <slot />
    </div>
</main>