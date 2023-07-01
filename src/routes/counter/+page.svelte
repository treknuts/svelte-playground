<script lang="ts">
  import { count } from "../../stores/countStore";

  let count_value: number;

  count.subscribe((value) => {
    count_value = value;
  });
</script>

<div class="h-full flex-grow grid place-content-center">
  <h4 class="text-3xl">
    You have clicked <span class="text-info">{count_value}</span> times.
  </h4>
  <button class="btn btn-info" on:click={() => count.update((n) => n + 1)}
    >Click me!</button
  >
</div>
