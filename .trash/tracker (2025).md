```dataviewjs
const trackerData = {
    entries: [],
    separateMonths: true,
    heatmapTitle: "bipolar mood",
    heatmapSubtitle: "this is for my daily moods",
}

const PATH_TO_YOUR_FOLDER = "5.8 — database/dailies";
const PARAMETER_NAME = 'mood';

for(let page of dv.pages(`"${PATH_TO_YOUR_FOLDER}"`).where((p) => p[PARAMETER_NAME])){
    trackerData.entries.push({
        date: page.file.name,
        filePath: page.file.path,
        intensity: page[PARAMETER_NAME],
    colorScheme: {
        paletteName: "custom",
    },
    defaultEntryIntensity: 5,
    intensityScaleStart: 1,
    intensityScaleEnd: 9
});
}


trackerData.basePath = PATH_TO_YOUR_FOLDER;

renderHeatmapTracker(this.container, trackerData);
```