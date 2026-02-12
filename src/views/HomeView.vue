<script setup lang="ts">
</script>

<template>
  <main>
    <TheWelcome />

    <h1>Novoice</h1>
    <h1>Generate your invoice for free with this easy form</h1>

    <form>
        <h1>Your Invoice Details</h1>
        <label for="invdate">Invoice Date: </label>
        <input type="date" id="invdate" name="invdate"><br>
        <label for="invnumber">Invoice Number: </label>
        <input type="text" id="invnumber" name="invnumber"><br><br><br>

        <h1>Your Client Details</h1>
        <label for="CompanyName">Company Name: </label>
        <input type="text" id="CompanyName" name="CompanyName"><br>
        <label for="abnclient">Client's ABN Number: </label>
        <input type="text" id="abnclient" name="abnclient"><br>
        <label for="addressclient">Client's Address: </label>
        <input type="text" id="addressclient" name="addressclient"><br><br><br>

        <h1>My Company Details</h1>
        <label for="mycompanyname">My Company Name: </label>
        <input type="text" id="mycompanyname" name="mycompanyname"><br>
        <label for="myaddress">My Company Address: </label>
        <input type="text" id="myaddress" name="myaddress"><br>
        <label for="myabn">My ABN Number: </label>
        <input type="text" id="myabn" name="myabn"><br>
        <label for="mynumber">My Phone Number: </label>
        <input type="text" id="mynumber" name="mynumber"><br><br><br>

        <h1>Banking Details</h1>
        <label for="bankname">Bank Name: </label>
        <input type="text" id="bankname" name="bankname"><br>
        <label for="bsbnumber">BSB Number: </label>
        <input type="text" id="bsbnumber" name="bsbnumber"><br>
        <label for="accountname">Account Name: </label>
        <input type="text" id="accountname" name="accountname"><br>
        <label for="accountnumber">Account Number: </label>
        <input type="text" id="accountnumber" name="accountnumber"><br><br><br>

        <h1>Service Details</h1>
        <label for="servicedate">Service Date: </label>
        <input type="date" id="servicedate" name="servicedate"><br>
        <label for="servicedescription">Service Description: </label>
        <input type="text" id="servicedescription" name="servicedescription"><br>
        <label for="location">Location/Address of Service: </label>
        <input type="text" id="location" name="location"><br>
        <label for="totalprice">Total Price: </label>
        <input type="text" id="totalprice" name="totalprice"><br><br><br>

<button>Generate Invoice</button>
    </form>
  </main>
</template>

<style>

input,
form,
button,
label,
textarea,
h1 {
    font: inherit;
}

body {

    background-color: rgb(238, 238, 238);
    font-weight: bold;
}

</style>
