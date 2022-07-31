<script>
	let parties = ['LP', 'NNPP', 'PDP', 'APC'];
	let first = ['Peter Obi', 'Kwankaso Rabiu', 'Atiku Abubakar', 'Asiwaju Tinubu'];
</script>

<div>
	<div class="">
		<h1 class=" text-2xl font-black text-left text-gray-600 mt-4 mb-6">Presidential Election</h1>
		<div class="animate__animated animate__tada bg-green-600 rounded-md p-4 mb-12 flex justify-start items-center space-x-4">
			<div class="w-full text-white">
				<div class="text-white text-xl font-bold">Vote ends in 6hrs 30mins</div>
				<div class="text-white text-md font-normal">Vote ends by Aug 1st 2022</div>
			</div>
			<div class="w-4 flex justify-end items-center">
				<i class="fal fa-x text-white" />
			</div>
		</div>
		<h1 class="text-2xl font-bold text-left text-gray-600 mt-12 mb-6">Presidential Aspirants</h1>

		<div class="my-12 block" />

		{#each parties as party, index}
			<div class="animate__animated animate__slideInUp flex justify-start items-center mt-4 bg-white">
				<div class="flex justify-start items-center space-x-4 w-20 h-20 p-4">
					<div><img src="/{party.toLowerCase() + '.png'}" class="w-full h-full" alt={party} /></div>
				</div>
				<div class="bg-stone-100 w-full p-2 flex justify-center items-center space-x-4">
                    <div class="w-full">
                        <div class="font-bold text-2xl text-gray-600">{party}</div>
                        <div class="font-medium text-lg text-gray-600">{first[index]}</div>
                    </div>
                    <div class="w-20 flex justify-end items-center">
                        <div class="p-4"><a href="/ballot" class="block bg-green-600 text-md text-white rounded-lg text-center py-2 px-4 font-black">VOTE</a>  </div>                      
                    </div>
				</div>
			</div>
		{/each}
	</div>
</div>
