<template>
  <div class="footer">
    <h1>Ableton</h1>
    <section>
      <div>
        <ul>
          <li>Register Live or Push</li>
          <li>About Ableton</li>
          <li>Jobs</li>
        </ul>

        <ul>
          <li><strong>Community</strong></li>
          <li>Find Ableton User Groups</li>
          <li>Find Certified Training</li>
          <li>Become a Certified Trainer</li>
        </ul>
      </div>

      <div>
        <ul>
          <li><strong>Education</strong></li>
          <li>Offers for students and teachers</li>
          <li>Ableton for the Classroom</li>
          <li>Ableton for Colleges and Universities</li>
        </ul>

        <ul>
          <li><strong>Distributors</strong></li>
          <li>Find Distributors</li>
          <li>Try Push in-store</li>
        </ul>
      </div>

      <div>
        <ul class="medium-hidden">
          <li><strong>Sign up to our newsletter</strong></li>
          <li>
            Enter your email address to stay up to date with the latest offers,
            tutorials, downloads, surveys and more.
          </li>
          <input />
        </ul>
      </div>
    </section>

    <div class="section-c">
      <ul>
        <li>
          <small><strong>Archive</strong></small>
        </li>
        <li>
          <small><strong>Contact Us</strong></small>
        </li>
        <li>
          <small><strong>Press resources</strong></small>
        </li>
        <li>
          <small><strong>Legal Info</strong></small>
        </li>
        <li>
          <small><strong>Privacy policy</strong></small>
        </li>
        <li>
          <small><strong>Cookie Settings</strong></small>
        </li>
        <li>
          <small><strong>Imprint</strong></small>
        </li>
      </ul>
      <div class="logo-container">
        <Logo />
        <span><small>Made in Berlin</small></span>
      </div>
    </div>
  </div>
</template>

<script>
import Logo from "./Logo.vue";

export default {
  name: "Footer",
  components: {
    Logo,
  },
};
</script>
<style lang="scss" scoped>
.footer {
  min-width: 100%;
  display: flex;
  flex-direction: column;
  padding: 2rem 5rem;
  font-size: 1.3rem;

  h1 {
    text-align: start;
  }

  section {
    display: flex;
    flex-direction: column;
    margin: 3rem 0;
    
    ul {
      font-family: futuraPTLight, Avenir, -apple-system, BlinkMacSystemFont,
        "Segoe UI", sans-serif;
      font-weight: bold;
      margin: 1rem 0;
      min-height: 160px;

      li {
          strong {
              font-family: futuraPT, Avenir, -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif;
          }
      }
    }
  }

  .section-c {
      display: flex;
      flex-direction: column;
      justify-content: space-between;
  }

  .logo-container {
    display: flex;
    height: 100%;
    flex-direction: row;
    justify-content: start;
    align-items: end;
    position: relative;
    margin-top: 2rem;

    small {
        font-size: 1rem;
    }
  }

  ul {
    display: flex;
    display: space-between;
    min-height: 5rem;
    min-width: 400px;
    max-width: 500px;
    flex-wrap: wrap;
    flex-direction: column;
    text-align: start;

    li {
    }
  }

  /* larger devices */
  @media only screen and (min-width: 1000px) {
    ul {
      max-height: 10rem;
    }
    
    section,
    .section-c {
      flex-direction: row;
      align-items: start;
    }
    .section-c > ul {
      flex-direction: row;
      max-width: 100%;
      min-height: auto;
      align-content: baseline;

      li {
        margin-right: 18px;
        line-height: 1.5;
        font-size: 1rem;
      }
    }

    .logo-container {
      margin-top: 0;
    }
  }
}
</style>
