import discord
import requests
import time
import asyncio
client = discord.Client()
boseused = "0"
aniketused = "0"
ladkiused = "0"
aniket = "rahianiket"
bose = "soumyabose58"
ladki = "Andytheking"
one = 1

TOKEN = 'NTIwMTk4ODE4OTQwMDU5NjY3.DuqYww.PusbyRJKo6UgM9JkEoIwEv2qD2Q'

client = discord.Client()

@client.event
async def on_message(message):
    
    
    if message.content.startswith('lif'):
        refferal = message.content[4:]
        res = requests.get('http://sms-activate.ru/stubs/handler_api.php?api_key=4925eb317276f094b64c02dd8Add5be8&action=getNumber&service=kp&forward=0&operator=any&ref=123&country=32')
        print(res.content)
        data=res.content
        idnum=str(data)
        bal1 = idnum[5]
        bal2 = idnum[6]
        bal3 = idnum[7]
        bal4 = idnum[8]
        num1 = idnum[25]
        num2 = idnum[26]
        num3 = idnum[27]
        num4 = idnum[28]
        num5 = idnum[29]
        num6 = idnum[30]
        num7 = idnum[31]
        num8 = idnum[32]
        num9 = idnum[33]
        num10 = idnum[34]
        num11 = idnum[35]
        id1 = idnum[16]
        id2 = idnum[17]
        id3 = idnum[18]
        id4 = idnum[19]
        id5 = idnum[20]
        id6 = idnum[21]
        id7 = idnum[22]
        id8 = idnum[23]
        number = num1+num2+num3+num4+num5+num6+num7+num8+num9+num10+num11
        id = id1 + id2 + id3 + id4 + id5 + id6 + id7 + id8
        print("number is +40%s\n " % (number))
        msg = '+phone +%s\n' % (number).format(message)
        await client.send_message(message.channel, msg)
        ready = requests.get('http://sms-activate.ru/stubs/handler_api.php?api_key=4925eb317276f094b64c02dd8Add5be8&action=setStatus&status=1&id=%s' % (id))
        await asyncio.sleep(15)
        tes = requests.get('http://sms-activate.ru/stubs/handler_api.php?api_key=4925eb317276f094b64c02dd8Add5be8&action=getStatus&id=%s' % (id))
        data1=tes.content
        tata=str(data1)
        sms1 = tata[12]
        sms2 = tata[13]
        sms3 = tata[14]
        sms4 = tata[15]
        sms = sms1 + sms2 + sms3 + sms4
        cod = sms
        wait = "T_CO"
        nobal = "BALA"
        bal = bal1+bal2+bal3+bal4
        print(tes.content)
        print("otp is %s\n " % (sms))

        if sms.isdigit() == False:
            ban1 = requests.get('http://sms-activate.ru/stubs/handler_api.php?api_key=4925eb317276f094b64c02dd8Add5be8&action=getStatus&status=-1&id=%s' % (id))
            print(" not num ")

        if sms.isdigit() == True:
            print(" yes num ")
            msg = "+code "+cod+" %s\n" % (refferal).format(message)
            await client.send_message(message.channel, msg)
            ban2 = requests.get('http://sms-activate.ru/stubs/handler_api.php?api_key=4925eb317276f094b64c02dd8Add5be8&action=getStatus&status=8&id=%s' % (id))
            if message.author.name == aniket:
                intaniket = int(aniketused, 10)
                def globallychange():
                    global aniketused
                    intaniketused = intaniket + one
                    aniketused = str(intaniketused)
                globallychange()
                msg = "you made %s life\n" % (aniketused).format(message)
                await client.send_message(message.channel, msg)
            
            if message.author.name == bose:
                intbose = int(boseused, 10)
                def globallychange():
                    global boseused
                    intboseused = intbose + one
                    boseused = str(intboseused)
                globallychange()
                msg = "you made %s life\n" % (boseused).format(message)
                await client.send_message(message.channel, msg)

            if message.author.name == ladki:
                intladki = int(ladkiused, 10)
                def globallychange():
                    global ladkiused
                    intladkiused = intladki + one
                    ladkiused = str(intladkiused)
                globallychange()
                msg = "you made %s life\n" % (ladkiused).format(message)
                await client.send_message(message.channel, msg)

        if cod == wait:
           msg = 'lif %s' % (refferal).format(message)
           await client.send_message(message.channel, msg)
           print("getting new number")
     
        if bal == nobal:
           msg = 'NO BALANCE Contact @rahianiket for replishment \n' % (number).format(message)
           await client.send_message(message.channel, msg)
           print("No balance")

    if message.content.startswith('cbal'):

           balance = requests.get('http://sms-activate.ru/stubs/handler_api.php?api_key=4925eb317276f094b64c02dd8Add5be8&action=getBalance')
           ybal=balance.content
           balancey=str(ybal)
           print(balance.content)
           id2 = "0"
           id3 = "0"
           id4 = "0"
           id2 = balancey[17]
           id3 = balancey[18]
           id4 = balancey[19]
           ybal = id2+id3+id4
           msg = 'System balance is %s\n' % (ybal).format(message)
           await client.send_message(message.channel, msg)
           print("balance is sent")
           if message.author.name == aniket:
               msg = "you made %s life\n" % (aniketused).format(message)
               await client.send_message(message.channel, msg)
               msg = "bose made %s life\n" % (boseused).format(message)
               await client.send_message(message.channel, msg)
               msg = "Ladki made %s life\n" % (ladkiused).format(message)
               await client.send_message(message.channel, msg)

           if message.author.name == bose:
               msg = "you made %s life\n" % (boseused).format(message)
               await client.send_message(message.channel, msg)

           if message.author.name == ladki:
               msg = "you made %s life\n" % (ladkiused).format(message)
               await client.send_message(message.channel, msg)
                                         
@client.event
async def on_ready():
    print('Logged in as')
    print(client.user.name)
    print(client.user.id)
    print('------')

client.run(TOKEN)
