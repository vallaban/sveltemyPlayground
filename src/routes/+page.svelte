<script>
    import Modal from './Modal.svelte'; 
    let showModal = false;
    function openModal() 
    { 
        showModal = true;
    }
    function closeModal() 
    { 
        showModal = false;
    } 
    </script>
     <button on:click={openModal}>Open Modal</button>
    <Modal show={showModal} on:click={closeModal}> <h2>Modal Title</h2>
    <p>This is the modal content.</p>
     <button on:click={closeModal}>Close</button>
    </Modal>