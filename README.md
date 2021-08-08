# Классификация эмоций пользователей по их текстовым сообщениям на русском языке <br>

ссылка на яндекс диск с docker контейнером и другими данными: https://disk.yandex.com/d/LVoQgG1jpR3UfQ

### Инструкция:

1. Скачать zip файл с яндекс диска

#### Запуск сервера
1. Скачать файл "tensorflow-server.tar" 
2. Открыть WindowsPowerShell
3. Ввести команды <br>
  <code> docker import tensorflow-server.tar </code> <br>
  <code> tensorflow_model_server --rest_api_port=8601 --model_name=senti_model --model_base_path=/project folder/saved_models/ </code> <br>
  <code> docker run -it -v C:\path\to\your\project folder:/project folder -p 8601:8601 --entrypoint /bin/bash tensorflow/serving </code> <br>
Сервер запущен!



