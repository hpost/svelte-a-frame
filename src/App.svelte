<script>
  import 'aframe'
  import 'aframe-extras'

  import Splash from './components/Splash.svelte'
  import CameraRig from './components/CameraRig.svelte'
  import SampleScene from './components/SampleScene.svelte'
</script>

<a-scene background="color: #FAFAFA">
  <Splash visible={true} />
  <SampleScene/>
  <CameraRig pointerLock={true}/>
</a-scene>