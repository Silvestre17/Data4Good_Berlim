# 🏙️ Berlin Urban Innovation: A Data4Good Hackathon Project 🚲

<p align="center">
    <a href="https://www.hertie-school.org/en/data4good-festival/">
        <img src="./img/Data4Good Festival.png" alt="Berlin Data4Good Project Banner" width="400">
    </a>
</p>

<p align="center">
    <!-- Project Links -->
    <a href="https://github.com/Silvestre17/Data4Good_Berlim"><img src="https://img.shields.io/badge/Project_Repo-100000?style=for-the-badge&logo=github&logoColor=white" alt="GitHub Repo"></a>
</p> 

## 📝 Description

This project is our submission for the **Data4Good Festival Hackathon**, focusing on urban innovation in **Berlin** 🇩🇪. By leveraging open datasets on traffic accidents, air quality, and cycling infrastructure, we developed a data-driven solution to identify safer, cleaner, and more efficient cycling routes throughout the city. The goal is to transform raw data into actionable insights that can enhance the quality of life for Berlin's citizens.

## ✨ Objective

The primary objective of this 48-hour challenge was to design, explore, and prototype a solution that addresses the multifaceted challenges of urban living. Our specific goals were to:

*   Analyze and identify **accident hotspots** across the city.
*   Develop a methodology to define and recommend the **safest and healthiest cycling routes**.
*   Create an **interactive tool** to help cyclists and city planners make better, data-informed decisions.

## 🎓 Event Context

This project was created during the **Data4Good Festival Hackathon**, organized by the **Hertie School** in Berlin, Germany, from April 19-21, 2024. As participants, we were challenged to develop a meaningful, data-driven solution to a real-world problem within a 48-hour timeframe.

<p align="center">
    <a href="https://www.hertie-school.org/">
        <img src="https://img.shields.io/badge/Hertie_School-003A70?style=for-the-badge" alt="Hertie School" />
    </a>
    <a href="#">
        <img src="https://img.shields.io/badge/Data4Good_Festival-228B22?style=for-the-badge" alt="Data4Good Festival" />
    </a>
</p>

## 🗺️ Data Sources

Our analysis was built upon three core datasets provided for the hackathon:

*   **Accidents in Berlin (2021):** Detailed records of road accidents, including precise geolocation data.
*   **Air Pollution Data (2021):** Air quality measurements (e.g., NO₂, PM10) from official monitoring stations.
*   **Urban Infrastructure Data:** Geospatial data on existing cycling routes across Berlin.

For a detailed overview of the data preparation process, see the original [data preparation notebook](./data-preparation.ipynb).

## 🛠️ Technologies Used

The project was implemented entirely in **Python**, leveraging its powerful data science and geospatial libraries.

#### Core Stack
<p align="center">
    <a href="https://www.python.org/">
        <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python" />
    </a>
    <a href="https://jupyter.org/">
        <img src="https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white" alt="Jupyter Notebook" />
    </a>
</p>

#### Data Analysis & Manipulation
<p align="center">
    <a href="https://pandas.pydata.org/">
        <img src="https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white" alt="Pandas" />
    </a>
    <a href="https://numpy.org/">
        <img src="https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white" alt="NumPy" />
    </a>
</p>

#### Geospatial Analysis & Visualization
<p align="center">
    <a href="https://geopandas.org/">
        <img src="https://img.shields.io/badge/GeoPandas-139453?style=for-the-badge" alt="GeoPandas" />
    </a>
    <a href="https://python-visualization.github.io/folium/">
        <img src="https://img.shields.io/badge/Folium-3E8E41?style=for-the-badge&logo=leaflet&logoColor=white" alt="Folium" />
    </a>
    <a href="https://matplotlib.org/">
        <img src="https://img.shields.io/badge/Matplotlib-D3D3D3?style=for-the-badge&logo=matplotlib&logoColor=black" alt="Matplotlib" />
    </a>
</p>

---

## ⚙️ Project Workflow

Our 48-hour sprint followed a condensed data science process:

1.  **Data Exploration & Cleaning:** Loaded the datasets, handled missing values, and standardized data types, particularly for geospatial coordinates and timestamps.
2.  **Geospatial Analysis:**
    *   Mapped accident locations to identify high-risk zones or **"accident hotspots"**.
    *   Integrated air quality data from monitoring stations to create a pollution layer across the city.
3.  **Route Scoring:** Developed a simple but effective scoring algorithm to evaluate cycling routes by combining safety and air quality metrics.
4.  **Interactive Visualization:** Built an interactive map using **Folium** to present our findings in an accessible and user-friendly way.

## 💡 Our Proposed Solution: "AIDSCA" - AI-Driven Smart City Assistant

We developed a prototype for an interactive web map called **AIDSCA**, designed to help cyclists plan their journeys based on safety and environmental factors.

#### Key Features:
*   **Interactive Map Layers:** The Folium map allows users to toggle different data layers on and off, including:
    *   📍 Accident hotspots.
    *   💨 Air pollution levels.
    *   🚲 Existing cycling infrastructure.
*   **Route Safety Score:** Each cycling route is color-coded based on a calculated **safety & health score**, which penalizes routes for proximity to accidents and high-pollution zones.
*   **Data-Driven Insights:** The analysis pinpoints specific intersections and road segments that are high-risk, providing a basis for data-driven policy recommendations to the city.

## 🚀 How to Run the Solution

To explore our analysis and replicate the results, please follow these steps:

1.  **Prerequisites:**
    *   Ensure you have Python 3.x installed.
    *   We recommend using a virtual environment.

2.  **Clone the Repository:**
    ```bash
    git clone https://github.com/Silvestre17/Data4Good_Berlim.git
    cd Data4Good_Berlim
    ```
3.  **Launch Jupyter:**
    *   Run Jupyter Notebook from your terminal:
        ```bash
        jupyter notebook
        ```
    *   Open the main project notebook ([`ISCTE Derrubar.ipynb`](./ISCTE%20Derrubar.ipynb)) to view the full workflow, from data loading to the final Folium map generation.

## 👥 Team Members

This project was a collaborative effort by:
*   **André Silvestre**
*   **Rita Matos**
*   **Maria Margarida Pereira**

## 🇩🇪 Note

While the project is documented in English, the context is the vibrant, data-rich environment of Berlin, Germany 🇩🇪. 🍺🥨 We hope our findings and tools can contribute to making Berlin a safer and more sustainable city for cyclists.