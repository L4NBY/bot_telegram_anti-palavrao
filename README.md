# anti palavrão telegram bot 

# Emxeplo 
Caso a pessoa chiga no grupo o bot vai dar um aviso apenas, Caso queira que o bot da ban , meu número ai wa.me/+557798119294  vou estar encinado 

# código

```

###########        
def menu_sempre(sempre):
    return True
@bot.message_handler(func=menu_sempre)
def messa(sempre):
    print(f'''MENSAGEM {sempre.from_user.first_name}''')
    l = {'Filho da puta',
'Caralho',
'Fdp',
'Arrombado',
'Lammer',
'Maldito',
'Golpista',
'Preto','viado','Viado',
'gay' , 'feio','Gay' , 'burro' , 'ladrão'}
    
    for c in l:
       
        if re.search(c, sempre.text):
            chigar = bot.send_message(sempre.chat.id , f'''😱Ei @{sempre.from_user.first_name} parece que você usou uma palavra proibida.

🔇Palavra proibida:**{c}**

⛔️Essa atitude pode levar ao seu banimento, pense bem antes de tentar novamente.''', parse_mode='Markdown')
            
            bot.delete_message(sempre.chat.id , sempre.id)
            sleep(10)
            bot.delete_message(sempre.chat.id , chigar.id)
            
        else:
            pass        
    ###########chigar##############
```
