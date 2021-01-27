<script>
    import { stores } from "@sapper/app";
    const { page } = stores();
    $: {
        if (typeof gtag !== "undefined") {
            gtag("config", "UA-112478975-2", {
                page_path: $page.path,
            });
        }
    }
</script>
