<template>
  <Head>
    <Title>About | {{ $config.projectMetadataTitle }}</Title>
    <Meta property="og:title" :content="'About | ' + $config.projectMetadataTitle" />
  </Head>

  <div class="card border scroll-500">
    <div class="card-body">
      <p class="fs-3" @click="$router.back()">
        <i class="bi bi-arrow-left-circle cursor-pointer"></i>
      </p>

      <h3 class="mb-3 mt-3">The First NFT Launchpad on Superposition</h3>

      <p class="text-break mt-3">
        meowNFTs is the first NFT launchpad and marketplace on Superposition.
      </p>

      <h5>New kind of NFTs</h5>

      <p class="text-break mt-3">
        NFTs created on meowNFTs are not your usual NFTs. Each NFT collection has a built-in pool which allows 
        the NFT to be <strong>always liquid</strong>.
      </p>

      <p class="text-break mt-3">
        This means that you can always sell your NFT back to the pool (except if you're the last one owning it 😄).
      </p>

      <h5>Useful links</h5>

      <ul>
        <li><a href="https://meow.domains" target="_blank">Meow Domains</a></li>
        <li><a href="https://github.com/iggy-social/meow-nfts" target="_blank">GitHub</a></li>
      </ul>

      <h5>Tech stack</h5>

      <p class="text-break mt-3">
        This app is built on top of various decentralized and open source technologies, such as:
      </p>

      <ul>
        <li><a href="https://arweave.org/" target="_blank">Arweave</a></li>
        <li><a href="https://punk.domains/" target="_blank">Punk Domains</a></li>
        <li><a href="https://iggy.social/" target="_blank">Iggy Social</a></li>
        <li>... and others.</li>
      </ul>

      <p class="text-break mt-3">
        There is no reliance on any web2 backend code/database, which means you can easily run your own instance of this app. 
        It will show the same content as this instance, but you can add your touches to the frontend.
      </p>

      <hr />

      <h5>Feedback</h5>

      <p class="text-break mt-3">
        Feel free to contact 
        <a href="https://warpcast.com/tempetechie.eth" target="_blank">Tempe Techie 🎩</a> or
        <a href="https://warpcast.com/tekr0x.eth" target="_blank">Tekr 🎩</a> 
        via Warpcast. 
      </p>

    </div>
  </div>
</template>

<script>
export default {
  name: 'About'
}
</script>