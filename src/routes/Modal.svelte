<!-- Modal.svelte -->
  <script>
export let show = false;
</script> 
{#if show}
<div class="modal-backdrop">
     <div class="modal-content">
         <slot></slot>
</div> </div>
{/if} 
<style>
.modal-backdrop {
     position: fixed; 
     top: 0;
      left: 0;
width: 100%; 
height: 100%;
background: rgba(0, 0, 0, 0.5); 
display: flex;
justify-content: center; 
align-items: center;
}
 .modal-content {
background: white;
 padding: 1rem; 
 border-radius: 8px;
} 
</style>