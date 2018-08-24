<template lang="html">
  <div class="admin">
    <h2>FORM UPLOAD</h2>
    <form>
      <input class="uk-input uk-width-1-2 input-box" type="text" placeholder="Product title"><br>
      <textarea class="uk-textarea uk-width-1-2 input-box" placeholder="product description"></textarea><br>
      <input class="uk-input uk-form-width-medium input-box" type="text" placeholder="Price">
      <input class="uk-input uk-form-width-medium input-box" type="text" placeholder="Weight (gr)"><br />
      <p>gambar utama</p>
      <input type="file" id="image" class="form-control-file"><br />
      <p>gambar lain</p>
       <input type="file" id="image" class="form-control-file"><br />
       <input type="file" id="image" class="form-control-file"><br />
       <input type="file" id="image" class="form-control-file"><br />
       <input type="file" id="image" class="form-control-file"><br />
       <div class="uk-margin">
            <select class="uk-select uk-width-1-6">
                <option @click="optionClicked('bag')">Bags</option>
                <option>Shoe Care</option>
                <option>Personal care</option>
            </select>
        </div>
        <div v-if="bagClicked">
          <div class="uk-margin">
               <select class="uk-select uk-width-1-6">
                   <option>Messenger Bag</option>
                   <option>Backpack</option>
                   <option>Sling Bag</option>
                   <option>Camera Bag</option>
                   <option>Pouch Bag</option>
               </select>
           </div>
        </div>
       <button class="uk-button uk-button-default submit-button">Upload</button>
    </form>
  </div>
</template>


<script>
export default {
  name: 'Admin',
  data() {
    return {
      bagClicked: false
    }
  },

  methods: {
    optionClicked(category) {
      if (category == 'bag') {
        return this.bagClicked = true;
      }
    }
  }
}
</script>

<style lang="css">
  .input-box {
    margin-bottom: 20px;
    border: 1px solid black;
    margin-right: 10px
  }

  .admin {
    margin-left: 10px
  }

  .submit-button {
    border: 1px black solid;
    margin-top: 20px;
  }
</style>
