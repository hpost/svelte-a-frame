<script>
  export let pointerLock = true
</script>

<a-entity id="rig" movement-controls="controls: gamepad, touch">
  <a-camera position="0 1.6 0" look-controls="pointerLockEnabled: {pointerLock}"></a-camera>
</a-entity>