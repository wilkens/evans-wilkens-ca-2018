# London Geographies
Code, data, and figures supporting Evans and Wilkens, "Nation, Ethnicity, and the Geography of British Fiction, 1880-1940" (*Cultural Analytics*, 2018).

## Notes on data and code
The code in the `London CA.ipynb` notebook loads bibliographic and geographic data produced by the HathiTrust digital library and the Textual Geographies project. Sources and corpora are described minimally in the notebook and in full in the article (link forthcoming on publication).

The analyses presented in the notebook are a proper superset of those included in the article. We have made no attempt to pare the code to only results and figures discussed in CA.

The `Geotypicality.ipynb` notebook contains code to produce the related [interactive visualization](https://plot.ly/~mattwilkens/119/british-literary-geography-1880-1940/#/) of corpus authors' geographic usage.

The `results/` directory contains text output of results derived from the input data. These include statistical tables, corpus listings, etc. Most, but not all, of the same data is displayed in the notebooks themselves.

The `figures/` directory contains static visualizations.

All the content in both of these directories can be regenerated by executing the notebooks.

In addition to the usual Python data science stack (we use Anaconda), four things are required to run the code in the notebooks:

* The `cartopy` and `plotly` packages. Available via `conda install cartopy plotly`
* A [MapBox access token](https://www.mapbox.com/help/how-access-tokens-work/)
* A [Plot.ly API token](https://plot.ly/python/getting-started/).

To execute the notebooks in full from the command line, run:
```
jupyter nbconvert --ExecutePreprocessor.timeout=-1 --to notebook --execute "<filename>"
```

## Expanded bibliographies

Lists of the volumes included in the study are located in the `results/publication/` directory. They have names like `corpus_listing_Hathi.csv`, etc.

We are also making available our larger [working bibliographies](https://docs.google.com/spreadsheets/d/1Wq-Ho7clTt6-_t3e1VfJbf0Grilf-JRyGhul2A0XDRc/edit?usp=sharing) culled from the critical sources identified in the article. These include volumes not held by Hathi and volumes published outside our target date range. The bibliographies also include additional metadata in some cases.

The larger bibliographies are being released in case they may be useful to other researchers working on related problems. We make no representations concerning accuracy for any volumes not included in the article corpus listings. Use at your own risk.
