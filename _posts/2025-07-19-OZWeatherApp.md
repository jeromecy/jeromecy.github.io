---
title: "OZWeatherApp: AI-Powered Australian Weather & Climate Insights"
date: 2025-07-19
categories: [R Shiny, Weather, AI, Australia]
tags: [weatherOz, Shiny, AI, agriculture, climate]
---

🌦️ **OZWeatherApp**

🚀 **Live Demo**  
Try the app now: [https://cbada.shinyapps.io/OZWeather/](https://cbada.shinyapps.io/OZWeather/)

## Overview

OZWeatherApp is an interactive Shiny web application that visualises Australian weather and climate data, powered by advanced AI analysis. Leveraging the `{weatherOz}` package, the app accesses and downloads data from key Australian sources, including:

- **SILO**: Scientific Information for Land Owners – Australia-wide gridded climate data from Queensland's Long Paddock initiative
- **DPIRD**: Department of Primary Industries and Regional Development – Observational data from WA weather stations via the Weather 2.0 Open API

The app also supports integration with the Australian Government Bureau of Meteorology (BOM) for bulletins and imagery.

## Features

- 🌍 **Interactive Map**: Click anywhere to select a location and retrieve weather data (default: Perth)
- 📅 **Date Range Selection**: Filter historical data by custom date ranges
- 📊 **Data Visualisation**: Interactive charts for temperature and rainfall
- 📋 **Enhanced Data Table**: Responsive, searchable, and sortable tables
- 📥 **Export Options**: Download data as CSV, Excel, or PDF
- 🤖 **AI Analysis**: Generate expert agricultural and meteorological insights using GPT-4o Mini or DeepSeek
- 🎨 **Modern UI**: Clean, responsive design with Australian spelling and branding
- 📱 **Mobile Friendly**: Works seamlessly on desktop and mobile

## AI Analysis Capabilities

OZWeatherApp includes advanced AI-powered features:

- **Expert Analysis**: AI models provide professional agricultural and meteorological insights
- **Crop Disease Assessment**: Advice on fungicide application and crop disease risk
- **Weather Pattern Forecasting**: Predictions based on historical data trends
- **Streaming Results**: Real-time display of AI analysis with typewriter effect
- **Multiple AI Models**: Support for GPT-4o Mini and DeepSeek

## Data Sources

OZWeatherApp uses the `{weatherOz}` package to access data from:

- **DPIRD**: WA weather station network via the Weather 2.0 Open API
- **SILO**: Australia-wide gridded climate data
- **BOM**: Agriculture bulletins, radar and satellite imagery, and seven-day forecasts

## API Usage

The app integrates with third-party APIs (SILO, DPIRD, OpenAI, DeepSeek) for analytics and visualisation.  
**Online Demo**: Uses a temporary API key for demonstration.  
**Local Use**: Users must provide their own API keys. See below for setup instructions.

## Installation & Usage

1. **Clone the repository:**

   ```bash
   git clone https://github.com/jeromecy/OZWeatherApp.git
   cd OZWeatherApp
   ```

2. **Install required packages:**

   ```r
   install.packages(c("shiny", "leaflet", "highcharter", "DT", "weatherOz", 
                    "shinyFeedback", "jsonlite", "dplyr", "markdown", 
                    "ellmer", "shinychat", "later"))
   ```

3. **Set up API keys:**  
   Create a `.Renviron` file in your project directory with the following:

   ```
   OPENAI_API_KEY="your_openai_api_key"
   DEEPSEEK_API_KEY="your_deepseek_api_key"
   SILO_API_KEY="your_silo_api_key"
   DPIRD_API_KEY="your_dpird_api_key"
   ```

4. **Run the application:**

   ```r
   shiny::runApp('OZWeather')
   ```

## Technical Stack

- **R Shiny**: Web application framework
- **Leaflet**: Interactive maps
- **Highcharter**: Data visualisation
- **DT**: Enhanced data tables
- **weatherOz**: Australian weather data access
- **AI Integration**: OpenAI GPT-4o Mini and DeepSeek models

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request with your changes.

## License

MIT License  
Copyright (c) 2025 Zhanglong Cao

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

## Developed By
Curtin Biometry and Agricultural Data Analytics  
Centre for Crop and Disease Management  
Curtin University, Perth, Australia

## Acknowledgements

This application uses the `{weatherOz}` package to facilitate access to Australian weather and climate data resources. Special thanks to the developers of `{weatherOz}` for providing such a valuable tool for accessing Australian weather data.

## Version History

- **Version 2.0**: Enhanced UI with AI analysis, improved data export, modern design, and comprehensive error handling
- **Version 1.0**: Basic weather data visualisation with interactive maps and charts
