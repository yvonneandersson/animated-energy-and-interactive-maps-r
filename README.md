# 🌍🔋 Animated Energy Charts & Interactive Maps – R Visualization

This repository contains solutions for **Assignment 3**, a group project using **R**, **gganimate**, **ggplot2**, and **interactive mapping libraries** to visualize global energy production and geographical data.

---

## 📚 Assignment Summary

This project includes two tasks:

1. Creating a **GIF animation** of global energy production using `gganimate`
2. Building an **interactive map** of Europe with enriched data using `ggplot2`, `sf`, and `ggiraph` or `ggplotly`

---

## 🔋 Task 1 – Animated Bar Chart: Energy Production (1800–2023)

You will create an animated bar chart visualizing different sources of energy over time using the dataset `Energy_production`.

### Steps include:
- Load and prepare the dataset from `.rda`
- Create a **static bar chart** with `ggplot2` showing energy quantity per source and type
- Use `gganimate` and `{frame_time}` to animate the timeline
- Customize styling (`theme()`, `labs()`, `element_text()`) for visual clarity
- Save the result as a `.gif` using `anim_save()`

🧾 Output: A dynamic `.gif` visual showing change in energy use across categories (Fossil, Non-fossil, Renewables)

## 📝 Results:

![](https://i.imgur.com/K904yOK.gif)


---

## 🌍 Task 2 – Interactive Map of Europe (with Tooltip Information)

Using world map data from the `sf` package, you will create an interactive European map.

### Key steps:

- Load and plot the world map with `geom_sf()`
- Filter for **Europe only** using `dplyr::filter()`
- Merge (`left_join()`) with an external dataset (e.g. World Bank or Our World in Data)
- Visualize extra information using:
  - `ggiraph` for tooltips
  - or `ggplotly` for zoomable, clickable maps
- Optional: Crop the map using `xlim()` and `ylim()` (e.g. exclude Russia's far east, Canary Islands)

📌 Tip: Customize `fill`, labels, and interactivity to show country-level statistics (e.g., population, GDP, emissions, etc.)

---

## 📝 Results

- Merged dataset used for Task 2 (`merged_europe_data.csv`)
- Code must include:
  - All used libraries (e.g., `sf`, `gganimate`, `ggplot2`, `dplyr`, `ggiraph`)
  - Reproducible paths so others can run your analysis
 
![](https://i.imgur.com/B48x1DU.gif)


---

## 💡 Summary

This project explores animated and interactive data visualization in R. It applies bar chart animation to show historical energy trends and builds custom interactive maps using public global data.

The assignment encourages both **storytelling with data** and **technical skill** in modern visualization tools in R.
