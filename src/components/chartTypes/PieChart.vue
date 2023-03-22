<!-- Copyright(c) 2023, Carlos Astengo, All Rights Reserved -->

<script lang="ts">
import { defineComponent, h } from 'vue';

import { GChart } from 'vue-google-charts';

export const type = 'PieChart';

export const data = [
  ['Task', 'Hours per Day'],
  ['Work', 11],
  ['Eat', 2],
  ['Commute', 2],
  ['Watch TV', 2],
  ['Sleep', 7],
];

export const options = {
  title: 'My Daily Activities',
  width: 450,
  height: 250,
};

export default defineComponent({
  name: 'GoogleChart',
  components: {
    GChart,
  },
  setup() {
    return () =>
      h(GChart, {
        data,
        options,
        type,
      });
  },
});
</script>