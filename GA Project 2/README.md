# ![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png) Project 2: Ames Housing Data and Kaggle Challenge

### Project Objectives:

You have been tasked by your direct supervisor to create a regression model to predict the price of houses in Ames, so that these prices can be included in the platform. You will also need to identify factors affecting sales price and make recommendations on what could be done to improve sales income.

---

### Data used:

For the purpose of the analysis, we are provided with the `train` and `test` datasets. The `train` dataset contains Ames' housing sales prices and their relevant information from 2006 to 2010. We will be using this dataset for model building purposes. The `test` dataset contains another set of Ames' housing sale price, but does not include the sale prices. We predicting the sale prices found in this dataset instead.

Information found in the `train` datasets includes information suchs as the sale prices, building class, information on the pool, basement, neighbourhood, garage and overall quality of the house. The full information could be found in the data dictionary below.

Information found in the `test` datasets contains the same fields as those found in thte `train` dataset, except for the sale prices.

---

### Data Dictionary:

<br>**Dataset name: `test`**
<br>This dataset contains data of houses that have been sold over from 2006 to 2010. 

| Feature | Type | Dataset | Description |
|:--|:-:|:-:|:--|
|id|int|Train|Identification number.|
|pid|int|Train|Parcel identification number.|
|ms_subclass|int|Train|The building class.|
|ms_zoning|string|Train|Identifies the general zoning classification of the sale.|
|lot_frontage|float|Train|Linear feet of street connected to property.|
|lot_area|int|Train|Lot size in square feet.|
|street|string|Train|Type of road access to property.|
|alley|string|Train|Type of alley access to property.|
|lot_shape|string|Train|General shape of property.|
|land_contour|string|Train|Flatness of the property.|
|utilities|string|Train|Type of utilities available.|
|lot_config|string|Train|Lot configuration.|
|land_slope|string|Train|Slope of property.|
|neighborhood|string|Train|Physical locations within Ames city limits.|
|condition_1|string|Train|Proximity to main road or railroad.|
|condition_2|string|Train|Proximity to main road or railroad (if a second is present)|
|bldg_type|string|Train|Type of dwelling.|
|house_style|string|Train|Style of dwelling.|
|overall_qual|int|Train|Overall material and finish quality.|
|overall_cond|int|Train|Overall condition rating.|
|year_built|int|Train|Original construction date.|
|year_remod/add|int|Train|Remodel date (same as construction date if no remodeling or additions).|
|roof_style|string|Train|Type of roof.|
|roof_matl|string|Train|Roof material.|
|exterior_1st|string|Train|Exterior covering on house.|
|exterior_2nd|string|Train|Exterior covering on house (if more than one material).|
|mas_vnr_type|string|Train|Masonry veneer type.|
|mas_vnr_area|float|Train|Masonry veneer area in square feet.|
|exter_qual|string|Train|Exterior material quality.|
|exter_cond|string|Train|Present condition of the material on the exterior.|
|foundation|string|Train|Type of foundation.|
|bsmt_qual|string|Train|Height of the basement.|
|bsmt_cond|string|Train|General condition of the basement.|
|bsmt_exposure|string|Train|Walkout or garden level basement walls.|
|bsmtfin_type_1|string|Train|Quality of basement finished area.|
|bsmtfin_sf_1|float|Train|Type 1 finished square feet.|
|bsmtfin_type_2|string|Train|Quality of second finished area (if present).|
|bsmtfin_sf_2|float|Train|Type 2 finished square feet.|
|bsmt_unf_sf|float|Train|Unfinished square feet of basement area.|
|total_bsmt_sf|float|Train|Total square feet of basement area.|
|heating|string|Train|Type of heating.|
|heating_qc|string|Train|Heating quality and condition.|
|central_air|string|Train|Central air conditioning.|
|electrical|string|Train|Electrical system.|
|1st_flr_sf|int|Train|First Floor square feet.|
|2nd_flr_sf|int|Train|Second floor square feet.|
|low_qual_fin_sf|int|Train|Low quality finished square feet (all floors).|
|gr_liv_area|int|Train|Above grade (ground) living area square feet.|
|bsmt_full_bath|float|Train|Basement full bathrooms.|
|bsmt_half_bath|float|Train|Basement half bathrooms.|
|full_bath|int|Train|Full bathrooms above grade.|
|half_bath|int|Train|Half baths above grade.|
|bedroom_abvgr|int|Train|Number of bedrooms above basement level.|
|kitchen_abvgr|int|Train|Number of kitchens.|
|kitchen_qual|string|Train|Kitchen quality.|
|totrms_abvgrd|int|Train|Total rooms above grade (does not include bathrooms).|
|functional|string|Train|Home functionality rating.|
|fireplaces|int|Train|Number of fireplaces.|
|fireplace_qu|string|Train|Fireplace quality.|
|garage_type|string|Train|Garage location.|
|garage_yr_blt|float|Train|Year garage was built.|
|garage_finish|string|Train|Interior finish of the garage.|
|garage_cars|float|Train|Size of garage in car capacity.|
|garage_area|float|Train|Size of garage in square feet.|
|garage_qual|string|Train|Garage quality.|
|garage_cond|string|Train|Garage condition.|
|paved_drive|string|Train|Paved driveway.|
|wood_deck_sf|int|Train|Wood deck area in square feet.|
|open_porch_sf|int|Train|Open porch area in square feet.|
|enclosed_porch|int|Train|Enclosed porch area in square feet.|
|3ssn_porch|int|Train|Three season porch area in square feet.|
|screen_porch|int|Train|Screen porch area in square feet.|
|pool_area|int|Train|Pool area in square feet.|
|pool_qc|string|Train|Pool quality.|
|fence|string|Train|Fence quality.|
|misc_feature|string|Train|Miscellaneous feature not covered in other categories.|
|misc_val|int|Train|$Value of miscellaneous feature.|
|mo_sold|int|Train|Month Sold.|
|yr_sold|int|Train|Year Sold.|
|sale_type|string|Train|Type of sale.|
|saleprice|int|Train|The property's sale price in dollars.|

---

### Key takeaways from the project:
1. The model that is the best at predicting sale price is the **Ridge Regression** model with a test $R^2$ score of 89.4%.

2. Features such as "Above Ground Living Area", "Overall Quality of the House" and "Overall Condition of the House" are good predictors of sale prices.

3. Houses that are located in "Commercial" areas and "Residential Medium Density" areas or neighbourhoods such as "Edwards" and "Oldtown" are likely to have lower sale prices. 

_Note: The Kaggle score (RMSE) for the production model was 27,051._

---

### Recommendations:
Recommendations are focused on targeting the right home owners as homes with higher sales price will command higher commission income as commission income is usually based on a percentage of the sale prices. The recommendations are as follows: 
1. Should spend more efforts on target bigger and well maintained houses as these houeses are likely to command higher sale prices. Higher sale prices will result in higher commission income.
2. Communicate the findings to potential sellers so that they can do minor renovations / maintainence works to try to boost the houses' sale prices. The sellers might be willing to maintain their houses if the benefits exceed the costs.

