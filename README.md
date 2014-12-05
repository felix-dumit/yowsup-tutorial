yowsup-tutorial
===============

como usar yowsup2:

##Registro
É necessário obter uma senha para registrar seu número de telefone. 
Nota: o número será desvinculado de qualquer telefone já cadastrado

Para isso execute o comando

```python
python yowsup-cli registration --requestcode sms --phone 55XXXXXXXX --cc 55 
```
 
 Após receber a mensagem de sms com o código execute o comando:
 
```python
python yowsup-cli registration --register CODIGO_RECEBIDO --phone 55XXXXXXXX --cc 55  
```

Anote o valor retornado para o campo **login** e **pw**, substitua estes valores para o arquivo ```run.py```na linha 19


##Execução

```python run.py```

O script retornará de volta para o remetente qualquer imagem ou texto enviado
