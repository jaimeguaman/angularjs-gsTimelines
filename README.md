# UX Animation Experiments - Koda 

## Summary

Use Greensock's (GSAP) `TimelineLite` to demonstrate the use of animation timelines to build complex transitions. Koda implementations will be used to explore the API usages & complexities of functionality required to create desired effects and UX. The samples contained here include:

*  [Demo_1.html](src/demo_1.html): &nbsp;&nbsp;Animations with click support only 
*  [Demo_2.html](src/demo_2.html): &nbsp;&nbsp;Animations with Timeline slider controls.

---

[CodePen Demo](http://codepen.io/ThomasBurleson/pen/OPMgqj)

![koda_gridlist](https://cloud.githubusercontent.com/assets/210413/5424252/316fb6c4-82ad-11e4-977d-6cf3d597c0f9.png)

---

#### Functional Considerations

While exploring the animation API requirements, the implemenation should also consider other functional requirements:

- Load images in background so zoom works quickly
- Use promises to delay transitions until the images are ready
- Dynamically modify timescale so unzoom is faster
- Use of global keypress to unzoom/reverse the timeline
- Use tile data model to define dynamic zoom from/to information
- Plugin use of Timeline Slider controls; independent of TimelineController
  - Sync Slider to transition timeline
  - Use slider to manually sequence through transition frames
- Support to drag on image to manually sequence through transitions

### Run Locally

Open Terminal console in the project directory.

```sh
bower update
http-server -d ./
```

Open Browser and navigate to URL `http://localhost:8080/`
