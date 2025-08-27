<script>
    // @ts-nocheck

    import Form from "./Form.svelte";

    let classVariable = ""
    export {classVariable as class}

    async function handle(data)
    {
        await fetch(`https://docs.google.com/forms/d/e/1FAIpQLSerFF_37h5-xhDUla7lOmQPnLJmnZa-UxZTuIdpPbWufk_DYA/formResponse?usp=pp_url&entry.1640907474=${data.firstname || "blank"}&entry.1618305576=${data.lastname || "blank"}&entry.1253263446=${data.email || "blank"}&entry.887760246=${data.phone || "blank"}&submit=Submit`,
            {
                method: "GET",
                headers: {
                    "Content-Type": "application/x-www-form-urlencoded"
                },
                mode: "no-cors"
            }
        )

        alert("Form Submitted")
    }
</script>

<Form class={classVariable} {handle}>
    <slot/>
</Form>