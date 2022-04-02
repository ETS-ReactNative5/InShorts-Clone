# InShorts-Clone

Download the apk from given link.
https://drive.google.com/file/d/13i3aJBDXNanKhxtQK1JSXDbBKwutvMoa/view?usp=sharing

Developed an android news feed application. 


* **Select 4 major news channels** -> **CNN**, **BBC News**, **Fox News** and **Google News**.
* **Latest updates for major countries like** -> **India**, **Australia**, **USA**, **Russia**, **France** and **United Kingdom*.
* **Tabbed View** for flawless transitions between the screens.
* **Axios** for fetch requests.

## About saurav.tech

Api Used https://saurav.tech/NewsAPI/

Saurav is a Youtuber, Vlogger and Freelancer.
He is a passionate blockchain developer from india. Most of his research effort is focused on improving ÐApp experience. 
Currently working in newfang
His Webiste - https://saurav.tech/

## Usage

### JS Applications

This is a React Native Project. You can install the dependencies and run the app.
For this you will require usb debugging and your phone should be connected to the laptop.

<details><summary><b>Show instructions</b></summary>

1. Install the dependencies:

    ```sh
    $ npm install 
    ```

2. Run the app in the android.

    ```sh
    $ npm start
    ```

3. Open another terminal
  
    ```sh
    $ npm run android
    ```

4. This will start building the project and install the apk on your device.
  
</details>


## Dependencies

* `@testing-library/react` : "^12.1.2"
* `@testing-library/user-event` : "^13.5.0"
* `axios` : "^0.25.0"  Promise based HTTP client for the browser and node.js
* `react` : "^17.0.2",
* `react-dom` : "^17.0.2",
* `react-scripts` : "5.0.0",
* `web-vitals` : "^2.1.4"
* `react-native-pager-view` : "5.0.12"  For horizontal swipe screen transistion
* `react-native-snap-carousel` : "^3.9.1" For transition between screens.
* `react-native-tab-view` : "^3.0.1"  Dependency for pager-view
* `react-native-web` : "~0.13.12"  Dependency for pager-view


## JS API

```js
axios
    .get(
      'https://saurav.tech/NewsAPI/everything/${source}.json'
    )
    .then(res => {
      setCoins(res.data);
      console.log(res.data);
    })
    .catch(error => console.log(error));
    
axios
    .get(
      'https://saurav.tech/top-headlines/category/${category}/${country}.json'
    )
    .then(res => {
      setCoins(res.data);
      console.log(res.data);
    })
    .catch(error => console.log(error));
```
