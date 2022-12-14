### Getting Started
To get started, clone this repository from GitHub and install the dependencies with npm.
                
```
npm install
```

```sh
cd server
json-server --watch db.json --routes routes.json
```


Next step is running the application using the serve script and navigate to **http://localhost:8080/** to view the application.
</p>

```
npm run serve
```

### Vue CLI Scripts
Following commands are derived from create-app-app.
```
"npm run serve": Starts the development server
"npm run build": Builds the application for deployment.
"npm run lint": Executes the lint checks.
"npm run test:unit": Runs the tests.
```

### Structure
This app consists of 2 main parts; the application layout and the resources. **App.vue** inside src folder is the main component containing the template for the base layout whereas required resources such as SASS structure for the layout are placed inside the **src/assets/** folder.</p>

### Layout Components
Main layout is the template of the **App.vue**, it is divided into a couple of child components such as topbar, menu and footer. Here is template of the
**App.vue** component that implements the logic such as menu state, layout modes and so on.

### Menu
Menu is a separate component defined in **AppMenu.vue** file based on PrimeVue MenuModel API. In order to define the menuitems,
navigate to data section of **App.vue** file and define your own model as a nested structure using the **menu** property.

### Dependencies
Dependencies are listed below and needs to be added to package.json.

```json
{
    "primevue": "~3.12.2",
    "primeicons": "~5.0.0",
    "primeflex": "~3.1.2",
}
```

### PrimeVue Theme
Repair It uses the free Saga, Arya and Vela themes which are distributed within PrimeVue, however it can be used with any PrimeVue theme as well such as material, tailwind and bootstrap as layout colors are derived from the theme used via CSS variables.

### SASS Variables
In case you'd like to customize the layout variables, open **_variables.scss** file under src/layout folder. The list is pretty short as majority of the variables are derived from the PrimeVue theme being used.

**src/assets/_variables.scss**
```css
$fontSize:1rem;
$borderRadius:12px;
$transitionDuration:.2s;
```
