<template>
  <Head>
    <Link rel="canonical" href="https://meownfts.com" />
  </Head>
</template>

<script>
import { useEthers } from '~/store/ethers'

export default {
  name: "index",

  mounted() {
    const curComp = window.localStorage.getItem("currentNftPage");

    if (!curComp) {
      return this.$router.push({ path: '/nft' });
    } else {
      return this.$router.push({ path: curComp });
    }
  },

  setup() {
    const { address, chainId } = useEthers()

    return { address, chainId }
  }
}
</script>