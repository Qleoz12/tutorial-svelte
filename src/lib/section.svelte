<script>
    export let titulo;
</script>

<section>
    <header>
        <slot name="header">
            <h1>{titulo}</h1>
        </slot>
    </header>
    <slot name="main">
        <p>default message</p>
    </slot>
</section>
