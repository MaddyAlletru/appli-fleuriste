<template>
  <section>
<div class="nav-bar"></div>
<h1>Test d'application commandes connectées</h1>

<div>
    <h2>{{ cruise.name }}</h2>
    <div>{{ cruise.description }}</div>
    <hr />

    <div class="row">
        <div>
            <!-- TODO: Add booking-form -->

        </div>
        <div>
            <!-- TODO: Add booking-list -->

        </div>
    </div>
</div>
</section>
</template>

<script>



export default {
    name: 'Host',
data() {
    return {
        cruise: {
            name: 'ici',
            description: 'Projet de cahier de commandes pour L\'Entre Pots. Le but de ce projet est de voir si je peux créer une petite application afin de simplifier la prise de commandes en magasin et la gestion de leur réalisation.',
            cabins: [
                { name: 'Coach', price: 125000 },
                { name: 'Business', price: 275000 },
                { name: 'First', price: 430000 },
            ]
        },
        bookings: [
            { name: 'Sample', price: 0 }
        ]
    }
},

// TODO: Add components

// TODO: Add methods
}
</script>

<style>
body {
    background-color: #e28d8d84;
    margin: 0, 5%;
    font-family: tahoma;
}

.row {
    display: grid;
    grid-template-columns: 1fr 1fr;
    vertical-align: middle;
    margin: 2em;
}

.button {
    background-color: #39495c;
    border-radius: 5px;
    color: white;
    text-align: center;
}

.nav-bar {
    background: linear-gradient(-50deg, #010801, #0d0d60);
    height: 60px;
    margin-bottom: 25px;
}
</style>