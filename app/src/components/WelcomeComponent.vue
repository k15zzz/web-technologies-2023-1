<template>
  <section class="welcome">
    <div class="bcg"></div>
    <div class="container">
      <div class="content">
        <div class="welcome-main">
          <h2>
            Development of <span>mobile applications</span> and <span>web services</span> of any complexity
          </h2>
          <p>
            We create mobile applications for iOS, Android that transfer your business to mobile applications of your
            customers' devices
          </p>
        </div>
        <div class="welcome-contact">
          <h3>
            Leave your contacts and we will call you back
            within 30 minutes
          </h3>
          <form action="" name="contact">
            <field-component
                label="Phone number"
                type="tel"
                placeholder="+7 (111) 111-11-11"
            />
            <field-component
                label="Full name"
                type="text"
                placeholder="Иванов Иван"
            />
            <input-button-component value="Get consultation"/>
          </form>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import FieldComponent from "@/components/UI/FieldComponent.vue";
import InputButtonComponent from "@/components/UI/InputButtonComponent.vue";

export default {
  name: "WelcomeComponent",
  components: {
    InputButtonComponent,
    FieldComponent
  }
}
</script>

<style lang="less" scoped>
section.welcome {
  width: 100%;
  height: 900px;
  background-color: var(--gray-100);

  .bcg {
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    background: url("@/assets/images/welcome.png") no-repeat right;
  }

  .container {
    margin: auto;

    .content {
      display: flex;
      flex-direction: column;
      gap: 40px;
      padding-top: 160px;

      .welcome-main {
        width: 600px;

        h2 {
          color: var(--gray-900, #101828);
          font-feature-settings: 'clig' off, 'liga' off;
          font-family: "Inter";
          font-size: 36px;
          font-style: normal;
          font-weight: 700;
          line-height: 144%; /* 51.84px */
          letter-spacing: 0.326px;

          span {
            color: var(--accent-low-opacity, #306FF5);
            font-feature-settings: 'clig' off, 'liga' off;
            font-family: Inter;
            font-size: 36px;
            font-style: normal;
            font-weight: 700;
            line-height: 144%;
            letter-spacing: 0.326px;
          }
        }

        p {
          margin-top: 24px;
          color: var(--gray-900);
          font-feature-settings: 'clig' off, 'liga' off;
          /* SF Text Medium */
          font-family: SF Pro Text;
          font-size: 15px;
          font-style: normal;
          font-weight: 500;
          line-height: 20px; /* 133.333% */
          letter-spacing: -0.24px;
        }
      }

      .welcome-contact {
        width: 676px;
        display: inline-flex;
        padding: 24px;
        flex-direction: column;
        justify-content: center;
        align-items: flex-start;
        gap: 32px;
        border-radius: 12px;
        background: var(--white);
        /* Elevation 32 pt */
        box-shadow: 0px 0px 24px 0px rgba(0, 0, 0, 0.16), 0px 0px 2px 0px rgba(0, 0, 0, 0.08);

        h3 {
          color: var(--gray-900, #101828);
          font-feature-settings: 'clig' off, 'liga' off;
          font-family: Inter;
          font-size: 20px;
          font-style: normal;
          font-weight: 700;
          line-height: 24px; /* 120% */
          letter-spacing: 0.38px;
        }

        form {
          display: flex;
          align-items: center;
          gap: 24px;
        }
      }
    }
  }
}
</style>