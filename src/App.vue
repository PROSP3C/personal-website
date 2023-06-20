<script setup>
window.Appcues.identify(
  '<<< USER_ID >>>', // unique, required
  {

    // recommended (optional) properties

    createdAt: 1566932390, // Unix timestamp of user signup date
    purchasedAd: 1566932395, // Unix timestamp of account purchase date (leave null if empty)
    planTier: 'Standard', // Current user’s plan tier
    role: 'Admin', // Current user’s role or permissions
    accountId: '1234', // Current user's account ID
    firstName: 'John', // current user's first name

    // additional suggestions

    companyName: 'Acme Corp', // Current user’s company name
    email: 'john.doe@example.com', // Current user's email
    location: '90210', // a zipcode, state, or country enables location-based targeting
    version: '2.0', // users on different versions may need to see different content
    language: 'spanish', // for multi-language applications
    renewalDate: 1577880288, // to remind users to renew
  },
)
</script>

<template>
  <div class="App">
    <h1>Test App</h1>

    <ElDivider />

    <div class="App-buttonContainer">
      <ElButton>Test Action 1</ElButton>
      <ElButton type="primary">Test Action 2</ElButton>
      <ElButton type="success">Test Action 3</ElButton>
      <ElButton type="info">Test Action 4</ElButton>
      <ElButton type="warning">Test Action 5</ElButton>
      <ElButton type="danger">Test Action 6</ElButton>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.App {
  width: 100%;
  height: 100vh;
  max-width: 400px;
  margin: auto;
  display: flex;
  align-items: center;
  flex-direction: column;
  justify-content: center;

  &-buttonContainer {
    width: 100%;
    display: flex;
    flex-wrap: wrap;
    gap: 20px;
    justify-content: space-between;
  }

  button {
    margin: 0;
  }
}
</style>
