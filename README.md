# Helper Components to easier use Heroicons in Vue

I was tired of importing every icon in each component one by one. That's why I've build myself this little helper components to import the icons more easy. I am new to Vue, so I am not sure whether or not this is a good approach. Suggestions welcome.

## Usage Now

Now any icon can be used with one single import and export. 

```vue
<template>
  <icon-outline name="SunIcon"/>
  <icon-outline name="StarIcon"/>
  <icon-outline name="PlayIcon"/>
</template>

<script>
import IconOutline from "@/Components/IconOutline.vue";

export default {
  components: {
    IconOutline,
  },
}
</script>
```

## Usage Before

Before every icon must be imported and exported one by one.

```vue
<template>
  <SunIcon>
  <StarIcon>
  <PlayIcon>
</template>

<script>
import { 
    SunIcon, 
    StarIcon, 
    PlayIcon } from '@heroicons/vue/outline'

export default {
  components: {
    SunIcon, 
    StarIcon, 
    PlayIcon    
  },
}
</script>
```

## Credits / Based on
https://github.com/zaydek/heroicons.dev

https://github.com/tailwindlabs/heroicons
