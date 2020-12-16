# WaterProject
Data science water project.
training_labels = pd.read_csv ('https://raw.githubusercontent.com/onaio/ona-tech/master/data/water_points.json', encoding = 'iso-8859-1')
training_lables.head()
piv_df= training_df[['basin','status_group','status_values']]
piv_table = piv_df.pivot_table(index='basin',
                           columns='status_group', aggfunc='count')
piv_table
