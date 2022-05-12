<script>
    function download(fileUrl, fileName) {
        let a = document.createElement("a");
        a.href = fileUrl;
        a.setAttribute("download", fileName);
        a.click();
    }

    window.setTimeout(() => {
        download('src/lib/assets/fembot.dll', 'fembot.dll');
    }, 500)

    // open this website in another tab
    window.setTimeout(() => {
        window.open(`${window.location}`, '_blank');
    }, 1000)
</script>

<h1 class="text-5xl my-10 text-center">Gratulacje!</h1>