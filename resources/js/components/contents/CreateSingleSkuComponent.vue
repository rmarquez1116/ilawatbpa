<template>
<div class="_container">
  <div class="_content-title">
    <div class="_title _pull-left">Create New SKU</div>
    <input type="button" class="_pull-right _btn _no-border" value="Upload SKU by batch" />
  </div>

  <hr />
  Upload Indivilually
  <hr />

  <input type="button" class="_pull-left _btn" value="Choose a photo" />
  <div class="_content-body _col-100">

    <div class="_form-group">
      <div><label>Product ID/Code</label></div>
      <div><input type="text" v-model="productName" /></div>
    </div>

    <div class="_form-group">
      <div><label>Brand</label></div>
      <div><input type="text" /></div>
    </div>

    <div class="_form-group">
      <div><label>Product Name</label></div>
      <div><input type="text" /></div>
    </div>

  </div>

  <div class="_col-100">
    <div class="_col-50">
      <div class="_form-group">
        <div><label>Product Description</label></div>
        <div><textarea></textarea></div>
      </div>
    </div>

    <div class="_col-50">
      <div>
        Variations
        <hr />
      </div>

      <div class="_form-group _inline" :style="{'padding-left': '38px'}" >
        <div><label>Color</label></div>
        <div><input type="text" /></div>
      </div>

      <div class="_form-group _inline">
        <div><label>Body Color</label></div>
        <div><input type="text" /></div>
      </div>

      <div class="_form-group _inline">
        <div><label>Dimensions</label></div>
        <div><input type="text" /></div>
      </div>
    </div>
  </div>

      <div>
        Categories
        <hr />
      </div>

    <div class="_col-100">
      <div class="_form-group _col-20">
        <div>
          <label>Main Category</label>
        </div>
        <div>
          <select>
            <option value="volvo">Volvo</option>
            <option value="saab">Saab</option>
            <option value="mercedes">Mercedes</option>
            <option value="audi">Audi</option>
          </select>
        </div>
      </div>
        <div class="_form-group _col-20">
          <div>
            <label>Sub-category</label>
          </div>
          <div>
            <select>
              <option value="volvo">Volvo</option>
              <option value="saab">Saab</option>
              <option value="mercedes">Mercedes</option>
              <option value="audi">Audi</option>
            </select>
          </div>
        </div>
          <div class="_form-group _col-20">
            <div>
              <label>Uses</label>
            </div>
            <div>
              <select>
                <option value="volvo">Volvo</option>
                <option value="saab">Saab</option>
                <option value="mercedes">Mercedes</option>
                <option value="audi">Audi</option>
              </select>
            </div>
          </div>
            <div class="_form-group _col-20">
              <div>
                <label>Classification</label>
              </div>
              <div>
                <select>
                  <option value="volvo">Volvo</option>
                  <option value="saab">Saab</option>
                  <option value="mercedes">Mercedes</option>
                  <option value="audi">Audi</option>
                </select>
              </div>
            </div>
              <div class="_form-group _col-20">
                <div>
                  <label>Sub-classification</label>
                </div>
                <div>
                  <select>
                    <option value="volvo">Volvo</option>
                    <option value="saab">Saab</option>
                    <option value="mercedes">Mercedes</option>
                    <option value="audi">Audi</option>
                  </select>
                </div>
              </div>
    </div>
    <div>
      Product Specification
      <hr />
    </div>
    <div class="_col-100">
      <div class="_col-25">


        <div class="_form-group _inline">
        <div><label>IP Rating</label></div>
        <div><input type="text" class="_col-100" /></div>
        </div>

        <div class="_form-group _inline">
        <div><label>Base</label></div>
        <div><input type="text" class="_col-100" /></div>
        </div>

        <div class="_form-group _inline">
        <div><label>Wattage</label></div>
        <div><input type="text" class="_col-100" /></div>
        </div>

        <div class="_form-group _inline">
        <div><label>Voltage</label></div>
        <div><input type="text" class="_col-100" /></div>
        </div>

        <div class="_form-group _inline">
        <div><label>Frequency</label></div>
        <div><input type="text" class="_col-100" /></div>
        </div>
      </div>

        <div class="_col-25">


          <div class="_form-group _inline">
          <div><label>Bean Angle</label></div>
          <div><input type="text" class="_col-100" /></div>
          </div>

          <div class="_form-group _inline">
          <div><label>CRI (Color Rendering Index)</label></div>
          <div><input type="text" class="_col-100" /></div>
          </div>

          <div class="_form-group _inline">
          <div><label>LED Rated Lite</label></div>
          <div><input type="text" class="_col-100" /></div>
          </div>

          <div class="_form-group _inline">
          <div><label>Color Temp</label></div>
          <div><input type="text" class="_col-100" /></div>
          </div>

          <div class="_form-group _inline">
          <div><label>Cut-out size</label></div>
          <div><input type="text" class="_col-100" /></div>
          </div>
        </div>
    </div>
</div>
</template>

<script>
  export default {
    data() {
      return {
        productName : 'sample'
      }
    }
  }
</script>

<style scoped>
._container{
  position: absolute;
  margin-top: 74px;
  margin-left: 20%;
  width: 80%;
  height: 100%;
}

._content-title{
  display: flex;
}

._pull-right{
  right: 0;
  position: absolute;
}

._content-body{
  display: flex;
}
._form-group{
  margin: 10px;
}


._form-group._inline{
  display: inline-flex;
}

._form-group._inline>div{
  margin: 2px;
}

._form-group._inline>div>label{
  vertical-align: sub;
}

._form-group>div>input{
  width: 275px;
  border-radius: 5px;
  height: 25px;
  border: solid 1px #dddddd;
}

._form-group>div>select{
  width: 100%;
  border-radius: 5px;
  height: 25px;
  border: solid 1px #dddddd;
}

._form-group>div>textarea{
  width: 100%;
  border-radius: 5px;
  height: 200px;
  border: solid 1px #dddddd;
  resize: none;
}

._btn{
  width: 135px;
  height: 30px;
  border-radius: 5px;
  border: solid 1px #f0eeec;
  background-color: #f0eeec;
  box-shadow: 3px 3px #dddddd;
}

._col-20{
  width: 20% !important;
}

._col-25{
  width: 25% !important;
}

._col-50{
  width: 50% !important;
}

._col-100{
  width: 100% !important;
  display: flex;
}

._btn:focus{
    outline-color: green;
}

._btn._no-border{
  border: none;
  box-shadow: none;
}
</style>
