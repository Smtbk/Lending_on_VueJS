<template>
	<div class="modal fade" id="modal" tabindex="-1">
    <div class="modal-dialog">
      <div class="modal-content">
        <div class="modal-header">
          <button type="button" class="btn-close" data-bs-dismiss="modal"></button>
        </div>
				
        <div class="modal-body">
          <p>Бронирование подтвержденно</p>
        </div>
				
        <div class="modal-footer">
          <button type="button" class="btn" data-bs-dismiss="modal">ОК</button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    name: 'ModalWin',
    methods: {
      close() {
        this.$emit('close');
      }
    }
  };
</script>