<script lang="ts">
  const playKey = (index: number) => {
    if (!index || index <= 0 || index > 23) {
      return;
    }

    const audio = new Audio(`/sounds/key-${index}.mp3`);
    audio.play();
  };
</script>

<svg
  width="1387"
  height="467"
  viewBox="0 0 1387 467"
  fill="none"
  xmlns="http://www.w3.org/2000/svg"
  class="piano"
>
  <path
    d="M638.996 44.2128L740.544 30.4131L714.007 451.115H651.516L638.996 44.2128Z"
    class="key key--white"
    on:click={() => playKey(1)}
  />
  <path
    d="M627.456 442.886L525.908 456.686L552.445 35.9836L614.936 35.9836L627.456 442.886Z"
    class="key key--white"
    on:click={() => playKey(2)}
  />
  <path
    d="M942.914 437.315L841.366 451.115L867.903 30.4131L930.395 30.4131L942.914 437.315Z"
    class="key key--white"
    on:click={() => playKey(3)}
  />
  <path
    d="M323.538 49.7834L425.086 35.9836L398.549 456.686L336.057 456.686L323.538 49.7834Z"
    class="key key--white"
    on:click={() => playKey(4)}
  />
  <path
    d="M1266.25 51.0879L1367.8 37.2881L1341.26 457.99H1278.77L1266.25 51.0879Z"
    class="key key--white"
    on:click={() => playKey(5)}
  />
  <path
    d="M1266.25 444.19L1179.45 457.99L1170.96 37.2881L1244.45 37.2881L1266.25 444.19Z"
    class="key key--white"
    on:click={() => playKey(6)}
  />
  <path
    d="M0.198484 42.9083L86.9996 29.1086L95.4927 449.811L22.0025 449.811L0.198484 42.9083Z"
    class="key key--white"
    on:click={() => playKey(7)}
  />
  <path
    d="M1166.36 426.108L1066.54 449.292L1053.83 27.9453L1132.51 27.9451L1166.36 426.108Z"
    class="key key--white"
    on:click={() => playKey(8)}
  />
  <path
    d="M100.091 60.9909L199.916 37.8068L212.62 459.154L133.938 459.154L100.091 60.9909Z"
    class="key key--white"
    on:click={() => playKey(9)}
  />
  <path
    d="M1052.91 462.278L964.417 453.282L971.021 31.7954L1033.44 28.8389L1052.91 462.278Z"
    class="key key--white"
    on:click={() => playKey(10)}
  />
  <path
    d="M213.545 24.821L302.035 33.8169L295.431 455.303L233.01 458.26L213.545 24.821Z"
    class="key key--white"
    on:click={() => playKey(11)}
  />
  <path
    d="M751.992 30.4131L855.696 30.4131L813.855 451.115H742.286L751.992 30.4131Z"
    class="key key--white"
    on:click={() => playKey(12)}
  />
  <path
    d="M514.46 456.686L410.756 456.686L452.597 35.9836L524.166 35.9836L514.46 456.686Z"
    class="key key--white"
    on:click={() => playKey(13)}
  />
  <path
    d="M50.2409 20.4357L121.598 19.5728L127.98 269.937L71.194 270.624L50.2409 20.4357Z"
    class="key key--black"
    on:click={() => playKey(14)}
  />
  <path
    d="M255.13 11.8923L188.438 13.8596L189.947 264.228L243.021 262.663L255.13 11.8923Z"
    class="key key--black"
    on:click={() => playKey(15)}
  />
  <path
    d="M666.823 23.7702L600.131 25.7375L601.64 276.106L654.713 274.541L666.823 23.7702Z"
    class="key key--black"
    on:click={() => playKey(16)}
  />
  <path
    d="M416.443 9.5631L459.528 15.9547L445.694 265.656L411.407 260.57L416.443 9.5631Z"
    class="key key--black"
    on:click={() => playKey(17)}
  />
  <path
    d="M826.095 8.69799L877.949 11.8464L878.363 262.021L837.098 259.516L826.095 8.69799Z"
    class="key key--black"
    on:click={() => playKey(18)}
  />
  <path
    d="M980.986 291.443L921.019 285.153L935.293 13.1079L983.015 18.1132L980.986 291.443Z"
    class="key key--black"
    on:click={() => playKey(19)}
  />
  <path
    d="M1188.97 286.865L1134.4 284.46L1127.89 12.187L1171.32 14.1007L1188.97 286.865Z"
    class="key key--black"
    on:click={() => playKey(20)}
  />
  <path
    d="M1286.92 279.16L1232.57 273.722L1241.22 1.50762L1284.47 5.8349L1286.92 279.16Z"
    class="key key--black"
    on:click={() => playKey(21)}
  />
  <path
    d="M1384.88 289.883L1330.52 284.445L1321.41 28.6993L1382.42 16.5584L1384.88 289.883Z"
    class="key key--black"
    on:click={() => playKey(22)}
  />
  <path
    d="M499.081 14.3453L557.845 15.7525L562.558 265.969L515.794 264.849L499.081 14.3453Z"
    class="key key--black"
    on:click={() => playKey(23)}
  />
</svg>

<style>
  svg {
    width: auto;
    height: auto;
  }

  .piano {
    position: absolute;
    inset: 50%;
    transform: translate(-50%, -50%);
    padding: 10%;
  }

  .key--white {
    fill: var(--white);
    transition: fill 100ms ease-in-out;
  }

  .key--white:hover,
  .key--white:active {
    fill: var(--yellow);
  }

  .key--black {
    fill: var(--black);
    transition: fill 100ms ease-in-out;
  }

  .key--black:hover,
  .key--black:active {
    fill: var(--pink);
  }
</style>
