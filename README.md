# AccidentTrafficAnalysis

[![License](https://img.shields.io/badge/License-GPLv3-blue.svg?style=for-the-badge)](https://github.com/ISIS1225DEVS/ISIS1225-Lib/blob/master/LICENSE)

## Overview

The **AccidentTrafficAnalysis** project focuses on analyzing traffic accidents in Bogotá, Colombia, using datasets from the Secretaría Distrital de Movilidad. The project integrates data structures like balanced binary search trees (BSTs), hash tables, and lists to provide efficient queries for accident data. Students practice tree-based searching, linear searches, and sorting algorithms to address key problems in traffic accident analysis. The project also emphasizes teamwork and using the MVC (Model-View-Controller) architecture to load and process CSV data effectively.

## Members

The students edit this section to add their names, Uniandes emails, and specify which project functionality of the project they will implement.

1. Student No. 1 Ángel Farfán, Student No. 1 Uniandes Email a.farfana@uniandes.edu.co, Student No. 1 20222183.
1. Student No. 2 Juan José Díaz, Student No. 2 Uniandes Email jj.diazo1@uniandes.edu.co, Student No. 2 202220657.
1. Student No. 3 Name Andrés Cáceres, Student No. 3 Uniandes Email a.caceresg@uniandes.edu.co, Student No. 3 202214863.

[Back to top](#accidenttrafficanalysis)

## Context

Bogotá, Colombia, as the nation's most populous city, faces significant challenges in terms of vehicle traffic, including cars, buses, motorcycles, bicycles, and electric scooters. With increasing vehicle numbers, traffic accidents have become a major issue for local authorities, who have responded with traffic regulations, public campaigns, and better infrastructure to improve mobility and reduce accidents.

Despite improvements, the number of accidents remains high, especially with the growing number of motorcycles on the road. The project uses datasets from Bogotá's Secretaría Distrital de Movilidad, spanning from 2015 to 2022, to analyze traffic accidents and identify patterns.

### Data Loading

The dataset for this challenge comes from the Open Data repository of the Secretaría Distrital de Movilidad de Bogotá. It contains records of all accidents in the city from 2015 to 2022. Each CSV file contains 15 columns, including accident codes, dates, locations, severity, and types of accidents. To handle the large CSV files efficiently, memory settings and recursion limits in Python must be adjusted accordingly.

### References

1. [Bogotá Open Data - Secretaría Distrital de Movilidad](https://www.datos.gov.co/)

## About the repository

This repository is part of the **Data Structures and Algorithms (EDA)** teaching framework at Universidad de los Andes. The repository was developed by faculty professors and staff in the Department of Systems and Computer Engineering (DISC) and uses the Non-Object-Oriented Python library **DISCLib**.

[DISClib](https://github.com/ISIS1225DEVS/ISIS1225-Lib) · [DISClib Demo and Examples](https://github.com/ISIS1225DEVS/ISIS1225-Examples) · [Report Bug](https://github.com/ISIS1225DEVS/ISIS1225-Lib/issues) · [Request Feature](https://github.com/ISIS1225DEVS/ISIS1225-Lib/issues)

## About The Project

**IMPORTANT** This is a work in progress and is part of a teaching framework for undergraduate college students at Universidad de los Andes. This project Is NOT intended as a full-functional source code project.

## Structure

The challenge template has four main parts:

1. [DISClib](https://github.com/ISIS1225DEVS/ISIS1225-Lib) Root folder with the official course library. For more on its implementation, visit the [DISClib Repository](https://github.com/ISIS1225DEVS/ISIS1225-Lib).
2. [App](./App) Folder with the model-view-controller (MVC) Python scripts. In here, the students implement their code to complete the challenge.
3. [Data](./Data) Folder with CSV data files to load into the application. Students must add the course-provided data files to complete the challenge.
4. [Docs](./Docs) Folder with reports, data tables, and other documentation. Students add their project report, data tables, and other documentation to complement their code implementation.

[Back to top](#accidenttrafficanalysis)

## Requirements

### Requirement 1: Report all accidents within a date range (Group)

As a traffic analyst, I want to know about all the accidents that occurred in the city within a specific date range. The expected output includes:

- Total number of accidents in the date range.
- All accidents ordered by date from most recent to oldest, including:
  - Accident code.
  - Date and time.
  - Day of the accident.
  - Location.
  - Address.
  - Severity.
  - Type of accident.
  - Latitude and longitude.

### Requirement 2: Report accidents during specific hours for a given month and year (Group)

As a traffic analyst, I want to know about accidents occurring during specific hours in a given month and year. The output includes:

- Total number of accidents in the given time interval.
- All accidents ordered from oldest to most recent within the time interval, including:
  - Accident code.
  - Time of the accident.
  - Date.
  - Day.
  - Location.
  - Address.
  - Severity.
  - Type of accident.
  - Latitude and longitude.

### Requirement 3: Report the 3 most recent accidents of a specific type along a road (Individual)

As a traffic analyst, I want a report on the 3 most recent accidents of a certain type along a specific road. The output includes:

- Total number of accidents along the road of the specified type.
- The 3 most recent accidents with details, including:
  - Accident code.
  - Date and time.
  - Day.
  - Location.
  - Address.
  - Severity.
  - Type of accident.
  - Latitude and longitude.

### Requirement 4: Report the 5 most recent accidents within a date range with a specific severity (Individual)

As a traffic analyst, I want a report on the 5 most recent accidents that match a specified severity within a date range. The output includes:

- Number of accidents for the date range.
- The 5 most recent accidents with details, including:
  - Accident code.
  - Date and time.
  - Day.
  - Location.
  - Address.
  - Type of accident.
  - Latitude and longitude.

### Requirement 5: Report the 10 least recent accidents in a given locality for a specific month and year (Individual)

As a traffic analyst, I want a report on the 10 least recent accidents in a locality for a specific month and year. The output includes:

- Number of accidents in the locality during the given date.
- The 10 least recent accidents with details, including:
  - Accident code.
  - Date and time.
  - Day.
  - Address.
  - Severity.
  - Type of accident.
  - Latitude and longitude.

### Requirement 6: Show N accidents within a specific area for a month and year (Group)

As a traffic analyst, I want to see a report of N accidents that occurred within a specific circular area for a given month and year. The output includes:

- N accidents organized by proximity to the center of the area.
- Details of each accident, including:
  - Accident code.
  - Date and time.
  - Day.
  - Location.
  - Address.
  - Severity.
  - Type of accident.
  - Latitude and longitude.

### Requirement 7: Report the earliest and latest accidents for each day of a month and year (Group)

As a traffic analyst, I want to see the earliest and latest accidents for each day of a given month and year, as well as a histogram of accident frequencies by hour for that same month and year.

The output includes:

- For each day, the earliest and latest accidents with details:
  - Accident code.
  - Date and time.
  - Day.
  - Location.
  - Address.
  - Severity.
  - Type of accident.
  - Latitude and longitude.
- A bar chart showing the frequency of accidents by hour for the given month and year.

### Requirement 8 (Bonus): Visualize accidents of a specific type for a date range on a map of Bogotá (Group)

As a traffic analyst, I want to visualize accidents of a specific type within a date range on a map of Bogotá. The output includes:

- Total number of accidents in the date range.
- An interactive cluster map with markers for each accident, color-coded by severity.

[Back to top](#accidenttrafficanalysis)

## Usage

To use this template, you need to follow the steps below:

* Read the official project document published in the course official site at [BrightSpace](https://bloqueneon.uniandes.edu.co/d2l/home).
* Distribute the project functionalities and implementation responsibilities among the group members.
* Download the official dataset for the project at the course official site at [BrightSpace](https://bloqueneon.uniandes.edu.co/d2l/home).
* Unzip and load the dataset into the application at the [Data](./Data) folder.
* Import the necessary modules from [DISClib](https://github.com/ISIS1225DEVS/ISIS1225-Lib) into the MVC scripts at the [App](./App) folder.
* Implement the missing functions according to the project needs in the MVC scripts at the [App](./App) folder.
* Evaluate the implementation of the MVC scripts, record your tests and analysis in the documents at the [Docs](./Docs) folder (The report **MUST BE** in PDF format).

[Back to top](#accidenttrafficanalysis)

## Contact and support

For further information and contact, use the following links:

* Official Repository [DISClib](https://github.com/ISIS1225DEVS/ISIS1225-Lib).
* Repository for [Demo and Examples](https://github.com/ISIS1225DEVS/ISIS1225-Examples).

If you require further information, please contact us [via this email](mailto:isis1225@uniandes.edu.co).

[Back to top](#accidenttrafficanalysis)

## Contributing

Contributions are what make the open-source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this project better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".

Don't forget to give the project a star! Thanks again!

1. Fork the Project.
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`).
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`).
4. Push to the Branch (`git push origin feature/AmazingFeature`).
5. Open a Pull Request.

[Back to top](#accidenttrafficanalysis)

## License

Copyright 2020, Departamento de sistemas y Computación, Universidad de Los Andes.
Developed for the class _"ISIS1225 - Estructuras de Datos y Algoritmos"_ or _"ISIS1225 - Data Structure and Algorithms"_ in English.

This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.

This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the [GNU General Public License](http://www.gnu.org/licenses/) for more information.

[Back to top](#accidenttrafficanalysis)

## Authors and acknowledgment

* [Dario Correal](https://github.com/dariocorreal) is the original author and main developer of the library.
* [Santiago Arteaga](https://github.com/phillipus85) is a contributor and repository administrator. 
* [Luis Florez](https://github.com/le99) is a contributor and developed examples and tutorials for the library.

[Back to top](#accidenttrafficanalysis)
