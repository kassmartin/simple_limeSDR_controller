Запустить simple_limeSDR_controller с аргументами:  

    --rx
        <номер ус-ва> - в нашем случае 0
        <канал ус-ва> - rx1 = 0, rx2 = 1
        <номер антены> - H = 1, L = 2, W = 3, AUTO = 255
        <кол-во повторов или 0> - 0 = пока не остановишь по ctrl+c
        <кол-во сэмплов для записи> - кратное 1024
        <сэплрейт> 
        <частота> 
        <усиление>
    К примеру, --rx 0 0 255 1 16384 2500000 50000000 10

    --tx
        <номер ус-ва> - в нашем случае 0
        <канал ус-ва> - TXx_1 = 0, TXx_2 = 1
        <номер антены> - TX1 = 1, TX2 = 2
        <кол-во повторов или 0> - 0 = пока не остановишь по ctrl+c
        <сэплрейт> 
        <частота> 
        <усиление>
        <имя файла в папке TX>
    К примеру, --tx 0 0 1 1 2500000 50000000 10 test_tx.bin
 
Скопировать из папки RX в TX
 cp RX/<захват>/<файл> TX/<файл>

Для сборки необходимо установить зависимости:
```bash
sudo apt install liblimesuite-dev limesuite-udev
```
