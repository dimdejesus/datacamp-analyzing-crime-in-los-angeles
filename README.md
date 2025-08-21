# Analyzing Crime in Los Angeles
A project in Associate in Data Science in Datacamp to investigate the crimes in Los Angeles

![Los Angeles skyline](la_skyline.jpg)

Los Angeles, California 😎. The City of Angels. Tinseltown. The Entertainment Capital of the World! 

Known for its warm weather, palm trees, sprawling coastline, and Hollywood, along with producing some of the most iconic films and songs. However, as with any highly populated city, it isn't always glamorous and there can be a large volume of crime. That's where you can help!

You have been asked to support the Los Angeles Police Department (LAPD) by analyzing crime data to identify patterns in criminal behavior. They plan to use your insights to allocate resources effectively to tackle various crimes in different areas.

## The Data

They have provided you with a single dataset to use. A summary and preview are provided below.

It is a modified version of the original data, which is publicly available from Los Angeles Open Data.

# crimes.csv

| Column     | Description              |
|------------|--------------------------|
| `'DR_NO'` | Division of Records Number: Official file number made up of a 2-digit year, area ID, and 5 digits. |
| `'Date Rptd'` | Date reported - MM/DD/YYYY. |
| `'DATE OCC'` | Date of occurrence - MM/DD/YYYY. |
| `'TIME OCC'` | In 24-hour military time. |
| `'AREA NAME'` | The 21 Geographic Areas or Patrol Divisions are also given a name designation that references a landmark or the surrounding community that it is responsible for. For example, the 77th Street Division is located at the intersection of South Broadway and 77th Street, serving neighborhoods in South Los Angeles. |
| `'Crm Cd Desc'` | Indicates the crime committed. |
| `'Vict Age'` | Victim's age in years. |
| `'Vict Sex'` | Victim's sex: `F`: Female, `M`: Male, `X`: Unknown. |
| `'Vict Descent'` | Victim's descent:<ul><li>`A` - Other Asian</li><li>`B` - Black</li><li>`C` - Chinese</li><li>`D` - Cambodian</li><li>`F` - Filipino</li><li>`G` - Guamanian</li><li>`H` - Hispanic/Latin/Mexican</li><li>`I` - American Indian/Alaskan Native</li><li>`J` - Japanese</li><li>`K` - Korean</li><li>`L` - Laotian</li><li>`O` - Other</li><li>`P` - Pacific Islander</li><li>`S` - Samoan</li><li>`U` - Hawaiian</li><li>`V` - Vietnamese</li><li>`W` - White</li><li>`X` - Unknown</li><li>`Z` - Asian Indian</li> |
| `'Weapon Desc'` | Description of the weapon used (if applicable). |
| `'Status Desc'` | Crime status. |
| `'LOCATION'` | Street address of the crime. |

## Questions and Answer
What I'll be placing in the answer are just text format please refer to [notebook.ipynb](./notebook.ipynb) for the code 

**Question #1**: Which hour has the highest frequency of crimes?

**Answer**: The one with highest frequency of crimes is during **12** in the afternoon.

**Question #2**: Which area has the largest frequency of night crimes (crimes committed between 10pm and 3:59am)?

**Answer**: The area with the highest frequency of crimes during night time is **Central**.

**Question #3**: Identify the number of crimes committed against victims of different age groups. Save as a pandas Series called victim_ages, with age group labels "0-17", "18-25", "26-34", "35-44", "45-54", "55-64", and "65+" as the index and the frequency of crimes as the values.

**Answer**: The number of crimes commited to the victims (grouped by category).
| Victim Age Group | Number of Crimes |
|--------|-------------|
| `26-34` | 47470 |
| `35-44` | 42157 |
| `45-54` | 28353 |
| `18-25` | 28291 |
| `55-64` | 20169 |
| `65+` | 14747 |
| `0-17` | 4528 |

## Analysis Steps
1. Data Loading: Used the given `crimes.csv` to analyze
2. Data Exploration: Look into the data and take advantage of what it gives
3. Data Processing: Use python, pandas, and numpy to filter the data to produce an answer to the question provided.

## Libraries used
* Python
* Pandas
* Numpy
* Seaborn

## How to run
1. Clone this repo through https or ssh.
2. Run this on virtual env `you don't want your local python setup to be messy ;)`
3. Run this command
```
pip install -r requirements
```
4. Open it through Jupyter Notebook, VS Code, or any text editor that you use.

## License
This project is licensed under the MIT License - see the LICENSE.md file for details

## Acknowledgement
* **Datacamp's** Associate Data Science in Python
* **Datalab** - I only placed it here because I used only the free versioon which limits me to 3 workbooks only