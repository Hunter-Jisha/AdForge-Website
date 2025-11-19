<script>
    import Navbar from "$lib/Navbar.svelte";
    import Arrow from "$lib/icons/Arrow.svelte";
    import Signal from "$lib/icons/Signal.svelte";
    import Globe from "$lib/icons/Globe.svelte";
    import Instagram from "$lib/icons/Instagram.svelte";
    import Quote from "$lib/icons/Quote.svelte";
    import Form from "$lib/Form.svelte";
    import ArrowDiagonal from "$lib/icons/ArrowDiagonal.svelte";
    import Profile from "$lib/icons/Profile.svelte";
    import Briefcase from "$lib/icons/Briefcase.svelte";
    import Robot from "$lib/icons/Robot.svelte";
    import GoogleFormWrapper from "$lib/GoogleFormWrapper.svelte";

</script>

<Navbar/>

<div class="w-full md:h-[55rem] relative flex flex-col flex-shrink-0 pt-24 p-8 gap-16">

    <img class="w-full h-full object-cover absolute top-0 left-0" alt="background" src="services_background.jpg">

    <div class="md:absolute mt-auto left-16 top-32 flex flex-col text-white gap-4 drop-shadow-md" style="text-shadow: 0px 0px 20px #000a;">
        <p class="text-xl">OUR SERVICES</p>
        <p class="font-fancy text-5xl md:text-8xl">From Hands-Free <br> To White-Glove  </p>
        <p class="text-xl md:text-2xl md:w-2/3">
            We build brand loyalty through <br>personalized customer experiences. <br>Growth is just a side-effect.
        </p>

        <button on:click={() => document.getElementById("services")?.scrollIntoView({ behavior: "smooth" })} 
        class="px-16 py-4 text-xl bg-white text-gray-700 w-min font-bold hover:bg-gray-200 transition-all">Continue</button>
    </div>
</div>

<div id="services" class="w-full relative flex flex-col bg-blue-400 flex-shrink-0 items-center p-8 md:px-48 gap-16">
    <p class="font-fancy text-6xl text-white text-center">Packages</p>

    <div class="w-full h-full gap-8 grid grid-rows-2 grid-cols-2 text-white">

        <div id="onboarding" class="flex flex-col row-span-1 col-span-2 items-start gap-12 bg-gray-700 text-gray-500 p-12">
            <div class="w-20 h-20 aspect-square p-2  bg-white text-gray-700">
                <Signal/>
            </div>
            <div class="w-full flex flex-col gap-4">
                <p class="font-fancy text-5xl text-white">Onboarding Package</p>
                <p class="text-xl md:text-3xl text-gray-400 center-text">
                    Branding | Web Design | Logos | Analysis
                </p> 
                <p class="text-2xl md:text-3xl text-gray-300">
                    Includes a full static website redesign, branding consultation, logo redesign, a KPI baseline report*, an analytics/pixel/tracking audit, a SWOT analysis, a marketing strategy, competitor and customer analyses, and checkout funnel / UX analysis*.
                </p>
                <!--<ul class="list-disc text-2xl md:text-3xl text-gray-300 columns-1 md:columns-2 [column-fill:_balance] space-y-2 pl-8">
                    <li>Full Static Website Redesign</li>
                    <li>Branding Consultation</li>
                    <li>Logo Redesign</li>
                    <li>KPI Baseline Report*</li>
                    <li>Analytics, Pixel, and Tracking Audit</li>
                    <li>SWOT Analysis</li>
                    <li>Marketing Strategy Report</li>
                    <li>Competitor Analysis</li>
                    <li>Customer Analysis</li>
                    <li>Checkout Funnel &amp; UX Analysis*</li>
                </ul>-->
            </div>
        </div>

        <div id="good" class="flex flex-col row-span-1 col-span-2 items-start gap-12 bg-gray-700 text-gray-500 p-12">
            <div class="w-20 h-20 aspect-square p-2 bg-white text-gray-700 md:ml-auto">
                <Instagram/>
            </div>
            <div class="w-full flex flex-col gap-4 items-end text-right">
                <p class="font-fancy text-5xl text-white">Bronze Package</p>
                <p class="text-xl md:text-3xl text-gray-400">
                    Social Media Autopilot | Review Management | Web Hosting
                </p>
                <p class="text-2xl md:text-3xl text-gray-300 max-w-prose">
                    Includes regular static social media posts, SEO optimization, website hosting, Google/Yelp review management, comment management, and weekly reports.
                </p>
                <!--<ul class="list-disc text-2xl md:text-3xl text-gray-300 columns-1 md:columns-2 [column-fill:_balance] space-y-2 pl-8">
                    <li>Regular, static social media posts</li>
                    <li>SEO Optimization</li>
                    <li>Website Hosting</li>
                    <li>Google/Yelp Review Management</li>
                    <li>Comment Management</li>
                    <li>Weekly Analytics Summaries</li>
                </ul>-->
            </div>
        </div>

        <div id="better" class="flex flex-col row-span-1 col-span-2 items-start gap-12 bg-gray-700 text-gray-500 p-12">
            <div class="w-20 h-20 aspect-square p-2 bg-white text-gray-700">
                <Globe/>
            </div>
            <div class="w-full flex flex-col gap-4">
                <p class="font-fancy text-5xl text-white">Silver Package</p>
                <p class="text-xl md:text-3xl text-gray-400 center-text">
                    Email | A/B Testing | Analytics | Photography
                </p>
                <p class="text-2xl md:text-3xl text-gray-300">
                    Includes all perks of the Bronze package, plus personalized analytics, a monthly photography session, email marketing campaigns including drip campaigns, <br>website A/B testing, checkout flow analysis, and a monthly strategy meeting.
                </p>
                <!--<ul class="list-disc text-2xl md:text-3xl text-gray-300 columns-1 md:columns-2 [column-fill:_balance] space-y-2 pl-8">
                    <li>All perks of Bronze package</li>
                    <li>Personalized Analytics</li>
                    <li>Monthly Photography Session</li>
                    <li>Email Marketing Campaigns</li>
                    <li>Website A/B Testing</li>
                    <li>Checkout Flow Analysis</li>
                    <li>Monthly Strategy Meeting</li>
                </ul>-->
            </div>
        </div>

        <div id="best" class="flex flex-col row-span-1 col-span-2 items-start gap-12 bg-gray-700 text-gray-500 p-12">
            <div class="w-20 h-20 aspect-square p-2  bg-white text-gray-700 md:ml-auto">
                <Briefcase/>
            </div>
            <div class="w-full flex flex-col gap-4 items-end text-right">
                <p class="font-fancy text-5xl text-white">Gold Package</p>
                <p class="text-xl md:text-3xl text-gray-400">
                    Personalized Storytelling | On-Site Partners | Engagement Growth
                </p>
                <p class="text-2xl md:text-3xl text-gray-300 max-w-prose">
                    Includes all perks of the Silver package, plus weekly on-site photo/video coverage with your dedicated content manager, personalized storytelling, customized trending videos, behind-the-scenes content with cameos and short biographies, and event curation.
                </p>
                <!--<ul class="list-disc text-2xl md:text-3xl text-gray-300 columns-1 md:columns-2 [column-fill:_balance] space-y-2 pl-8">
                    <li>All perks of Silver package</li>
                    <li>Photographer/Videographer On-Site Weekly</li>
                    <li>Personalized Storytelling</li>
                    <li>Customized Trending Videos</li>
                    <li>Behind-the-Scenes / Cameos / Biographies</li>
                    <li>Event Curation</li>
                </ul>-->
            </div>
        </div>

        <div id="a-la-carte" class="flex flex-col row-span-1 col-span-2 items-start gap-12 bg-gray-700 text-gray-500 p-12">
            <div class="w-20 h-20 aspect-square p-2  bg-white text-gray-700">
                <Robot/>
            </div>
            <div class="w-full flex flex-col gap-4">
                <p class="font-fancy text-5xl text-white">A La Carte</p>
                <ul class="list-disc text-2xl md:text-3xl text-gray-300 columns-1 md:columns-2 [column-gap:3rem] [column-fill:_balance] space-y-2 pl-8 mx-auto">
                    <li>AI Consulting</li>
                    <li>Brand Consulting</li>
                    <li>Analytics / Reports</li>
                    <li>Photo Shoots</li>
                    <li>2D / 3D Videos</li>
                    <li>Paid Ad Campaigns</li>
                    <li>Website Redesigns</li>
                    <li>SEO Optimization</li>
                </ul>
            </div>
        </div>

    </div>
</div>

<div id="get-started" class="w-full relative flex flex-col bg-gray-700 flex-shrink-0 items-center pt-32 pb-96 px-16 md:px-48 gap-16 text-white">
    <p class="text-center md:text-left font-fancy text-6xl">Ready To Go?</p>

    <div class="flex flex-col md:flex-row w-full gap-32 md:gap-96">
        <div class="w-full flex flex-col gap-8">
            <div class="flex flex-col gap-2">
                <p class="text-4xl font-fancy">Let's do it</p>
                <p class="text-md text-gray-400">Tell us a bit about yourself and <br> we'll take it from here</p>
            </div>
    
            <GoogleFormWrapper class="w-full flex flex-col gap-4">
                <div class="w-full flex flex-row gap-4 h-14">
                    <input class="w-full h-full px-4 font-bold bg-gray-500 text-white focus:text-gray-800 focus:bg-white transition-all" type="text" name="firstname" placeholder="First Name"/>
                    <input class="w-full h-full px-4 font-bold bg-gray-500 text-white focus:text-gray-800 focus:bg-white transition-all" type="text" name="lastname" placeholder="Last Name"/>
                </div>

                <input class="w-full h-14 px-4 font-bold bg-gray-500 text-white focus:text-gray-800 focus:bg-white transition-all" name="email" type="email" placeholder="Email"/>
                <input class="w-full h-14 px-4 font-bold bg-gray-500 text-white focus:text-gray-800 focus:bg-white transition-all" name="phone" type="number" placeholder="Phone"/>

                <input class="w-full h-14 px-4 font-bold text-white bg-gray-500 transition-all text-lg" type="submit" value="SUBMIT"/>

            </GoogleFormWrapper>
        </div>

        <div class="w-full flex flex-col gap-12">
            <div class="flex flex-col gap-2">
                <p class="text-4xl font-fancy">Not Quite</p>
                <p class="text-md text-gray-400">Schedule a discovery session — let's work together to 
                    uncover what obstacles your business is facing
                </p>
            </div>
            
            <div class="w-full flex flex-col gap-2">
                <a href="/" class="flex w-full flex-row items-center justify-between h-14 pl-6 bg-gray-500 hover:bg-blue-400 transition-all text-white font-bold">
                    <p class="whitespace-nowrap">Home</p>
                    <ArrowDiagonal class="h-full aspect-square p-4"/>
				</a>

                <a href="/about" class="flex w-full flex-row items-center justify-between h-14 pl-6 bg-gray-500 hover:bg-blue-400 transition-all text-white font-bold">
                    <p class="whitespace-nowrap">About Us</p>
                    <ArrowDiagonal class="h-full aspect-square p-4"/>
				</a>
            </div>
        </div>
    </div>
</div>