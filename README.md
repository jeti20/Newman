# Newman

Run and test collections from the command line using Newman

1.Install Node.js: Newman is a command-line tool that runs on Node.js --> https://nodejs.org/en

2. Download and install the latest version of Newman globally on your system

```
npm install -g newman
```

3.Create a JSON file of your Postman collection

4.Right click on Collection and export collection,  create folder and save the collection in this folder.

5. Save your environment Variables or use the environment variables provided - save it in the same folder 
![image](https://github.com/user-attachments/assets/ba498cf8-9b01-4448-88f6-c673b21740f0)


6. Open terminal and go to the created folder with exported collection

7. Execute Collections using newman

```
newman run <collection.json> -e <environment.json>
```

example output 
![image](https://github.com/user-attachments/assets/d31c837f-4ead-4849-997d-6ad7110d4abb)

**How to share postman collection link - no need of exporting the collection**

1. Go to postman and collection you want
2. Find share button
3. Choosevia json link
4. copy this link
5. open terminal and type

```
newman run <Copied link>

```

but if you using also global var, then you have to export them and include them in command command 

1. Go to Environments on the left panel
2. Chhose Globals
3. Click "Export" button on the lerft upper corner 
4. Choose export and folder where u executing the command
```
newman run <Copied link> -g <nazwa_pliku_z_zmiennymi_globalnymi.json>
```



