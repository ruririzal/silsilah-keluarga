#  Silsilah Keluarga

### Getting Started
 Aplikasi silsilah keluarga dengan basis Vue CLI (https://cli.vuejs.org/).
 Untuk memulai, clone repository ini dari GitHub dan install dependencies dengan npm atau yarn.
                
```
npm install
```

or

```
yarn
```

<p>Tahap selanjutnya adalah menjalankan aplikasi menggunakan perintah serve dan buka alamat url **http://localhost:8080/** untuk melihat aplikasi </p>

```
npm run serve
```

#  Menggunakan "Sakai Admin Template for Vue" sebagai basis tampilan dengan beberapa modifikasi dibeberapa bagian
 
### Live Preview "Sakai Admin Template for Vue" 
 
Visit [Sakai Vue](https://www.primefaces.org/sakai-vue) website for a live preview. 
 

### Vue CLI Scripts
Following commands are derived from create-app-app.
```
"npm run serve": Starts the development server
"npm run build": Builds the application for deployment.
"npm run lint": Executes the lint checks.
"npm run test:unit": Runs the tests.
```

### Structure
Sakai consists of 2 main parts; the application layout and the resources. **App.vue** inside src folder is the main component containing the template for the base layout whereas required resources such as SASS structure for the layout are placed inside the **src/assets/** folder.</p>

### Layout Components
Main layout is the template of the **App.vue**, it is divided into a couple of child components such as topbar, menu and footer. Here is template of the
**App.vue** component that implements the logic such as menu state, layout modes and so on.

### Menu
Menu is a separate component defined in **AppMenu.vue** file based on PrimeVue MenuModel API. In order to define the menuitems,
navigate to data section of **App.vue** file and define your own model as a nested structure using the **menu** property.

### Dependencies
Dependencies of Sakai are listed below and needs to be added to package.json.

```json
{
    "primevue": "~3.12.2",
    "primeicons": "~5.0.0",
    "primeflex": "~3.1.2",
}
```

### SASS Variables
In case you'd like to customize the layout variables, open **_variables.scss** file under src/layout folder. The list is pretty short as majority of the variables are derived from the PrimeVue theme being used.

**src/assets/_variables.scss**
```css
$fontSize:1rem;
$borderRadius:12px;
$transitionDuration:.2s;
```
