<script>
export default {
  name: 'ErrorPage',
  props: {
    error: Object
  },
  beforeCreate() {
    if (process.client) {
      window.location.replace('/dashboard/login');
    }
  },
  render: () => null
}
</script>
