# FestivalApp-Expo (Production)
This project is a festival app built using React Native and Expo CLI framework.

## About the project 
The FestivalApp-Expo is designed specifically for the festival taking place in Herrljunga Kommun. It aims to provide users with a smooth and engaging experience throughout the festival. The app includes four main pages, each offering unique features and information.


## First Page (Scener)
This page provides comprehensive information about various venues where events take place, the amazing artists performing there, and also offers a visual experience with inspiring pictures. Additionally, you have the opportunity to bookmark your favorite venues and artists to make it even easier to find and enjoy the events that interest you the most.

To change the content in the scene, follow these steps:

1. Locate the 'scene.json' file at FestivalApp-Expo\jsonTemp\scene.json.
2. Edit the file and find the block of code you want to modify or add a new block of code for it.

Here's an example of the code structure:

```json
{
    "artist": "{Artist name here}",
    "time": "{Time when artist is playing here}"
},
```

Example Code: 
```json
 {
     "artist": "Drake",
     "time": "15:00"
 },
```

## Second page (Områden) 
On this page, we provide an interactive map feature where we have marked various areas. You will also find detailed information about each specific area and what there is to discover there.

The changes you can make to this page is the information under the maps section, which displays the details of each place.

Follow these steps:

1. Locate the 'location.json' file at FestivalApp-Expo\jsonTemp\location.json.
2. Edit the file to locate the desired block of code and modify the 'name,' 'info,' and 'mapLink' accordingly.

Here is an example of how it looks inside the JSON file.

```json
{
     "name": "Torget",
     "info": "Torget är beläget mitt i Herrljunga centralort och utgör festivalens nav. Här kan du njuta av otrolig mat och fina musikupplevelser. Slå dig ner eller dansa? Det är frågan! ",
     "color": "rgb(51, 255, 51)",
     "mapLink": "https://goo.gl/maps/oECJ4JbFWJXBqJfE6"
}
```

## Third page (Mat) 
On this page, you will find information about various food carts and their diverse food offerings. Here, you can discover a wide range of options, including vegan food, meat dishes, and seafood.

To change the information or add new data, it is modified in the JSON file. 

Follow these steps:

1. Locate the 'food.json' file at FestivalApp-Expo\jsonTemp\food.json.
2. Edit the file to locate the desired block of code and modify the 'name', 'vegan', 'meat', 'fish', 'menu' accordingly.

Here is an example of how it looks inside the JSON file.

```json
{
   "name": "Toro Grill",
   "vegan": "false",
   "meat": "true",
   "fish": "false",
   "menu": [
     {
        "food": "Handgjorda burgare & hemgjorda pommes frites. (K)"
     }
   ]
},
```

you can only Have 'true' or 'false' in 'vegan', 'meat' and 'fish' 

'true' = show the icon 
'False' = not showing the icon 

## Fourth page (Sponsors) 
this page you will find proudly displayed logos of our valuable sponsors who support the festival, along with their links.

To change the content or add new data, it is modified in the JSON file. 

1. Locate the 'sponsorsInfo.json' file at FestivalApp-Expo\jsonTemp\sponsorsInfo.json.
2. Edit the file to locate the desired block of code and modify the 'BigSponsors', 'Sponsors', 'homepage' accordingly.

This JSON file is a bit special because we have two specific types of sponsors: 'BigSponsors' and 'Sponsors'. The difference is that the Big Sponsor is the sponsor who wants to have the first and biggest placement, while the Sponsor has a normal size and is positioned below the Big Sponsor. 

The 'BigSponsors' and 'Sponsors' code 
```json
 {
   "picture": "data:image/png;base64,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",
   "homepage": "https://leader-sjuharad.se/"
 }
```

I use the data:image type for pictures, but it also works with URLs

## Change the menu
To add a new section to menu, follow this steps:


1. Locate the 'StackMenuRouter.js' in repository/folder
2. Add the following code under <View style={{ alignItems: 'center' }}>, where you can find similar code:
  
```js
 {
<TouchableOpacity onPress={() => navigation.navigate('NameOfScreen')}>
  <Text style={styles.link}>Name You Want to Display in the Menu</Text>
</TouchableOpacity>
 }
```
3. The secound code you need to add is method a litle bit more down(somthing between row 78 to 133) you will find somthing similiar 
  
```js
const NameOfScreen = () => {
  return (
    <View style={styles.container}>
      <View style={styles.container}>
        { /* Add/Import the content you want to display on this page */ }
      </View>
    </View>
  );
};
```
4. The final code to add undernith <Stack.Navigator> is 
  
```js
   <Stack.Screen name="NameOfScreen" component={NameOfScreen} options={{ headerShown: false }}/>
```
 
# Start the App 
Before you start, make sure you have the following requirements:

1. Node: Install Node.js, which includes npm (Node Package Manager).
2. IDE of your choice: You can use any Integrated Development Environment (IDE) for editing the code. (I used VSCode for this project).
3. Mobile device: You will need a mobile device (Android or iPhone) that can run the Expo app.
  
## Installation
1. Install Node.js by visiting the official website: Node.js and following the installation instructions for your operating system.
2. Open the terminal and navigate to the project directory.
3. Install Expo CLI globally by running the following command:
  ````npm install -g expo-cli````

## Running the App
1. Start the development server by running the following command in the project directory:
   ````npm start```` 
  
2. A QR code will be displayed in the terminal or in a new browser window.

3. Install the Expo app on your mobile device:
  
    For Android: Download and install the Expo app from the Google Play Store.
    For iPhone: Download and install the Expo app from the App Store.
4. Open the Expo app on your mobile device and scan the QR code displayed in the terminal or browser. This will load and run the app on your device.
5. You should now see the app running on your mobile device.

 # Other information
In the Scene.js file, there is a function available to display the picture of the scene. However, it is currently commented out. To utilize this function, please follow the steps below:

1. Locate the Scene.js file in your project.
2. Uncomment the function code by removing the comment markers (```` {/* <ImgPopup src={scen1.image} /> */} ````).
3. Open the JSON scene file (Scene.json) and find the image field.
4. Modify the URL in the image field to the desired picture URL of your choice.
  
By following these steps, you can display a custom picture for the scene
