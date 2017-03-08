[Link](https://bastiaanvanassche.github.io/mesos-presentation) to the slideshow (hosted with GitHub pages)
# Running the slideshow from a local web server
1. Install Node.js (4.0.0 or later)
2. Navigate to the presentation folder `$ cd mesos-presentation`
3. Install dependencies: `$ npm install`
4. Serve the presentation: `$ npm start`
5. Open [http://localhost:8000](http://localhost:8000) to view the presentation

# Generate PDF version of the slideshow
[DeckTape](https://github.com/astefanutti/decktape) is a high-quality PDF exporter for HTML5 presentation frameworks. There's a docker image available, so you can generate a PDF version of your presentation running on [http://localhost:8000](http://localhost:8000):

`docker run --rm --net=host -v $(pwd):/slides astefanutti/decktape http://localhost:8000 slides.pdf`