<script>
  export let width = 16
  export let height = 16
  export let name = ''
  export let color = 'currentColor'
</script>

<svg
  xmlns="http://www.w3.org/2000/svg"
  {width}
  {height}
  viewBox="0 0 20 20"
  aria-labelledby={name}
  role="presentation"
>
  <title id={name} lang="en">{`${name} icon`}</title>
  <g fill={color}>
    <slot />
  </g>
</svg>

<style>
  svg {
    display: inline-block;
    vertical-align: middle;
  }
</style>
