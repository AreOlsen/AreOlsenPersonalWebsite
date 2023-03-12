<script>
    export let data;
</script>

<main class="grid gap-3 grid-cols-11 grid-rows-1">
    <div class="col-span-5 gap-2 flex-col flex justify-self-start self-start">
        <h1 class="text-4xl font-bold">Welcome to my blog.</h1>
        <p>
        Hello, and welcome to my blog!  I am thrilled to have the opportunity to share my thoughts and discoveries with you.
        As an avid computer science enthusiast, I have always been fascinated by the way technology is transforming our world. From the earliest days of computing to the latest advancements in artificial intelligence, I have been captivated by the power of technology to change the way we live, work, and interact with each other.
        My passion for technology began at a young age, when I first discovered the magic of coding. As I experimented with different programming languages and software development tools, I began to realize the limitless possibilities that technology offered. Whether it was designing websites, building mobile apps, or creating sophisticated algorithms, I was hooked on the thrill of creating something new and innovative.
        Over time, my interests in computer science have evolved and expanded. I have become increasingly interested in the intersection of technology with other fields, such as biology, physics, and economics. I believe that the integration of technology with these other areas of study has the potential to unlock new frontiers of knowledge and understanding.
        However, my interests are not limited to just computer science. I am a curious and introspective individual who loves to explore new ideas and delve into deep philosophical discussions. From questions of ethics and morality to the mysteries of the universe, I find myself drawn to a wide range of topics that challenge me to think deeply and critically.
        In creating this blog, my hope is to share my insights and experiences with others who share my passion for technology and intellectual curiosity. I plan to write about everything from the latest advancements in machine learning to the philosophy of mind and consciousness. Whether you are a fellow computer science enthusiast or simply someone who is curious about the world around us, I hope that my blog will inspire you to think deeply and explore new frontiers of knowledge and understanding.
        Finally, I believe that this blog will serve as a documentation of my journey as a computer science enthusiast and curious human being. I plan to share my experiences, challenges, and successes with my readers, as well as offer tips and advice for those who are interested in pursuing a similar path of self-improvement and discovery.
        Thank you for taking the time to read my blog, and I look forward to embarking on this exciting journey with you!
        </p>
    </div>
    <div class="divider divider-horizontal col-span-1" ></div>
    <div class="col-span-5 flex flex-col gap-2 justify-self-start self-start">
        <h1 class="text-4xl font-bold">Blog Index.</h1>
        <ul>
            {#each data.posts as post,i}
                <li>
                    <a href={post.path}>
                        <h2 class="font-bold text-lg">{post.meta.title}</h2>
                        <h3 class="italic">{post.meta.date}</h3>
                    </a>
                    <div class="divider"></div>
                </li>
            {/each}
        </ul>
    </div>
</main>