<template>
<div class="bg-blue-100" >
    <h1 class=" border-gray-300 border-b-2">Welcome to op-developers club</h1>
    <div class="flex items-center min-h-screen">
        <div class="container mx-auto">
            <div class="max-w-md mx-auto my-10 bg-gray-100 p-5 rounded-md shadow-sm">
                <div class="text-center">
                    <h1 class="my-3 text-3xl font-semibold text-gray-700 dark:text-gray-200">Contact Us</h1>
                    <p class="text-gray-400 dark:text-gray-400">Fill up the form below to send us a message. {{name}} </p>
                </div>
                <div class="m-7">
                        <div class="mb-6">
                            <label for="name" class="block mb-2 text-sm text-gray-600 dark:text-gray-400">Full Name</label>
                            <input v-model="form.name" type="text" name="name" id="name" placeholder="John Doe" required class="w-full px-3 py-2 placeholder-gray-300 border border-gray-300 rounded-md focus:outline-none focus:ring focus:ring-indigo-100 focus:border-indigo-300 dark:bg-gray-700 dark:text-white dark:placeholder-gray-500 dark:border-gray-600 dark:focus:ring-gray-900 dark:focus:border-gray-500" />
                        </div>
                        <div class="mb-6">
                            <label for="email" class="block mb-2 text-sm text-gray-600 dark:text-gray-400">Email Address</label>
                            <input v-model="form.email" type="email" name="email" id="email" placeholder="you@company.com" required class="w-full px-3 py-2 placeholder-gray-300 border border-gray-300 rounded-md focus:outline-none focus:ring focus:ring-indigo-100 focus:border-indigo-300 dark:bg-gray-700 dark:text-white dark:placeholder-gray-500 dark:border-gray-600 dark:focus:ring-gray-900 dark:focus:border-gray-500" />
                        </div>
                 
                        <div class="mb-6">
                            <label for="message" class="block mb-2 text-sm text-gray-600 dark:text-gray-400">Your Message</label>
                            <textarea v-model="form.message" rows="5" name="message" id="message" placeholder="Your Message" class="w-full px-3 py-2 placeholder-gray-300 border border-gray-300 rounded-md focus:outline-none focus:ring focus:ring-indigo-100 focus:border-indigo-300 dark:bg-gray-700 dark:text-white dark:placeholder-gray-500 dark:border-gray-600 dark:focus:ring-gray-900 dark:focus:border-gray-500" required></textarea>
                        </div>
                        <div class="mb-6">
                            <button @click="onSubmit" type="submit" class="w-full px-3 py-4 text-white bg-indigo-500 rounded-md focus:bg-indigo-600 focus:outline-none">Send Message</button>
                        </div>
                        <p class="text-base text-center text-gray-400" id="result"> © OP-Developers 2016
                        </p>
                </div>
            </div>
        </div>
    </div>
    </div>

</template>


<script>
export default {
    name: 'Home',

    data() {
        return {
            form: {
                name: '',
                email: '',
                message: '',
            }
        }
    },

    methods :{
        // axios.post()
        onSubmit() {
            console.log(this.form)
            // console.log(e)
    
            
        },
    }
}
</script>