status: #child 
tags: [[raven]] [[spreadsheet]] [[tracker]] [[daily notes]]
## bipolar disorder

```dataviewjs

dv.span("** mood **")

const hue1 = 13 
const hue2 = 219

const calendarData = {
    year: 2025, // optional, remove this line to autoswitch year 
    intensityScaleStart: 1,
    intensityScaleEnd: 9,
    colors: {
        red2green: [
            `hsl(${hue1}, 100%, 37%)`,     // 1 - darkest red
            `hsl(${hue1}, 100%, 50%)`,     // 2 - 
            `hsl(${hue1}, 100%, 60%)`,     // 3 - 
            `hsl(${hue1}, 100%, 77%)`,     // 4 - lightest red
            `hsl(0, 0%, 80%)`,             // 5 - neutral gray
            `hsl(${hue2*0.7}, 70%, 72%)`,  // 6 - lightest green
            `hsl(${hue2*0.85}, 43%, 56%)`, // 7 - 
            `hsl(${hue2}, 49%, 36%)`,      // 8 - 
            `hsl(${hue2}, 59%, 24%)`,      // 9 - darkest green
        ],
    },
    entries: []
}

for(let page of dv.pages('"5.8 — database/dailies"').where(p=>p.moods)){ 

    calendarData.entries.push({
        date: page.file.name, 
        intensity: page.moods,
        content: await dv.span(`[](${page.file.name})`), //for hover preview
    })
      
}

renderHeatmapCalendar(this.container, calendarData)

```

```dataview
TABLE WITHOUT ID
dateCreated as date,
symptoms as symptoms

FROM "5.8 — database/dailies"
```


```dataviewjs
dv.span("fluoxetine")

const calendarData = {
    year: 2025, // optional, remove this line to autoswitch year
    colors: {
        //white: ["#fff","#fff","#fff","#fff","#fff"],
        transparent: ["transparent"],
    },
    entries: []
}

for(let page of dv.pages('"5.8 — database/dailies"').where(p=>p.fluoxetine)){
	 
    calendarData.entries.push({
        date: page.file.name,
        content: await dv.span(`[🔺](${page.file.name})`), //for hover preview
    }) 
}

//console.log(calendarData)
	
renderHeatmapCalendar(this.container, calendarData)


```
```dataviewjs
dv.span("aripiprazole")

const calendarData = {
    year: 2025, // optional, remove this line to autoswitch year
    colors: {
        //white: ["#fff","#fff","#fff","#fff","#fff"],
        transparent: ["transparent"],
    },
    entries: []
}

for(let page of dv.pages('"5.8 — database/dailies"').where(p=>p.aripiprazole)){
	 
    calendarData.entries.push({
        date: page.file.name,
        content: await dv.span(`[🔺](${page.file.name})`), //for hover preview
    }) 
}

//console.log(calendarData)
	
renderHeatmapCalendar(this.container, calendarData)


```


## monoquin
```dataviewjs

dv.span("** monoquin post **")

const hue1 = 13 
const hue2 = 132

const calendarData = {
    year: 2025, // optional, remove this line to autoswitch year 
    intensityScaleStart: 1,
    intensityScaleEnd: 4,
    colors: {
        red2green: [
            `hsl(${hue1}, 100%, 37%)`,     // 1 
            `hsl(${hue1}, 100%, 77%)`,     // 2
            `hsl(${hue2}, 49%, 36%)`,      // 3 
            `hsl(${hue2}, 59%, 24%)`,      // 4 
        ],
    },
    entries: []
}

for(let page of dv.pages('"5.8 — database/dailies"').where(p=>p.monoquinPost)){ 

    calendarData.entries.push({
        date: page.file.name, 
        intensity: page.monoquinPost,
        content: await dv.span(`[](${page.file.name})`), //for hover preview
    })
      
}

renderHeatmapCalendar(this.container, calendarData)

```
```dataviewjs
dv.span("monoquin edit")

const calendarData = {
    year: 2025, // optional, remove this line to autoswitch year
    colors: {
        //white: ["#fff","#fff","#fff","#fff","#fff"],
        transparent: ["transparent"],
    },
    entries: []
}

for(let page of dv.pages('"5.8 — database/dailies"').where(p=>p.monoquinEdit)){
	 
    calendarData.entries.push({
        date: page.file.name,
        content: await dv.span(`[🌀](${page.file.name})`), //for hover preview
    }) 
}

//console.log(calendarData)
	
renderHeatmapCalendar(this.container, calendarData)


```
## habits
```dataviewjs

dv.span("** calisthenics **")

const hue1 = 13 
const hue2 = 132

const calendarData = {
    year: 2025, // optional, remove this line to autoswitch year 
    intensityScaleStart: 1,
    intensityScaleEnd: 9,
    colors: {
        red2green: [
            `hsl(${hue1}, 100%, 37%)`,     // 1 - darkest red
            `hsl(${hue1}, 100%, 50%)`,     // 2 - 
            `hsl(${hue1}, 100%, 60%)`,     // 3 - 
            `hsl(${hue1}, 100%, 77%)`,     // 4 - lightest red
            `hsl(0, 0%, 80%)`,             // 5 - neutral gray
            `hsl(${hue2*0.7}, 70%, 72%)`,  // 6 - lightest green
            `hsl(${hue2*0.85}, 43%, 56%)`, // 7 - 
            `hsl(${hue2}, 49%, 36%)`,      // 8 - 
            `hsl(${hue2}, 59%, 24%)`,      // 9 - darkest green
        ],
    },
    entries: []
}

for(let page of dv.pages('"5.8 — database/dailies"').where(p=>p.calisthenics)){ 

    calendarData.entries.push({
        date: page.file.name, 
        intensity: page.calisthenics,
        content: await dv.span(`[](${page.file.name})`), //for hover preview
    })
      
}

renderHeatmapCalendar(this.container, calendarData)

```

```dataviewjs
dv.span("journaling")

const calendarData = {
    year: 2025, // optional, remove this line to autoswitch year
    colors: {
        //white: ["#fff","#fff","#fff","#fff","#fff"],
        transparent: ["transparent"],
    },
    entries: []
}

for(let page of dv.pages('"5.8 — database/dailies"').where(p=>p.journaling)){
	 
    calendarData.entries.push({
        date: page.file.name,
        content: await dv.span(`[🖋](${page.file.name})`), //for hover preview
    }) 
}

//console.log(calendarData)
	
renderHeatmapCalendar(this.container, calendarData)


```


```dataviewjs

dv.span("** bookReading **")

const hue1 = 13 
const hue2 = 132

const calendarData = {
    year: 2025, // optional, remove this line to autoswitch year 
    intensityScaleStart: 1,
    intensityScaleEnd: 9,
    colors: {
        red2green: [
            `hsl(${hue1}, 100%, 37%)`,     // 1 - darkest red
            `hsl(${hue1}, 100%, 50%)`,     // 2 - 
            `hsl(${hue1}, 100%, 60%)`,     // 3 - 
            `hsl(${hue1}, 100%, 77%)`,     // 4 - lightest red
            `hsl(0, 0%, 80%)`,             // 5 - neutral gray
            `hsl(${hue2*0.7}, 70%, 72%)`,  // 6 - lightest green
            `hsl(${hue2*0.85}, 43%, 56%)`, // 7 - 
            `hsl(${hue2}, 49%, 36%)`,      // 8 - 
            `hsl(${hue2}, 59%, 24%)`,      // 9 - darkest green
        ],
    },
    entries: []
}

for(let page of dv.pages('"5.8 — database/dailies"').where(p=>p.bookReading)){ 

    calendarData.entries.push({
        date: page.file.name, 
        intensity: page.bookReading,
        content: await dv.span(`[](${page.file.name})`), //for hover preview
    })
      
}

renderHeatmapCalendar(this.container, calendarData)

```

```dataviewjs
dv.span("art stuff")

const calendarData = {
    year: 2025, // optional, remove this line to autoswitch year
    colors: {
        //white: ["#fff","#fff","#fff","#fff","#fff"],
        transparent: ["transparent"],
    },
    entries: []
}

for(let page of dv.pages('"5.8 — database/dailies"').where(p=>p.doArt)){
	 
    calendarData.entries.push({
        date: page.file.name,
        content: await dv.span(`[🎨](${page.file.name})`), //for hover preview
    }) 
}

//console.log(calendarData)
	
renderHeatmapCalendar(this.container, calendarData)


```

```dataviewjs
dv.span("songs daily")

const calendarData = {
    year: 2025, // optional, remove this line to autoswitch year
    colors: {
        //white: ["#fff","#fff","#fff","#fff","#fff"],
        transparent: ["transparent"],
    },
    entries: []
}

for(let page of dv.pages('"5.8 — database/dailies"').where(p=>p.songDaily)){
	 
    calendarData.entries.push({
        date: page.file.name,
        content: await dv.span(`[🎹](${page.file.name})`), //for hover preview
    }) 
}

//console.log(calendarData)
	
renderHeatmapCalendar(this.container, calendarData)

```


```dataviewjs
dv.span("anki")

const calendarData = {
    year: 2025, // optional, remove this line to autoswitch year
    colors: {
        //white: ["#fff","#fff","#fff","#fff","#fff"],
        transparent: ["transparent"],
    },
    entries: []
}

for(let page of dv.pages('"5.8 — database/dailies"').where(p=>p.ankiDeck)){
	 
    calendarData.entries.push({
        date: page.file.name,
        content: await dv.span(`[💆](${page.file.name})`), //for hover preview
    }) 
}

//console.log(calendarData)
	
renderHeatmapCalendar(this.container, calendarData)


```

