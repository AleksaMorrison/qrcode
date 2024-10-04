<script setup> 
</script>

<template>
  <div class="qrcode-wrap">
    <div class="qrcode">
      <img src="../assets/image-qr-code.png" alt="qr-code">
      <div class="qrcode-text">
        <p class="text-1">Improve your front-end skills by building projects</p>
        <p class="text-2">Scan the QR code to visit Frontend Mentor and take your coding skills to the next level</p>
      </div>
    </div>
    <div class="attribution">
      <p>
        Challenge by <a href="https://www.frontendmentor.io?ref=challenge" target="_blank">Frontend Mentor</a>. 
        Coded by <a href="https://github.com/AleksaMorrison">Aleksandra Morrison</a>.
      </p>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.qrcode-wrap {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  background-color: var(--white);
  border-radius: 20px;
  padding: var(--spacing-200);
  padding-bottom: var(--spacing-500);
  width: 320px;
  box-shadow: var(--shadow);
  height: min-content;
   
  & .qrcode {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: flex-start;
    gap: var(--spacing-300);

    &-text {
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      padding-left: var(--spacing-200);
      padding-right: var(--spacing-200);
      gap: var(--spacing-200);

      & p {
        margin-top: 0;
        margin-bottom: 0;
        text-align: center;
      }

      & .text-1 {
        font-weight: 700;
        font-size: 22px;
        line-height: 120%;
        letter-spacing: 0px;
      }

      & .text-2 {
        color: var(--slate-500);
        font-weight: 500;
        font-size: 15px;
        line-height: 140%;
        letter-spacing: 0.2px;
      }
    }

    & img {
      width: 100%;
      height: auto;
    }

  }

  & .attribution { 
      display: none;
      font-size: 11px; text-align: center;
      & a { 
        color: hsl(228, 45%, 44%); 
        &:hover { 
          text-decoration: underline; 
        }
      }
    }
}
</style>
