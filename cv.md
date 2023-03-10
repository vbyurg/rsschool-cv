# ![фото](./assets/img/photo-cv-markdown.jpg) Victor Byurg

## Contacts
* **Location:** Germany, Landau in der Pfalz
* **Email:** v.byurg@gmail.com
* **GitHub** vbyurg
* **Discord** Victor Byurg (@vbyurg)


## About me
I am a future frontend developer. Development is my hobby.

I like working with user interface design. I lovenon-standard design.

My interest in development makes my hobbya favorite! 
I treat every project withrespect and bring everything to the end!
Time in development fliesby unnoticed and I get great pleasurefrom my work. 
This pleasure motivates mefor further development.

Almost all of my free time I study newtechnologies to my next projectsthey were more professional.

In my free time I spend time with my family,
I have a beautiful wife, the mostunusual son on the planet and a very strange red cat. 
I love reading,playing guitar and learning something new!

## Skills
* HTML
* CSS
* SCSS
* JavaScript
* Git/GitHub
* Figma

## Exampe
``` 
 cityInput.addEventListener('change', cityChoice);
// Choice city
function cityChoice() {
    city = cityInput.value;
    if (city) {
        getWeather(city);
    };
}
// Get weather info from API
async function getWeather() {

    const url = `https://api.openweathermap.org/data/2.5/weather?q=${city}&lang=ru&appid=3ad7a98561014b40ee447e2216eaafa1&units=metric`;
    const res = await fetch(url);
    const data = await res.json();

    // Err
    if (res.status > 400 && res.status < 600) {
        weatherError.textContent = `Ошибка! Город "${city}" не найден`;
        weatherIcon.className = 'weather-icon owf';
        temperature.textContent = ``;
        humidityBlock.textContent = ``;
        windBlock.textContent = ``;
        weatherDescription.textContent = '';
    } else {
        // Clean error text
        weatherError.textContent = ``;
        // Add weather icon
        weatherIcon.className = 'weather-icon owf';
        weatherIcon.classList.add(`owf-${data.weather[0].id}`);

        // Show temperature info
        temp = Math.round(data.main.temp);
        temperature.textContent = `${temp} °C`;

        // Show humidity info
        humidity = Math.round(data.main.humidity);
        humidityBlock.textContent = `Влажность ${humidity} %`;

        // Show wind info
        wind = Math.round(data.wind.speed);
        windBlock.textContent = `Ветер ${wind} м/с`;

        // Show weather description
        weatherDescription.textContent = data.weather[0].description;
    }
}

getWeather()

// Set city value to localStorage
function setCity() {
    localStorage.setItem('city', cityInput.value);
    getWeather()
}
window.addEventListener('beforeunload', setCity);

// Get city value from localStorage
function getCity() {
    if (localStorage.getItem('city')) {
        cityInput.value = localStorage.getItem('city');
    }
    cityChoice()
}
window.addEventListener('load', getCity);
```


## Experience
* [ArtHobby](https://github.com/vbyurg/arthobby)
* [ThriveTalk](https://github.com/vbyurg/thrivery)
* [Cats](https://github.com/vbyurg/cat_energy)
* [House of sites](https://github.com/vbyurg/example)
* [Plants](https://github.com/vbyurg/plants)
* [Momentum](https://github.com/vbyurg/Momentum)

## Education
### **University:**
+ Institute of international social and humanitarian relations, Organization management
+ Moscow University of the Humanities, Psychologist

### **Courses**
+ Training center “Professional”, Frontend
+ INNOPOLIS UNIVERSITY, Frontend
+ Rolling Scopes School, JavaScript/Front-end. Stage 0 (https://app.rs.school/certificate/lr13r3vi)
+ Rolling Scopes School, JavaScript/Front-end. Stage 1

## English

**A2**
