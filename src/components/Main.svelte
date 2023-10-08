<script>
     import Step from "./Step.svelte";

    let steps = [
        {
            name: "Blogging Website",
            icon: "fa-solid fa-blog",
            description:
                "A place where you can anonymously put out your blogs ",
        },
        {
            name: "Utlimate Todos",
            icon: "fa-solid fa-list-check",
            description:
                "Test for model robustness with customized test profiles and receive exhaustive reporting on the performance and potential vulnerabilities of your model.",
        },
        {
            name: "Library",
            icon: "fa-solid fa-book-atlas",
            description:
                "A place where students can store their notes and study material without any raucous."
        },
    ];

    let benefits = [
        {
            metric: "10x",
            name: "a self taught developer",
            description:
                "I taught myself to code using free online resources and absolutely fell in love with the creativity and problem solving that is involved in developing and engineering innovative new online experiences. Starting of with JavaScript, HTML & CSS and evolving my knowledge base to include JavaScript frameworks, backend programming, design,and much much more.",
        },
        {
            name: "a UI & UX designer",
            description:
                "Carefully crafting and designing amazing user experiences allows me to express and experiment with every morsel of creativity I have. I love the challenge of learning new design concepts and enabling users with amazing online experiences.",
        },
        {
            name: "an Explorer",
            description:
                "It intrigues me that while I am in the process of learning things I keep on exploring new fields that aren't even related to what I have to do at that point of time . I love to explore new tech. related things as much as I love travelling."
        },
    ];
</script>

<main class="flex flex-col flex-1 p-4">
    <section id="introPage" class="grid grid-cols-1 lg:grid-cols-2 gap-10 py-8 sm:py-14 ">
        <div class="flex flex-col lg:justify-center text-center lg:text-left gap-6 md:gap-8 lg:gap-10">
            <h2 class="font-semibold text-4xl sm:text-5xl md:text-6xl">
                Hi! I'm <span class = "nunito text-violet-400">Rishabh </span>Sharma 
                <br/>Midway of becoming a <span class = "nunito text-violet-400">Full Stack Developer</span>
            </h2>
            <p class="text-base sm:text-lg md:text-xl">
                <span class = "nunito text-violet-400">Skill Set</span><br/>
                <span class = "nunito text-pink-300">Programming Language :</span> Java , JavaScript , Python ,  HTML , Vanilla CSS <br/>
                <span class = "nunito text-pink-300">Design :</span> Figma <br/>
                <span class = "nunito text-pink-300">Framework :</span> NodeJS <br/>
                <span class = "nunito text-pink-300">Currently Learning :</span> C , MERN Stack , TailwindCSS
            </p>
            <a                
                class="blueShadow mx-auto lg:mr-auto lg:ml-0 text-base sm:text-lg md:text-xl poppins relative overflow-hidden px-6 py-3 group rounded-full bg-white text-slate-950 cursor-pointer" href="https://www.instagram.com/rishu.aex/" target="_blank"
            >
                <div
                    class="absolute top-0 right-full w-full h-full bg-violet-400 opacity-20 group-hover:translate-x-full z-0 duration-200"
                />
                <h4 class="relative z-9">Get in touch &rarr;</h4>
            </a>
        </div>
        <div class="relative shadow-2xl grid place-items-center">
            <img
            src={"images/Profilepic.png"}
            alt="Zetane Engine"
            class="object-cover z-[2] max-h-[70vh]"
        />

    </section>


    <section id="projects" class="py-20 lg:py-32 flex flex-col gap-24">
        <div class="flex flex-col gap-2 text-center">
            <h6 class="text-large sm:text-xl md:text-2xl">
                A few of my creative endeavors.
            </h6>
            <h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">
                I may <span class="nunito text-violet-400">develop</span> in near future !!
            </h3>
        </div>
        <a
            href="https://www.youtube.com/watch?v=dQw4w9WgXcQ"
            target="_blank"
            class="mx-auto px-4 py-2 rounded-md border border-solid border-white flex items-center gap-2 -mb-4 sm:-mb-0 -mt-10 hover:border-violet-700 duration-200"
        >
            <i class="fa-regular fa-circle-play" />
            <p>Watch the video</p>
        </a>
        <div class="grid grid-cols-1 lg:grid-cols-3 gap-12 lg:gap-10">
            <Step step={steps[0]}>
                <p>
                    Currently analysing what features to add
                    and how can our website can stand out from the crowd.The <strong
                    class="text-violet-400">first concern will be the 
                    users privacy</strong> how you can navigate throughout the website anonymously.
                </p>
            </Step>
            <Step step={steps[1]}>
                <p>
                    Ultimate Todos using <strong
                        class="text-violet-400">Next.js</strong
                    >,
                    <strong class="text-violet-400">Node.js + Express.js</strong
                    >
                    that allows a user to login, manage a tidy and efficacious todo
                    list, and persist this information across devices.
                </p>
            </Step>
            <Step step={steps[2]}>
                <p>
                    Library is going to be wonderfull place
                    where you will be able to store your notes & study material included with
                    <strong class="text-violet-400">In-built Web Player</strong> where you can
                    listen to your <strong class="text-violet-400">favourite songs and podcasts</strong> while working.
                    
                </p>
            </Step>
        </div>
    </section>

    <section  id="about" class="py-20 pt-10 lg:pt-16 lg:py-32 flex flex-col gap-16 sm:gap-20 md:gap-24 relative">
        <div class="flex flex-col gap-2 text-center relative before:absolute 
            before:top-0 before:left-0 before:w-2/3 before:h-1.5 before:bg-violet-700 
            after:absolute after:bottom-0 after:right-0 after:w-2/3 after:h-1.5 after:bg-violet-700 py-4">

            <h6 class="text-large sm:text-xl md:text-2xl">
                Want to know more?
            </h6>
            <h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">
                A bit <span class="poppins text-violet-400">about</span> me.
            </h3>
        </div>
        <p class="mx-auto nunito font-semibold text-lg sm:text-xl md:text-2xl">
            I am . . .
        </p>
        <div class="flex flex-col gap-20 w-full mx-auto max-w-[800px]">
            {#each benefits as benefit, index}
            <div class="flex gap-6 sm:gap-8">
                <p
                    class="nunito text-4xl sm:text-5xl md:text-6xl text-slate-500 font-semibold"
                >
                    0{index + 1}
                </p>
                <div class="flex flex-col gap-6 sm:gap-8">
                    <h3 class="text-2xl sm:text-3xl md:text-5xl">
                        {benefit.name}
                    </h3>
                    <p>{benefit.description}</p>
                </div>
            </div>
        {/each}
    </div>
    <h5 class={" text-2xl sm:text-3xl font-semibold text-center poppins "}>
        The <span class="text-violet-400">Complete</span> Package
    </h5>
    <div
        class="flex flex-col overflow-x-scroll gap-10 max-w-[800px] mx-auto w-full"
    >
        <table class="bg-white text-slate-700 rounded text-center">
            <thead class={"border-b border-solid border-slate-200  "}>
                <tr class="">
                    <th />
                    <th class="whitespace-nowrap p-2 px-4">Candidate #1</th>
                    <th class="whitespace-nowrap p-2 px-4">Candidate #2</th>
                    <th class="whitespace-nowrap p-2 px-4">Candidate #3</th>
                    <th
                        class="bg-violet-700 text-white whitespace-nowrap p-4 px-8"
                        >Me</th
                    >
                </tr>
            </thead>
            <tbody>
                <tr class="border-b border-solid border-slate-200">
                    <td
                        class="border-r border-solid border-white pl-4 pr-8 py-4 font-semibold text-sm"
                        >Dedication</td
                    >
                    <td><i class="fa-solid fa-xmark text-slate-500" /></td>
                    <td><i class="fa-solid fa-check text-slate-500" /></td>
                    <td><i class="fa-solid fa-xmark text-slate-500" /></td>
                    <td><i class="fa-solid fa-check text-green-500" /></td>
                </tr>
                <tr class="border-b border-solid border-slate-200">
                    <td
                        class="border-r border-solid border-white pl-4 pr-8 py-4 font-semibold text-sm"
                        >Critical Thought</td
                    >
                    <td><i class="fa-solid fa-xmark text-slate-500" /></td>
                    <td><i class="fa-solid fa-check text-slate-500" /></td>
                    <td><i class="fa-solid fa-check text-slate-500" /></td>
                    <td><i class="fa-solid fa-check text-green-500" /></td>
                </tr>
                <tr>
                    <td
                        class="border-r border-solid border-white pl-4 pr-8 py-4 font-semibold text-sm"
                        >Interpersonal Skills</td
                    >
                    <td><i class="fa-solid fa-check text-slate-500" /></td>
                    <td><i class="fa-solid fa-check text-slate-500" /></td>
                    <td><i class="fa-solid fa-xmark text-slate-500" /></td>
                    <td><i class="fa-solid fa-check text-green-500" /></td>
                </tr>
                <tr class="border-t border-solid border-slate-200">
                    <td
                        class="border-r border-solid border-white pl-4 pr-8 py-4 font-semibold text-sm"
                        >Progamming Ability</td
                    >
                    <td><i class="fa-solid fa-check text-slate-500" /></td>
                    <td><i class="fa-solid fa-xmark text-slate-500" /></td>
                    <td><i class="fa-solid fa-check text-slate-500" /></td>
                    <td><i class="fa-solid fa-check text-green-500" /></td>
                </tr>
            </tbody>
        </table>
    </div>
    <div class="mx-auto -mt-12 italic sm:hidden opacity-50">
        <p>Scroll to see more &rarr;</p>
    </div>
    <p class="mx-auto">So why not invest?</p>

    </section>
</main>