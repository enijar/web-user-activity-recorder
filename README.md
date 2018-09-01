# Web User Activity Recorder

This is a task for the [OpenGift Hackathon](https://opengift.io/hackathon/). 

The task is to record user activity on a website and send that report to a programmer or manager for useful insights.

### Setup

Install dependencies with:

```bash
npm install
```

Build assets with:

```bash
npm run assets:build
```

Start a server with:

```bash
cd public/ && python -m SimpleHTTPServer 8000
```

### Approach

All recorders have their own class inside the [src/js/Recorder/Recorders](src/js/Recorder/Recorders) directory. 

The [Recorder](src/js/Recorder/index.js) class initialises all recorders and controls when the recorder starts 
and stops.

[app.js](src/js/app.js) is where the recorder is started.

### TODO

[x] Implement click, form, link, resize and scroll recorders
[ ] GUI to show useful data of a recorded session
[ ] GUI to show replay of a recorded session
[ ] Sync localStorage data to server then delete localStorage
[ ] Write tests for each recorder