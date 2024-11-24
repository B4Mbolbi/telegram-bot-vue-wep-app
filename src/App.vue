<div>
<img :src="TWA.initDataUnsafe.user.photo_url">
</div>
<div style="width: 100%; height: 100%;background: #008CBA">
<!-- ... -->
<button @click="closeAppAndSendData()">Закрыть и отправить данные</button>
</div>

<script>
export default {
  methods: {
    closeAppAndSendData() {
      // Отправить данные в Telegram бот
      fetch(`https://api.telegram.org/bot7933334930:AAEJlGJbaLow8rxkNjo2DNthF6YuRRO648A/sendMessage`, {
        method: 'POST',
        headers: { 'Content-Type': 'application/json' },
        body: JSON.stringify({
          chat_id: TWA.initDataUnsafe.user.id,
          text: `Данные: ${JSON.stringify(TWA.initDataUnsafe)}`,
        }),
      })
          .then(() => {
            // Закрыть приложение
            window.close();
          })
          .catch((error) => {
            console.error('Ошибка отправки данных:', error);
          });
    },
  },
};
</script>