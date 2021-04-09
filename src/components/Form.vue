<template>
  <section class="min-h-screen flex flex-col">
    <div class="flex flex-1 items-center justify-center">
      <div
        class="rounded-lg sm:border-2 px-4 lg:px-24 py-16 lg:max-w-xl sm:max-w-md w-full text-center"
      >
        <form class="text-center">
          <h1
            class="font-bold tracking-wider text-3xl mb-8 w-full text-gray-600"
          >
            Sign in
          </h1>
          <div class="py-2 text-left">
            <input
              type="name"
              class="bg-gray-200 border-2 border-gray-100 focus:outline-none bg-gray-100 block w-full py-2 px-4 rounded-lg focus:border-gray-700"
              placeholder="Nombre"
              v-model="name"
            />
          </div>
          <div class="py-2 text-left">
            <input
              type="lastName1"
              class="bg-gray-200 border-2 border-gray-100 focus:outline-none bg-gray-100 block w-full py-2 px-4 rounded-lg focus:border-gray-700"
              placeholder="Apellido Paterno"
              v-model="lastName1"
            />
          </div>
          <div class="py-2 text-left">
            <input
              type="lastName2"
              class="bg-gray-200 border-2 border-gray-100 focus:outline-none bg-gray-100 block w-full py-2 px-4 rounded-lg focus:border-gray-700"
              placeholder="Apellido Materno"
              v-model="lastName2"
            />
          </div>
          <div class="py-2 text-left">
            <input
              type="adress"
              class="bg-gray-200 border-2 border-gray-100 focus:outline-none bg-gray-100 block w-full py-2 px-4 rounded-lg focus:border-gray-700"
              placeholder="Domicilio"
              v-model="address"
            />
          </div>
          <div class="py-2 text-left">
            <input
              type="phone"
              class="bg-gray-200 border-2 border-gray-100 focus:outline-none bg-gray-100 block w-full py-2 px-4 rounded-lg focus:border-gray-700"
              placeholder="Telefono Fijo"
              v-model="homePhone"
            />
          </div>
          <div class="py-2 text-left">
            <input
              type="cellPhone"
              class="bg-gray-200 border-2 border-gray-100 focus:outline-none bg-gray-100 block w-full py-2 px-4 rounded-lg focus:border-gray-700"
              placeholder="Telefono Celular"
              v-model="cellPhone"
            />
          </div>
          <div class="py-2 text-left">
            <input
              type="town"
              class="bg-gray-200 border-2 border-gray-100 focus:outline-none bg-gray-100 block w-full py-2 px-4 rounded-lg focus:border-gray-700"
              placeholder="Municipio"
              v-model="town"
            />
          </div>
          <div class="py-2 text-left">
            <input
              type="state"
              class="bg-gray-200 border-2 border-gray-100 focus:outline-none bg-gray-100 block w-full py-2 px-4 rounded-lg focus:border-gray-700"
              placeholder="Estado"
              v-model="state"
            />
          </div>
          <div class="py-2 text-left">
            <input
              type="country"
              class="bg-gray-200 border-2 border-gray-100 focus:outline-none bg-gray-100 block w-full py-2 px-4 rounded-lg focus:border-gray-700"
              placeholder="País"
              v-model="country"
            />
          </div>
          <div class="py-2 text-left">
            <input
              type="userType"
              class="bg-gray-200 border-2 border-gray-100 focus:outline-none bg-gray-100 block w-full py-2 px-4 rounded-lg focus:border-gray-700"
              placeholder="Tipo de usuario"
              v-model="typeOfUser"
            />
          </div>
          <div class="py-2 text-left">
            <input
              type="cedule"
              class="bg-gray-200 border-2 border-gray-100 focus:outline-none bg-gray-100 block w-full py-2 px-4 rounded-lg focus:border-gray-700"
              placeholder="Cedula Profesional"
              v-model="professionalLicense"
            />
          </div>
          <div class="py-2 text-left">
            <input
              type="email"
              class="bg-gray-200 border-2 border-gray-100 focus:outline-none bg-gray-100 block w-full py-2 px-4 rounded-lg focus:border-gray-700"
              placeholder="Email"
              v-model="email"
            />
          </div>
          <div class="py-2 text-left">
            <input
              type="password"
              class="bg-gray-200 border-2 border-gray-100 focus:outline-none bg-gray-100 block w-full py-2 px-4 rounded-lg focus:border-gray-700"
              placeholder="Password"
              v-model="password"
            />
          </div>
          <div class="py-2">
            <input
              type="submit"
              class="border-2 border-gray-100 focus:outline-none bg-purple-600 text-white font-bold tracking-wider block w-full p-2 rounded-lg focus:border-gray-700 hover:bg-purple-700"
              value="Sign In"
            />
          </div>
        </form>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "Form",
  data:function(){
    return{
      name: "",
      lastName1: "",
      lastName2: "",
      address: "",
      homePhone: "",
      cellPhone: "",
      town: "",
      state: "",
      country: "",
      typeOfUser: "",
      professionalLicense: "",
      email: "",
      password: "",
      error: false,
      error_msg: "",
    }
  }
};
</script>
