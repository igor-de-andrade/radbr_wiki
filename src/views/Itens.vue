<script setup>
import NavBar from "@/components/NavBar.vue";
import Card from "../components/Card.vue";
</script>

<template>
  <NavBar />
  <div class="itens">
    <div class="grouping">
      <h1 class="title">Itens</h1>
      <hr />
      <p class="description">
        A cada update cresce o número de itens encontrados no Tibia. Muitos
        deles podem ser comercializados por jogadores dentro do mercado
        encontrado nos depots das cidades. No mercado é possível ver os valores
        praticados de um determinado item em um servidor, como também
        informações sobre o peso, as descrições, os ataques e defesas de armas e
        escudos. Existem tantos itens catalogados com tantos propósitos
        diferentes que essa lista foi dividida em diferentes categorias.
      </p>
    </div>

    <section>
      <div class="grouping">
        <h2 class="subtitle">Equipamentos</h2>
        <hr />
        <p class="description">
          Esses itens servem para a defesa de seu personagem, eles possuem
          variados níveis de defesa. Um jogo completo de equipamentos, também
          conhecido como set, é formado por um capacete, uma armadura, um escudo
          ou um spellbook, uma bota e uma calça.
        </p>
      </div>

      <div class="card-list">
        <Card name="Druid" imgPath="/public/itens/equipaments/druid.gif" />
        <Card name="Drunou" imgPath="/public/itens/equipaments/drunou.gif" />
        <Card
          name="Infernalist"
          imgPath="/public/itens/equipaments/infernalist.gif"
        />
        <Card name="Knight" imgPath="/public/itens/equipaments/knight.gif" />
        <Card name="Knocker" imgPath="/public/itens/equipaments/knocker.gif" />
        <Card name="Paladin" imgPath="/public/itens/equipaments/paladin.gif" />
        <Card
          name="Sorcerer"
          imgPath="/public/itens/equipaments/sorcerer.gif"
        />
        <Card
          name="Especiais"
          imgPath="/public/itens/equipaments/special.gif"
        />
      </div>
    </section>

    <section>
      <div class="grouping">
        <h2 class="subtitle">Armas</h2>
        <hr />
        <p class="description">
          Todo personagem precisa ter uma arma, seja ela de uma ou duas mãos,
          aqui segue a lista com todas elas.
        </p>
      </div>
      <div class="card-list">
        <Card name="Druid" imgPath="/public/itens/weapons/druid.gif" />
        <Card name="Drunou" imgPath="/public/itens/weapons/drunou.gif" />
        <Card
          name="Infernalist"
          imgPath="/public/itens/weapons/infernalist.gif"
        />
        <Card name="Knight" imgPath="/public/itens/weapons/knight.gif" />
        <Card name="Knocker" imgPath="/public/itens/weapons/knocker.gif" />
        <Card name="Paladin" imgPath="/public/itens/weapons/paladin.gif" />
        <Card name="Sorcerer" imgPath="/public/itens/weapons/sorcerer.gif" />
      </div>
    </section>

    <section>
      <div class="grouping">
        <h2 class="subtitle">Outros</h2>
        <hr />
        <p class="description">
          Existem vários equipamentos além dos de defesa e armas e todo Tibiano
          precisa estar preparado para qualquer perigo que encontrar.
        </p>
      </div>
      <div class="card-list">
        <Card name="Imbuiment" imgPath="/public/itens/others/imbuiments.gif" />
        <Card name="Divinação" imgPath="/public/itens/others/divination.gif" />
        <Card name="Bonding" imgPath="/public/itens/others/bonding.gif" />
      </div>
    </section>
  </div>
</template>

<style scoped>
.itens {
  padding: 30px;
  display: flex;
  flex-direction: column;
  gap: 50px;
}

.grouping {
  display: flex;
  flex-direction: column;
  gap: 10px;
}

section {
  display: flex;
  flex-direction: column;
  gap: 20px;
}

hr {
  border-top: 1px solid #ccc;
}

.title {
  font-family: "Cinzel Decorative", serif;
  font-weight: 800;
  font-style: normal;
  font-size: 36px;
}

.subtitle {
  font-family: "Cinzel Decorative", serif;
  font-weight: 600;
  font-style: normal;
  font-size: 24px;
}

.description {
  font-family: "Mont-serrat", sans-serif;
  font-style: normal;
  font-size: 14px;
}

.card-list {
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  gap: 30px;
  justify-content: center;
}
</style>
