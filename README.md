# Political Campaign Sendouts

##  Goal
This repository contains files and codes used for a political campaign. The goal was to send out messages fast and widely as advertisement.

![Candidato a Vereador Roberto Estácio](santinho.jpg)

## Methodology
 - It was used the candidate's personal contacts (leads) and also public data that contained phone number to be able to it

![personal contacts](listas_juntas_roberto.xlsx)
![public contacts part 1](public_leads_A.xlsx)
![public contacts part 2](public_leads_B.xlsx)
![public contacts part 3](public_leads_C.xlsx)
![public contacts part 4](public_leads_parte_4) #link, the XLSX file is too heavy for Github
   
 - First, it was necessary to go through data wrangling to keep all phone number in the correct format to apply the API, and also later put them all together
![data wrangling](public_leads_to_send_message.ipynb)

 - Secondly, those phone number should be verified as valid and active Whatsapp accounts, once this was the app where message would be sent. This app is widespread in Brazil, being the most efficient place to send messages if one wants the other to actually see it. THis could be done also through the API

![sending out messages via API](disparo_evo.ipynb)
   
 - Finally, after verifying if a phone number is a Whatsapp account, those numbers are put together in a final list, and then the API can be applied to send out messages

## The API

Evolution API is a non-official open-source Brazilian API for Whatsapp messager. 

![logo](evo_api.png)

it requires a VPS to be installed and a whatssap account with a valid phone number to be able to send messages.

![Evolution API Documentation](https://doc.evolution-api.com/v2/en/get-started/introduction)
