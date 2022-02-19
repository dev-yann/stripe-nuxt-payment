<template>
  <div
    class="relative flex items-top justify-center min-h-screen bg-gray-100 sm:items-center sm:pt-0"
  >
    <link
      href="https://cdn.jsdelivr.net/npm/tailwindcss@2.1.2/dist/tailwind.min.css"
      rel="stylesheet"
    />
    <div class="max-w-4xl mx-auto sm:px-6 lg:px-8">
      <a
        class="flex justify-center pt-8 sm:pt-0"
        href="https://nuxtjs.org"
        target="_blank"
      >
        <svg
          width="218"
          height="45"
          viewBox="0 0 159 30"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
        >
          <path
            d="M55.5017 6.81866H60.1727L70.0719 22.9912V6.81866H74.3837V29.7345H69.7446L59.8135 13.5955V29.7345H55.5017V6.81866Z"
            fill="#003543"
          />
          <path
            d="M93.657 29.7344H89.6389V27.1747C88.7241 28.9761 86.8628 29.9904 84.5113 29.9904C80.7869 29.9904 78.3684 27.3059 78.3684 23.4423V13.2339H82.3865V22.5976C82.3865 24.8566 83.7594 26.4276 85.8171 26.4276C88.0712 26.4276 89.6389 24.6598 89.6389 22.2377V13.2339H93.657V29.7344Z"
            fill="#003543"
          />
          <path
            d="M107.64 29.7344L103.784 24.2342L99.9291 29.7344H95.6492L101.596 21.1242L96.1074 13.2339H100.485L103.784 17.9821L107.051 13.2339H111.461L105.94 21.1242L111.886 29.7344H107.64Z"
            fill="#003543"
          />
          <path
            d="M120.053 8.25848V13.2339H124.627V16.6063H120.053V24.7974C120.053 25.0725 120.162 25.3363 120.356 25.531C120.55 25.7257 120.813 25.8353 121.087 25.8357H124.627V29.728H121.98C118.386 29.728 116.035 27.6323 116.035 23.9687V16.6095H112.801V13.2339H114.83C115.776 13.2339 116.327 12.6692 116.327 11.7349V8.25848H120.053Z"
            fill="#003543"
          />
          <path
            d="M134.756 24.5446V6.81866H139.066V23.1864C139.066 27.6067 136.943 29.7345 133.349 29.7345H128.332V25.8421H133.461C133.804 25.8421 134.134 25.7054 134.377 25.4621C134.619 25.2188 134.756 24.8888 134.756 24.5446Z"
            fill="#003543"
          />
          <path
            d="M141.649 22.0409H145.799C146.029 24.6006 147.728 26.2308 150.472 26.2308C152.923 26.2308 154.623 25.2501 154.623 23.2199C154.623 18.3085 142.331 21.7129 142.331 12.9395C142.334 9.17515 145.568 6.55945 150.215 6.55945C155.05 6.55945 158.317 9.34153 158.516 13.6306H154.388C154.193 11.6341 152.632 10.2918 150.207 10.2918C147.953 10.2918 146.548 11.3397 146.548 12.9427C146.548 18.0173 159 14.2226 159 23.1576C159 27.4131 155.504 30 150.474 30C145.279 30 141.882 26.8563 141.654 22.0441"
            fill="#003543"
          />
          <path
            d="M24.7203 29.704H41.1008C41.6211 29.7041 42.1322 29.5669 42.5828 29.3061C43.0334 29.0454 43.4075 28.6704 43.6675 28.2188C43.9275 27.7672 44.0643 27.2549 44.0641 26.7335C44.0639 26.2121 43.9266 25.6999 43.6662 25.2485L32.6655 6.15312C32.4055 5.70162 32.0315 5.32667 31.581 5.06598C31.1305 4.8053 30.6195 4.66805 30.0994 4.66805C29.5792 4.66805 29.0682 4.8053 28.6177 5.06598C28.1672 5.32667 27.7932 5.70162 27.5332 6.15312L24.7203 11.039L19.2208 1.48485C18.9606 1.03338 18.5864 0.658493 18.1358 0.397853C17.6852 0.137213 17.1741 0 16.6538 0C16.1336 0 15.6225 0.137213 15.1719 0.397853C14.7213 0.658493 14.3471 1.03338 14.0868 1.48485L0.397874 25.2485C0.137452 25.6999 0.000226653 26.2121 2.8053e-07 26.7335C-0.000226092 27.2549 0.136554 27.7672 0.396584 28.2188C0.656614 28.6704 1.03072 29.0454 1.48129 29.3061C1.93185 29.5669 2.44298 29.7041 2.96326 29.704H13.2456C17.3195 29.704 20.3239 27.9106 22.3912 24.4118L27.4102 15.7008L30.0986 11.039L38.1667 25.0422H27.4102L24.7203 29.704ZM13.0779 25.0374L5.9022 25.0358L16.6586 6.36589L22.0257 15.7008L18.4322 21.9401C17.0593 24.2103 15.4996 25.0374 13.0779 25.0374Z"
            fill="#00DC82"
          />
        </svg>
      </a>
      <div class="mt-8 bg-white overflow-hidden shadow sm:rounded-lg p-6">
        <div
          v-show="isDisplaySkeleton"
          class="w-60 h-24 border-2 rounded-md mx-auto mt-20"
        >
          <div
            class="flex animate-pulse flex-row items-center h-full justify-center space-x-5"
          >
            <div class="w-12 bg-gray-300 h-12 rounded-full"></div>
            <div class="flex flex-col space-y-3">
              <div class="w-36 bg-gray-300 h-6 rounded-md"></div>
              <div class="w-24 bg-gray-300 h-6 rounded-md"></div>
            </div>
          </div>
        </div>
        <form v-show="isDisplayForm" id="payment-form" @submit="handleSubmit">
          <div v-show="!confirm" id="payment-element">
            <!-- Elements will create form elements here -->
          </div>
          <button v-show="!confirm" ref="submit" class="mt-8">
            <div ref="spinner" class="spinner hidden"></div>
            <span ref="submitText">Pay now</span>
          </button>
        </form>
        <div ref="message">
          <!-- Display error message to your customers here -->
        </div>
      </div>
      <div class="flex justify-center pt-4 space-x-2">
        <a href="https://github.com/nuxt/nuxt.js" target="_blank"
          ><svg
            class="w-6 h-6 text-gray-600 hover:text-gray-800 button&#45;&#45;github"
            xmlns="http://www.w3.org/2000/svg"
            xmlns:xlink="http://www.w3.org/1999/xlink"
            aria-hidden="true"
            role="img"
            width="32"
            height="32"
            preserveAspectRatio="xMidYMid meet"
            viewBox="0 0 24 24"
          >
            <path
              d="M12 2.247a10 10 0 0 0-3.162 19.487c.5.088.687-.212.687-.475c0-.237-.012-1.025-.012-1.862c-2.513.462-3.163-.613-3.363-1.175a3.636 3.636 0 0 0-1.025-1.413c-.35-.187-.85-.65-.013-.662a2.001 2.001 0 0 1 1.538 1.025a2.137 2.137 0 0 0 2.912.825a2.104 2.104 0 0 1 .638-1.338c-2.225-.25-4.55-1.112-4.55-4.937a3.892 3.892 0 0 1 1.025-2.688a3.594 3.594 0 0 1 .1-2.65s.837-.262 2.75 1.025a9.427 9.427 0 0 1 5 0c1.912-1.3 2.75-1.025 2.75-1.025a3.593 3.593 0 0 1 .1 2.65a3.869 3.869 0 0 1 1.025 2.688c0 3.837-2.338 4.687-4.563 4.937a2.368 2.368 0 0 1 .675 1.85c0 1.338-.012 2.413-.012 2.75c0 .263.187.575.687.475A10.005 10.005 0 0 0 12 2.247z"
              fill="currentColor"
            /></svg
        ></a>
        <a href="https://twitter.com/nuxt_js" target="_blank"
          ><svg
            class="w-6 h-6 text-gray-600 hover:text-gray-800"
            xmlns="http://www.w3.org/2000/svg"
            xmlns:xlink="http://www.w3.org/1999/xlink"
            aria-hidden="true"
            role="img"
            width="32"
            height="32"
            preserveAspectRatio="xMidYMid meet"
            viewBox="0 0 24 24"
          >
            <path
              d="M22.46 6c-.77.35-1.6.58-2.46.69c.88-.53 1.56-1.37 1.88-2.38c-.83.5-1.75.85-2.72 1.05C18.37 4.5 17.26 4 16 4c-2.35 0-4.27 1.92-4.27 4.29c0 .34.04.67.11.98C8.28 9.09 5.11 7.38 3 4.79c-.37.63-.58 1.37-.58 2.15c0 1.49.75 2.81 1.91 3.56c-.71 0-1.37-.2-1.95-.5v.03c0 2.08 1.48 3.82 3.44 4.21a4.22 4.22 0 0 1-1.93.07a4.28 4.28 0 0 0 4 2.98a8.521 8.521 0 0 1-5.33 1.84c-.34 0-.68-.02-1.02-.06C3.44 20.29 5.7 21 8.12 21C16 21 20.33 14.46 20.33 8.79c0-.19 0-.37-.01-.56c.84-.6 1.56-1.36 2.14-2.23z"
              fill="currentColor"
            /></svg
        ></a>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import { Context } from '@nuxt/types'
import { Component, Ref, Vue } from 'nuxt-property-decorator'

@Component
export default class indexPage extends Vue {
  private secret!: string
  private stripeElement: any
  private confirm: boolean = false

  private skeletonLoader: boolean = true

  @Ref() readonly submit!: HTMLButtonElement
  @Ref() readonly spinner!: HTMLDivElement
  @Ref() readonly message!: HTMLDivElement
  @Ref() readonly submitText!: HTMLSpanElement

  async asyncData(ctx: Context): Promise<object | null> {
    const secret = await ctx.$axios.$get('/api/secret')

    return {
      secret,
    }
  }

  mounted() {
    const querySecret = new URLSearchParams(window.location.search).get(
      'payment_intent_client_secret'
    )

    if (querySecret) {
      this.confirm = true
      this.checkStatus(querySecret)
      return
    }

    if (this.$stripe) {
      this.stripeElement = this.$stripe.elements({ clientSecret: this.secret })

      this.stripeElement
        .create('payment', {})
        .on('ready', () => {
          this.skeletonLoader = false
        })
        .mount('#payment-element')
    }
  }

  // Show a spinner on payment submission
  setLoading(isLoading: boolean) {
    if (isLoading) {
      // Disable the button and show a spinner
      this.submit.disabled = true
      this.spinner.classList.remove('hidden')
      this.submitText.classList.add('hidden')
    } else {
      this.submit.disabled = false
      this.spinner.classList.add('hidden')
      this.submitText.classList.remove('hidden')
    }
  }

  async handleSubmit(e: any) {
    e.preventDefault()
    this.setLoading(true)

    const { error } = await this.$stripe!.confirmPayment({
      elements: this.stripeElement,
      confirmParams: {
        // Make sure to change this to your payment completion page
        return_url: 'http://localhost:3000',
      },
    })

    // This point will only be reached if there is an immediate error when
    // confirming the payment. Otherwise, your customer will be redirected to
    // your `return_url`. For some payment methods like iDEAL, your customer will
    // be redirected to an intermediate site first to authorize the payment, then
    // redirected to the `return_url`.
    if (error.type === 'card_error' || error.type === 'validation_error') {
      this.showMessage(error.message ? error.message : 'empty error')
    } else {
      this.showMessage('An unexpected error occured.')
    }

    this.setLoading(false)
  }

  showMessage(messageText: string) {
    this.message.classList.remove('hidden')
    this.message.textContent = messageText
  }

  async checkStatus(secret: string) {
    const { paymentIntent } = await this.$stripe!.retrievePaymentIntent(secret)

    if (paymentIntent) {
      switch (paymentIntent.status) {
        case 'succeeded':
          this.showMessage('Payment succeeded!')
          break
        case 'processing':
          this.showMessage('Your payment is processing.')
          break
        case 'requires_payment_method':
          this.showMessage('Your payment was not successful, please try again.')
          break
        default:
          this.showMessage('Something went wrong.')
          break
      }
    }
  }

  get isDisplayForm(): boolean {
    return !this.confirm && !this.skeletonLoader
  }

  get isDisplaySkeleton(): boolean {
    return this.skeletonLoader && !this.confirm
  }
}
</script>

<style lang="css" scoped>
/* Buttons and links */
button {
  background: #5469d4;
  font-family: Arial, sans-serif;
  color: #ffffff;
  border-radius: 4px;
  border: 0;
  padding: 12px 16px;
  font-size: 16px;
  font-weight: 600;
  cursor: pointer;
  display: block;
  transition: all 0.2s ease;
  box-shadow: 0px 4px 5.5px 0px rgba(0, 0, 0, 0.07);
  width: 100%;
}
button:hover {
  filter: contrast(115%);
}
button:disabled {
  opacity: 0.5;
  cursor: default;
}

/* spinner/processing state, errors */
.spinner,
.spinner:before,
.spinner:after {
  border-radius: 50%;
}
.spinner {
  color: #ffffff;
  font-size: 22px;
  text-indent: -99999px;
  margin: 0px auto;
  position: relative;
  width: 20px;
  height: 20px;
  box-shadow: inset 0 0 0 2px;
  -webkit-transform: translateZ(0);
  -ms-transform: translateZ(0);
  transform: translateZ(0);
}
.spinner:before,
.spinner:after {
  position: absolute;
  content: '';
}
.spinner:before {
  width: 10.4px;
  height: 20.4px;
  background: #5469d4;
  border-radius: 20.4px 0 0 20.4px;
  top: -0.2px;
  left: -0.2px;
  -webkit-transform-origin: 10.4px 10.2px;
  transform-origin: 10.4px 10.2px;
  -webkit-animation: loading 2s infinite ease 1.5s;
  animation: loading 2s infinite ease 1.5s;
}
.spinner:after {
  width: 10.4px;
  height: 10.2px;
  background: #5469d4;
  border-radius: 0 10.2px 10.2px 0;
  top: -0.1px;
  left: 10.2px;
  -webkit-transform-origin: 0px 10.2px;
  transform-origin: 0px 10.2px;
  -webkit-animation: loading 2s infinite ease;
  animation: loading 2s infinite ease;
}

@-webkit-keyframes loading {
  0% {
    -webkit-transform: rotate(0deg);
    transform: rotate(0deg);
  }
  100% {
    -webkit-transform: rotate(360deg);
    transform: rotate(360deg);
  }
}
@keyframes loading {
  0% {
    -webkit-transform: rotate(0deg);
    transform: rotate(0deg);
  }
  100% {
    -webkit-transform: rotate(360deg);
    transform: rotate(360deg);
  }
}
</style>
