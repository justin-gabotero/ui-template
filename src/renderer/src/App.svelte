<script lang="ts">
  // ipc handle
  const ipcHandle = () => {
    window.electron.ipcRenderer.send('ping')
  }
</script>

<div class="action">
  ipc button
  <button on:click={ipcHandle}>ping</button>
</div>
