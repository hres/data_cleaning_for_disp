# data_cleaning_for_disp

The code was used to clean up active ingredient names in the Drug_Product_Ingredients table from [Canada Vigilance Adverse Reaction Online Database](https://www.canada.ca/en/health-canada/services/drugs-health-products/medeffect-canada/adverse-reaction-database/canada-vigilance-adverse-reaction-online-database-data-structures.html)

The goal was to recognize active ingredients in salt forms, recognize synonyms for an active ingredient and correct typos,in order to map
active ingredient names to ATC code, NHP names or vaccine products.

The ultimate goal was to improve accuracy in the calculation of disproportionality analysis (the [new_cv_drug_rxn.R](https://github.com/hres/data_cleaning_for_disp/blob/master/new_cv_drug_rxn) file includes code for Disproportionality analysis that produce master_table_pt,master_table_hlt for the Disproportionality App)

The [global.R](https://github.com/hres/data_cleaning_for_disp/blob/master/global.R) file includes updated file path, which can be used directly with corresponding [ui.R](https://github.com/hres/cvapps/blob/master/apps/shinydisp2/ui.R),[server.R](https://github.com/hres/cvapps/blob/master/apps/shinydisp2/server.R) for Disp App.
