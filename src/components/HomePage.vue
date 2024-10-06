<template>
  <v-container>
    <v-row class="main-row d-flex flex-column align-center py-15 px-16 px-sm-5">
      <v-col cols="12" sm="10" md="8" class="top px-9 py-9">
        <div class="heading1">Join our community</div>
        <div class="subheading1 my-3">
          30-day, hassle-free money back guarantee
        </div>
        <div class="para1 pr-6">
          Gain access to our full library of tutorials along with expert code
          reviews. Perfect for any developers who are serious about honing their
          skills.
        </div>
      </v-col>
      <v-col
        cols="12"
        sm="10"
        md="8"
        class="bottom d-flex flex-column flex-sm-row pa-0"
      >
        <v-col cols="12" sm="6" class="left px-9 py-8">
          <div class="heading2">Monthly Subscription</div>
          <div class="subheading2 mt-2 d-flex align-center">
            $29 <span class="pm ml-3">per month</span>
          </div>
          <div class="para2 my-1">Full access for less than $1 a day</div>
          <v-btn
            class="btn text-capitalize mt-5"
            elevation="8"
            block
            size="large"
            >Sign Up</v-btn
          >
        </v-col>
        <v-col cols="12" sm="6" class="right px-10 py-8">
          <div class="heading3 mb-3">Why Us</div>
          <div class="para3">
            Tutorials by industry experts <br />
            Peer & expert code review <br />
            Coding exercises <br />
            Access to our GitHub repos <br />
            Community forum <br />
            Flashcard decks <br />
            New videos every week
          </div>
        </v-col>
      </v-col>
    </v-row>
  </v-container>
</template>

<style scoped>
@font-face {
  font-family: f1;
  src: url(/src/assets/Karla-SemiBold.ttf);
}
@font-face {
  font-family: f2;
  src: url(/src/assets/Karla-Regular.ttf);
}
@font-face {
  font-family: f3;
  src: url(/src/assets/Karla-Bold.ttf);
}
/* TOP */
.top {
  background-color: #fff;
  border-top-left-radius: 5px;
  border-top-right-radius: 5px;
  border-bottom-left-radius: 0px;
  border-bottom-right-radius: 0px;
}
.heading1 {
  color: hsl(179, 61%, 44%);
  font-size: 20px;
  letter-spacing: -1px;
  font-family: f3;
}
.subheading1 {
  color: hsl(71, 73%, 54%);
  font-size: 16px;
  font-family: f3;
}
.para1 {
  color: hsl(218, 22%, 67%);
  font-size: 14px;
  line-height: 21px;
  letter-spacing: 0px;
  font-family: f2;
}

/* LEFT */
.left {
  background-color: hsl(179, 61%, 44%);
  border-bottom-left-radius: 5px;
}
.pm {
  font-size: 14px;
  color: hsl(180, 58%, 64%);
}
.subheading2 {
  font-size: 30px;
}
.para2 {
  font-size: 13px;
  color: hsl(181, 87%, 85%);
  letter-spacing: 1px;
}
.btn {
  background-color: hsl(71, 73%, 54%);
  font-size: 13px;
}

/* RIGHT */
.right {
  background-color: hsl(179, 47%, 52%);
  border-bottom-right-radius: 5px;
}
.heading3 {
  color: white;
}
.para3 {
  color: hsl(179, 61%, 74%);
  font-size: 12px;
}

@media screen and (max-width: 599.5px) {
  .left {
    border-top-left-radius: 0px;
    border-top-right-radius: 0px;
    border-bottom-left-radius: 0px;
    border-bottom-right-radius: 0px;
  }
  .right {
    border-top-left-radius: 0px;
    border-top-right-radius: 0px;
    border-bottom-left-radius: 5px;
    border-bottom-right-radius: 5px;
  }
}
</style>