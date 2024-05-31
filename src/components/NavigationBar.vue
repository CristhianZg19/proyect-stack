<template>
  <v-navigation-drawer expand-on-hover rail>
    <v-list>
      <v-list-item
        :prepend-avatar="avatar"
        subtitle="cristhianzapata@gmail.com"
        title="Administrador"
      ></v-list-item>
    </v-list>

    <v-divider></v-divider>

    <v-list density="compact" nav>
      <v-list-item
        prepend-icon="mdi-account-multiple"
        title="Usuarios"
        value="shared"
      ></v-list-item>
      <v-list-item
        prepend-icon="mdi-cog"
        title="Configuración"
        value="starred"
      ></v-list-item>
    </v-list>
    <template v-slot:append>
      <div class="pa-2">
        <v-btn v-tooltip="'Cerrar sessión'" block
          ><v-icon>mdi-logout</v-icon></v-btn
        >
      </div>
    </template>
  </v-navigation-drawer>
</template>
<script setup >
import avatar from "@/assets/avatar.png";
</script>