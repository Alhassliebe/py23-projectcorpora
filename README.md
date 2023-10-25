# projectcorpora  

### • data_to_db.py  
В данном файле происходит парсинг сайтов с анекдотами и сохранение информации о них в базе данных anecdote.db

### • anecdote.db  
Собственно база данных, которая служит основой для нашего корпуса анекдотов

### • db_diagram
Схема базы данных anecdote.db, состоящей из 3 таблиц:  
  1. **meta** с инф-й об анекдотах (text_id - номер анекдота, source - ссылка на анекдот, full_text - полный текст анекдота)
  2. **sentences** с инф-й о предложениях (text_id, sent_id - номер предложения в тексте, sent - само предложение)
  3. **words** с инф-й о словах (text_id, sent_id, word_id - номер слова в предложении, word - слово, lemma - лемма, pos - часть речи)
