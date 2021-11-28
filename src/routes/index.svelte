<script>
    import Greeting from "$lib/Greeting.svelte";
    import Entry from "$lib/Entry.svelte ";
    import EntryModal from "$lib/EntryModal.svelte";
</script>
<div class="bg-secondary text-white">
    <Greeting />
</div>
<!-- Entries -->
<section class="container p-3 bg-dark text-white">
    <div class="d-flex justify-content-between">
   	 <div class="p-2">Mood Log</div>
   	 <input class="btn btn-light mb-2" type="button" value="+ New Entry" data-bs-toggle="modal" data-bs-target="#newEntry"/>
    </div>

    <div class="list-group mb-3">
   	 <!-- Individual Entries -->
    	<Entry />
    </div>
</section>

<EntryModal />