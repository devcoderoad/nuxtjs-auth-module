<template>
  <div>
    <div>Login</div>
    <v-form>
      <v-row>
        <v-col cols="12" md="4">
          <v-text-field
            v-model="username"
            :rules="{}"
            label="Username"
            required
          ></v-text-field>
        </v-col>
        <v-col cols="12" md="4">
          <v-text-field
            v-model="password"
            type="password"
            :rules="{}"
            label="Password"
            required
          ></v-text-field>
        </v-col>
      </v-row>
      <v-row>
        <v-col>
          <v-btn type="submit" elevation="2">Submit</v-btn>
        </v-col>
      </v-row>
    </v-form>
  </div>
</template>

<script>
export default {
  name: 'AuthLogin',
  data() {
    return { username: '', password: '' }
  },
}
</script>
