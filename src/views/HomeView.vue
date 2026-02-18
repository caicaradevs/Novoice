<script setup lang="ts">
</script>

<template>
  <main class="page">
    <header class="page__header">
      <h1 class="page__title">Create New Invoice</h1>
      <p class="page__subtitle">Add the information Required to Generate your Invoice</p>
    </header>

    <section class="card">
      <form class="form" action="#" method="post">
        <div class="grid grid--2">
          <div class="field">
            <label for="invdate">Invoice Date</label>
            <input type="date" id="invdate" name="invdate" placeholder="DD/MM/YYYY" />
          </div>

          <div class="field">
            <label for="invnumber">Invoice Number</label>
            <input type="text" id="invnumber" name="invnumber" placeholder="#000000" />
          </div>
        </div>

        <div class="grid grid--2">
          <div class="field field--full">
            <label for="servicedescription">Service Description</label>
            <input type="text" id="servicedescription" name="servicedescription" placeholder="Description of Service Provided" />
          </div>

          <div class="field">
            <label for="servicedate">Service Date</label>
            <input type="date" id="servicedate" name="servicedate" placeholder="Date of Service" />
          </div>

          <div class="field">
            <label for="location">Location</label>
            <input type="text" id="location" name="location" placeholder="Venue or Address" />
          </div>

          <div class="field">
            <label for="totalprice">Total Price</label>
            <input type="text" id="totalprice" name="totalprice" placeholder="$AUD" inputmode="decimal" />
          </div>
        </div>

        <hr class="divider" />

        <div class="section-head">
          <h2>Client Details</h2>
        </div>

        <div class="grid grid--2">
          <div class="field">
            <label for="CompanyName">Company Name</label>
            <input type="text" id="CompanyName" name="CompanyName" placeholder="Hey Business" />
          </div>

          <div class="field">
            <label for="abnclient">ABN Number</label>
            <input type="text" id="abnclient" name="abnclient" placeholder="1234567890" />
          </div>

          <div class="field field--full">
            <label for="addressclient">Address</label>
            <input type="text" id="addressclient" name="addressclient" placeholder="Spencer St, Melbourne, Australia" />
          </div>
        </div>

        <hr class="divider" />

        <div class="section-head">
          <h2>Your Company Details</h2>
        </div>

        <div class="grid grid--2">
          <div class="field">
            <label for="mycompanyname">Business Name</label>
            <input type="text" id="mycompanyname" name="mycompanyname" placeholder="Business Name" />
          </div>

          <div class="field">
            <label for="myabn">ABN Number</label>
            <input type="text" id="myabn" name="myabn" placeholder="1234567890" />
          </div>

          <div class="field">
            <label for="mynumber">Phone Number</label>
            <input type="text" id="mynumber" name="mynumber" placeholder="1234567890" />
          </div>

          <div class="field field--full">
            <label for="myaddress">Address</label>
            <input type="text" id="myaddress" name="myaddress" placeholder="Spencer St, Melbourne" />
          </div>
        </div>

        <hr class="divider" />

        <div class="section-head">
          <h2>Banking Details</h2>
        </div>

        <div class="grid grid--2">
          <div class="field">
            <label for="bankname">Bank Name</label>
            <input type="text" id="bankname" name="bankname" placeholder="Bank Name" />
          </div>

          <div class="field">
            <label for="bsbnumber">BSB Number</label>
            <input type="text" id="bsbnumber" name="bsbnumber" placeholder="000-000" />
          </div>

          <div class="field">
            <label for="accountname">Account Name</label>
            <input type="text" id="accountname" name="accountname" placeholder="Your Account Name" />
          </div>

          <div class="field">
            <label for="accountnumber">Account Number</label>
            <input type="text" id="accountnumber" name="accountnumber" placeholder="123456789" />
          </div>
        </div>

        <div class="actions">
          <button class="btn btn--primary" type="submit">Generate Invoice</button>
        </div>
      </form>
    </section>
  </main>
</template>

<style>

:root{
  --bg: #f4f6fb;
  --card: #ffffff;
  --text: #0f172a;
  --muted: #64748b;
  --line: #e5e7eb;
  --field: #f8fafc;
  --field-border: #e2e8f0;
  --primary: #2563eb;
  --primary-dark: #1d4ed8;
  --radius: 14px;
}

*{ box-sizing: border-box; }
html,body{ height:100%; }
body{
  margin:0;
  font-family: ui-sans-serif, system-ui, -apple-system, "Segoe UI", Roboto, Arial, "Noto Sans", "Helvetica Neue", sans-serif;
  color: var(--text);
  background: var(--bg);
}

.page{
  max-width: 980px;
  margin: 48px auto;
  padding: 0 18px;
}

.page__header{
  margin-bottom: 18px;
}
.page__title{
  font-size: 34px;
  line-height: 1.15;
  margin: 0 0 8px 0;
  letter-spacing: -0.02em;
}
.page__subtitle{
  margin: 0;
  color: var(--muted);
  font-size: 15px;
}

.card{
  background: var(--card);
  border: 1px solid var(--line);
  border-radius: var(--radius);
  box-shadow: 0 10px 30px rgba(15, 23, 42, 0.06);
  padding: 22px;
}

.form{ width: 100%; }

.section-head h2{
  font-size: 16px;
  margin: 0;
  letter-spacing: -0.01em;
}

.divider{
  border: 0;
  border-top: 1px solid var(--line);
  margin: 18px 0;
}

.grid{
  display: grid;
  gap: 14px;
  margin-bottom: 14px;
}

.grid--2{
  grid-template-columns: repeat(2, minmax(0, 1fr));
}

.field{
  display: flex;
  flex-direction: column;
  gap: 8px;
}

.field--full{
  grid-column: 1 / -1;
}

label{
  font-size: 13px;
  color: #334155;
}

input{
  width: 100%;
  border: 1px solid var(--field-border);
  background: var(--field);
  border-radius: 12px;
  padding: 12px 12px;
  font-size: 14px;
  outline: none;
  transition: border-color .15s ease, box-shadow .15s ease, background .15s ease;
}

input::placeholder{
  color: #94a3b8;
}

input:focus{
  background: #fff;
  border-color: rgba(37, 99, 235, 0.6);
  box-shadow: 0 0 0 4px rgba(37, 99, 235, 0.15);
}

.btn{
  border: 1px solid transparent;
  border-radius: 12px;
  padding: 10px 14px;
  font-weight: 600;
  font-size: 14px;
  cursor: pointer;
}

.actions{
  margin-top: 18px;
  display: flex;
  justify-content: flex-end;
}

.btn--primary{
  background: var(--primary);
  color: #fff;
}
.btn--primary:hover{
  background: var(--primary-dark);
}

/* Responsive */
@media (max-width: 720px){
  .page{ margin: 28px auto; }
  .card{ padding: 16px; }
  .grid--2{ grid-template-columns: 1fr; }
  .actions{ justify-content: stretch; }
  .btn--primary{ width: 100%; }
}


</style>
