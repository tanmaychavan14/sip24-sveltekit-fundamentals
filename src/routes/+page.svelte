
<script>
    export let data;
</script>
<header class ="bg-white py-4 shadow-md" >
    <div class="container mx-auto px-4 flex justify-between items-center">
        <h1 class="text-2xl font-bold font-['Comic_Sans_MS']">InstaClone</h1>
            <a href="/add-post" class="bg-red-500 hover:bg-red-700 text-white font-bold py-2 px-4 rounded-md">Add Post</a>

        
    </div>
</header>
<div class="container mx-auto md:my-5">
    <div class="grid grid-cols-1 md:grid-cols-3 gap-4">
        {#each data.posts as post}
<div>
    <img class="w-full" src="data:image;base64,{post.image}" alt="post">
    <div class ="text-5m py-2">
<span class="font-bold">
{post.username}
</span>
<span class="text-gray-700">{post.content}</span>
    </div>
</div>
{/each}
    </div>

</div>