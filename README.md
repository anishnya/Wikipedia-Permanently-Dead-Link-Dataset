# Wikipedia-Permanently-Dead-Link-Dataset
This repository contains the dataset for 'Characterizing “Permanently Dead" Links on Wikipedia' IMC 2022 paper. The dataset contains 10,000 links in a JSON format. For any questions, or more information, please feel free to contact anishnya@umich.edu.  

This is the following structure of the data. 

```
{
    "url": <string>,
    "article_url": <string>,
    "current_status": <string>,
    "date_link_posted": <string>,
    "date_link_marked_dead": <string>,
    "copy_after_posted": [<string>, <string>],
    "copy_before_marked_dead": [<string>, <string>],
    "copy_after_marked_dead": [<string>, <string>]
}
```
For archived copy data, this is the following format. 

```
[Archived Copy Date, Archived Copy Status Code]
```

For all dates, they are in the following format: YYYY-MM-DDTHH:MM:SS+00:00. Packages such as arrow-py, can automatically parse dates in this format. 

