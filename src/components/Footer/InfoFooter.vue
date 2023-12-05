<script>
export default {
  name: "InfoFooter",
  props: ["departments"],
  data() {
    return {
      // Social data array
      socialClass: [
        "fa-facebook-square",
        "fa-twitter-square",
        "fa-youtube-square",
        "fa-instagram-square",
      ],
    };
  },
};
</script>

<template>
    <!-- INFO-FOOTER SECTION -->
    <section id="info-footer">
      <div class="adava-info container">
        <!-- Social  -->
        <div class="col social-info">
          <a href="#">
            <img src="/src/assets/images/medical_logo_1x_dark.png" alt="adava" />
          </a>
          <p>
            Sed ut perspiciatis unde omnis iste natus error sit voluptatem
            accusantium dolemue launti totam aperiam, eaque ipsa quae abillo.
            Invente veriatis et quasi architecto beatae luptatem accusantium,
            remaperiamsiat. Voluptatem accusest etsium doloremque laudaien. Lorem
            ipsum sits dolores ets unser.
          </p>
          <span class="uppercase">learn more about us</span>
          <div class="social-icon">
            <a href="#">
              <i
                v-for="(social, index) in socialClass"
                :key="index"
                class="fab"
                :class="social"
              ></i>
            </a>
          </div>
        </div>
        <!-- Contact  -->
        <div class="col contact-info">
          <h6 class="uppercase">contact information</h6>
          <div>
            <i class="fas fa-map-marker-alt"></i>
            <address class="clickable">
              121king Street, London United Kingdom
            </address>
          </div>
          <div>
            <i class="fas fa-phone"></i>
            <span class="clickable">1.800.458.556</span>
          </div>
        </div>
        <!-- Departments -->
        <div class="col departments-info">
          <h6 class="uppercase">medical departments</h6>
          <ul>
            <li v-for="(department, index) in departments" :key="index">
              <i class="fas fa-chevron-circle-right"></i>
              <a href="#" class="clickable">
                {{ department }}
              </a>
            </li>
          </ul>
          <button class="uppercase clickable">View our departments</button>
        </div>
      </div>
    </section>
  </template>

  <style lang="scss" scoped>

#info-footer {
  padding: 40px 0;
}
.adava-info {
  display: flex;
}
.contact-info,
.departments-info {
  width: 350px;
}

.contact-info 
  h6 {
    font-weight: 300;
    font-size: 14px;
    color: #46525f;
      content: "";
      width: 100px;
      border: 1px solid #3aafbf;
      display: block;
      margin: 15px 0;
    }
  
  i {
    color: #3aafbf;
    font-size: 12px;
  }
  address {
    display: inline-block;
    font-size: 13px;
    font-weight: lighter;
    font-style: normal;
    padding-left: 10px;
    color: #7c858f;
  }
  span {
    font-size: 13px;
    font-weight: lighter;
    padding-left: 7px;
    color:  #7c858f;

  }


.departments-info {
  h6 {
    font-weight: 300;
    font-size: 14px;
    color: grey;
  
  }
  li {
    
    display: flex;
    align-items: center;
    margin-bottom: 8px;
    a {
      text-decoration: none;
      color: grey;
      font-size: 12px;
      font-weight: lighter;
      padding-left: 5px;
     
    }
    i {
      font-size: 16px;
      color: grey;
    }
  }
  button {
    background-color: white;
    border: 1px solid grey;
    padding: 8px 22px;
    font-size: 13px;
    color: grey;
    font-weight: 300;
    margin-top: 50px;
    
  }
}

.social-info {
  width: 500px;
}
p{
  font-size: 12px;
    width: 420px;
    font-weight: lighter;
    line-height: 22px;
}

span {
    font-size: 12px;
    font-weight: lighter;
    color: grey;
  }

  .social-icon{
    margin-top: 18px;
    font-size: 22px;
  }
  i {
      padding-right: 5px;
      &.fa-facebook-square {
        color: #3c5998;
        //? Hover effect
        &:hover {
          transform: scale(1.1);
        }
      }
      &.fa-twitter-square {
        color: #54acee;
        //? Hover effect
        &:hover {
          transform: scale(1.1);
        }
      }
      &.fa-youtube-square {
        color: rgb(207, 7, 7);
        //? Hover effect
        &:hover {
          transform: scale(1.1);
        }
      }
      &.fa-instagram-square {
        color: #3f729b;
        //? Hover effect
        &:hover {
          transform: scale(1.1);
        }
      }
    }
</style>