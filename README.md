### Important data files
    - `cases_final_v1.parquet.gzip` is the original cleaned DataPrep files spitted out from `Project51_109B_DataPrep.ipynb`. This files was used for inital EDA in `Project51_109B_EDA.ipynb`
    - `Project51_UnSupervised_Model.ipynb` uses the data file `cases_final_v1.parquet.gzip` and generates the summary of all the `opnion_text` column and saves them in the new column named `opinion_text_summary`. This is now saved to `cases_summary_v1.parquet.gzip`
    - `cases_final_nc_v1.parquet.gzip` is data parsed from the new North Carolina dataset which contains headset. I have also created a cleaned version of this dataset which only contains two colums text and summary. Which is saved to file `cases_final_nc_cleaned_v1.parquet.gzip`.  `cases_final_nc_cleaned_v1.parquet.gzip` dataset was used to train the Supervised Model in `Project51_Supervised_Seq2Seq_Model.ipynb`. 

### Weight Files
    - The model weights are saved to `Seq2Seq.h5`. Which can be used to generate summary from Supervised Model.
