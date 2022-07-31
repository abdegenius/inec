<script>
</script>
<div>
    <div class="">
        <div class="w-12 h-12 bg-stone-200 text-center flex justify-center items-center rounded-full">
            <a href="/login"><i class="fa fa-arrow-left text-2xl font-black text-gray-600 block"></i></a>
        </div>
        <h1 class="text-4xl font-black text-left text-gray-600 mt-20 mb-6">Access Vote Portal</h1>
        <p class="text-lg font-medium text-left text-gray-600 mb-12">Please enter your voter identification number(VIN)</p>

        <form class="mt-16 animate__animated animate__fadeInUp" action="/otp">
            <div class="mb-6">
                <label class="text-md block mb-2 font-bold text-gray-600">Enter VIN Number</label>
                <input type="text" name="vin" value="PRE1234567890" class="tracking-wide w-full p-4 outline-none bg-white rounded-lg border-gray-300 border"/>
            </div>
            <div class="mt-12">
                <input type="submit" name="submit" value="Get OTP" class="cursor-pointer w-full p-4 text-center text-white font-bold outline-none bg-green-600 rounded-lg"/>
            </div>
        </form>
    
    </div>
  

</div>