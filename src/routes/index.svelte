<script>
    let parties = ["LP", "NNPP", "PDP", "APC"]
    let votes = [4000000000, 3000000, 2000000, 1000000]
</script>
<div>
    <div class="flex justify-between items-center">
        <div class="text-2xl font-black text-gray-600">INEC</div>
        <div class="text-lg font-bold text-gray-500"><a href="/login">Login</a></div>
    </div>

    <div class="flex justify-between items-center mt-12 bg-green-50 p-4 rounded-lg">
        <div class="w-1/2 p-4">
            <h2 class="text-2xl text-green-800 font-black">Cast Your Vote</h2>
            <h5 class="text-lg text-right text-green-400 font-normal">Learn more</h5>
            <br>
            <a href="/login" class="block bg-green-800 text-md text-white rounded-lg text-center py-2 px-4 font-black">Start voting..</a>
        </div>
        <div class="w-1/2 text-green-500 bottom-0 right-0 flex justify-end items-bottom animate__animated animate__bounce">
            <img src="/vote.png" class="w-auto h-auto " alt="Vote" />
        </div>
    </div>

    <div class="flex justify-start space-x-6 items-center mt-12">
        <div class="bg-gray-600 text-lg text-white text-center rounded-lg py-1 px-6 font-normal">All</div>
        <div class="bg-transparent text-lg text-gray-400 text-center py-1 px-6 font-normal">Top 10</div>
        <div class="bg-transparent text-lg text-gray-400 text-center py-1 px-6 font-normal">Top 20</div>
    </div>
   
    <div class="flex justify-start space-x-6 items-center mt-12">
        <h3 class="text-xl font-normal text-gray-500">See live updates</h3>
    </div>

    <div class="flex justify-between items-center mt-12">
        <div class="bg-transparent text-lg text-gray-400 text-center py-1 px-6 font-normal">Parties</div>
        <div class="bg-transparent text-lg text-gray-400 text-center py-1 px-6 font-normal">Votes</div>
    </div>

    <div class="my-12 block"></div>

    {#each parties as party, index}

        <div class="animate__animated animate__pulse flex justify-between items-center mt-4 p-4 rounded-lg bg-stone-50">
            <div class="flex justify-start items-center space-x-4">
                <div><img src="/{party.toLowerCase()+".png"}" class="animate__animated animate__slideInRight w-12 h-12" alt="{party}"/></div>
                <div class="font-medium text-lg text-gray-600">{party}</div>
            </div>
            <div class="bg-transparent text-2xl text-gray-600 text-center py-1 px-6 font-black">
                {votes[index]}
            </div>
        </div>

    {/each}

</div>