# Smart Citizen Post

This is a simple package simplifing the interaction with the Smart Citizen API http://developer.smartcitizen.me

## Install

```
npm install smartcitizen
```

## Post data

```
var SmartCitizen = require('smartcitizen')

var smartcitizen = new SmartCitizen({
    id: 8909, // Your device id
    token: 'F1XZt67EG9ya0E5k6yfHhgVQsXl4SbsDcE4ZBc4VMGtsTrOeBri7VjwcqZ0NWqDVE' // Your token
});

smartcitizen.push({
    recorded_at: new Date(),
    sensors: [{
        id: 'noise',
        value: 59
    }]
})
```
