<template>
    <h1>Hola desde aqui 2</h1>
</template>
<script setup lang="ts">
import { ref } from 'vue';
// icons
import { LockIcon,UserIcon,MailIcon } from 'vue-tabler-icons';
const checkbox1 = ref(false);
</script>
<template>
    <v-label class="mb-2 font-weight-medium">Usuario</v-label>
    <v-text-field
        variant="outlined"
        type="text"
        placeholder="usuario"
        color="primary"
    >  
        <template v-slot:append-inner>
            <UserIcon stroke-width="1.5" size="22"  class="text-medium-emphasis" />
        </template>
    </v-text-field>
    <v-label class="mb-2 font-weight-medium">Nombre</v-label>
    <v-text-field
        variant="outlined"
        type="text"
        placeholder="Nombre"
        color="primary"
    >  
        <template v-slot:append-inner>
            <UserIcon stroke-width="1.5" size="22"  class="text-medium-emphasis" />
        </template>
    </v-text-field>
    <v-label class="mb-2 font-weight-medium">Email</v-label>
    <v-text-field
        variant="outlined"
        type="email"
        placeholder="Email"
        color="primary"
    >  
        <template v-slot:append-inner>
            <MailIcon stroke-width="1.5" size="22"  class="text-medium-emphasis" />
        </template>
    </v-text-field>
    <v-label class="mb-2 font-weight-medium">Password</v-label>
    <v-text-field
        variant="outlined"
        type="password"
        placeholder="Password"
        color="primary"
    >  
        <template v-slot:append-inner>
            <LockIcon stroke-width="1.5" size="22" class="text-medium-emphasis" />
        </template>
    </v-text-field>
    <v-label class="mb-2 font-weight-medium">Confirm Password</v-label>
    <v-text-field
        variant="outlined"
        type="password"
        color="primary"
        hide-details
        placeholder="Confirm Password"
    >
        <template v-slot:append-inner>
            <LockIcon stroke-width="1.5" size="22"  class="text-medium-emphasis"  />
        </template>
    </v-text-field>
     <div class="my-3">
        <v-checkbox density="compact" v-model="checkbox1" hide-details color="primary" label="Check Me Out!"></v-checkbox>
    </div>
    <v-btn color="primary" class="mr-3">Submit</v-btn>
    <v-btn color="error" class="mr-3">Cancel</v-btn>
</template>

