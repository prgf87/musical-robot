<template>
  <q-page class="flex flex-center" padding>
    <section class="full-width" style="max-width: 400px">
      <h5 class="text-center q-my-sm">Login</h5>
      <q-card>
        <q-card-section>
          <q-form>
            <q-input
              model-value=""
              label="Email"
              type="email"
              placeholder="info@email.com"
              filled
              class="q-mb-md"
            />
            <q-input
              model-value=""
              label="Password"
              type="password"
              placeholder=""
              filled
            />
          </q-form>
        </q-card-section>
        <q-checkbox class="q-mb-md" label="Remember me" :model-value="true" />
        <q-btn label="Login" class="full-width" color="primary" />
      </q-card>
    </section>
  </q-page>
</template>
