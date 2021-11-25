# edt-ts

OS: Fedora 34 \

Python: version 3.9 \
 
Python modules: \
* pandas \
* numpy \
* tslearn \
* sklearn \
* tsfresh \

These packages can be installed using pip, the version number is important (especially for tsfresh). \

The folder 'data' includes csv files for the running example as w**ell as the manufacturing use case.
The manufacturing use case data was originally in yaml form, converted to XES and then to csv. 

To start the script in terminal: python time_series.py {running, manufacturing}.

Parameters that have to be set: \
*use_case: if one of the existing use cases is to be reproduced, just enter the use case name e.g. running, manufacturing \
For a new dataset: \
*df: the dataframe has to be provided if a new dataset should be tried \
*id: the identifier of the instances e.g. uuid \
*result_column: whats the name of the column that specifies the result \
*variable_interest: if more than two categories exist, which category is of interest \
Optionally: \
*interval: if the intervals are to be set manually


To try with additional data the preprocessing step has to be adapted to fit the new data to the required format. 
See the functions "prepare_running" and "prepare_manufacturing" on what is expected.