<template>
  <div class="m-4">
    <FormKit
      type="text"
      label="name"
      :validation="[
        ['required'],
        ['length', 3, 20],
        ['matches', /^[A-Za-z0-9\_]+$/],
      ]"
      validation-visibility="live"
      :validation-messages="{
        matches: 'Please enter a valid name.',
      }"
      placeholder="Enter your name..."
    />
  </div>
</template>

<style></style>
