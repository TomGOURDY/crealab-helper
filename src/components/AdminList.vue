<template>
  <section id="admin-list">
    <div id="lists">
        <ul class="list" id="items-owned">
          <li>Imprimante 3D</li>
          <li>Troisième main</li>
          <li>Cruciforme</li>
        </ul>
        <div>
          <h2>Liste de courses</h2>
          <ul class="list" id="items-needed">
            <li>LED</li>
            <li>PLA</li>
          </ul>
        </div>
        
    </div>
    <div id="form">
      <input type="text" id="matos-name" placeholder="Nom du produit"/>
      <input type="number" id="matos-quantity" placeholder="Quantité du produit"/>
      <input type="number" id="matos-minQuantity" placeholder="Quantité minimum du produit"/>
      <input type="number" id="matos-price" placeholder="Prix du produit" step=".01"/>
      <input type="text" id="matos-link" placeholder="Lien du site marchand">
      <div class="checkbox-wrapper">
        <input type="checkbox" id="matos-isConsommable" name="consommable"/>
        <label for="consommable">Consommable ?</label>
      </div>
      <div class="checkbox-wrapper">
        <input type="checkbox" id="matos-isPriority" name="priority"/>
        <label for="priority">Achat prioritaire ?</label>
      </div>
      <input id="sendList" type="submit" value="Passer commande"/>
    </div>
  </section>
</template>

<script>
export default {
    name: "AdminList"
}
</script>

<style>
h2 {
  font-size: 30px;
  font-weight: bold;
  text-decoration: underline;
}
#admin-list {
  margin-left: 25%;
  margin-right: 25%;
}

#lists {
  display: flex;
  justify-content: space-between;
  text-align: left;
  font-size: 20px;
}

ul {
  list-style: none;
}

.list {
  display: flex;
  flex-direction: column;
}

.list li {
  padding: 5px;
}

#form {
  margin-top: 60px;
  display: flex;
  flex-direction: column;
}
#form input {
  margin-bottom: 5px;
  padding: 15px;
  font-size: 20px;
}

#form input::placeholder {
  font-size: 20px;
  padding-top: 5px;
}
.checkbox-wrapper {
  display: flex;
}

.checkbox-wrapper label {
  margin-left: 20px;
  font-size: 20px;
}

#sendList {
  margin-top: 5px;
  padding: 15px;
  font-size: 20px;
}
</style>