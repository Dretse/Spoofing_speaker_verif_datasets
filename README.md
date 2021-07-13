# Spoofing_speaker_verif_datasets
This project contain the description of the datasets associated with the experiments of the "Spoofing Speaker Verification With Voice Style Transfer And Reconstruction Loss" paper, submitted for the 13th IEEE International Workshop on Information Forensics and Security (WIFS 2021).

## Datasets format
This project contain seven description files in **.csv** for the datasets.<br>
Each file correspond to the sets described in the table II of the paper :<br>

Datasets| From | Speakers | Files | Associated csv<br>
--------------- | ------------ | ---- | ------------ | ------
**Template**    | *VoxCeleb 1* | 1251 | 148642  | VoxCeleb1_test.csv <br>
**ASV_train**   | *VoxCeleb 2* | 5395 | 939766  | VoxCeleb2_train.csv<br>
**ASV_valid**   | *VoxCeleb 2* | 5395 | 104419  | VoxCeleb2_valid.csv<br>
**ASV_test**    | *VoxCeleb 2* | 600  | 1547    | VoxCeleb2_test.csv<br>
**VST_train**   | *VCTK*       | 100  | 34733   | VCTK_train.csv<br>
**VST_valid**   | *VCTK*       | 100  | 3860    | VCTK_valid.csv<br>
**E_VST_Test**  | *VCTK*       | 10   |  3671   | VCTK_test.csv<br>

VoxCeleb2_train.csv is not available here due to its large size.

## Reading the files
We advise you to import them using [pandas library](https://pandas.pydata.org/) and use them with the [sidekit library](https://projets-lium.univ-lemans.fr/sidekit/).<br>
Each speech utterance is represented as a line, and  the files contain the following columns :
column name : | 	dataset |	speaker_id |	file_id |	start |	duration |	gender 
 -------------|-----------|------------|----------|-------|----------|---------
contains :    | source dataset name |	speaker reference in the dataset |	path to the file of the speech utterance |	start of the file |	end of the file 	| gender 
example : | VCTK |	p347 |	p347/p347_373_mic1 |	0 |	2.04 |	M
