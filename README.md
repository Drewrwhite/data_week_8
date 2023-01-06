# Code Review: BigQuery and the Cloud

#### By Drew White

#### Code Review - Demonstrating use of BigQuery and the Cloud with a visualization created using Looker. 

## Technologies Used

* Google Cloud
* Big Query
* Looker
* SQL
* Python
* Pandas
* Jupyter Notebooks

</br>

## Description:
### Part 1:  
* Using Python, creates a BigQuery client in `main.ipynb`.  
* In BigQuery, makes a new dataset called `plants` in project directory.  
* In `main.ipynb`, uses client to list the datasets in the BigQuery project. Confirms that the new `plants` dataset is there.  
* In `main.sql`, writes SQL code that will create a table in the plants dataset called `flower_shop`.  
* In `main.sql`, writes SQL code that will give table schema : `plant_id`, `species_name`, `variety_name`, `zone`, `price`.  
* In `main.sql`, writes SQL code that will insert values into `flower_shop` table.  
* Run code from `main.sql` in BigQuery so it add new table with values.  
* In `main.ipynb` writes Python code: `.list_tables()` to verify that `flower_shop` was created.  
* In `main.ipynb` writes Python code: `.get_table()` to verify schema of `flower_shop`.

### Part 2:
  The data set I chose to work with for my visualization was "Iowa Liquor Sales". This data set contained a lot of information : `invoice_and_item_number`, `date`, `store_number`, `store_name`, `address`, `city`, `zip_code`, `store_location`, county_number, `county`, `category`, `category_name`, `vendor_number`, `vendor_name`, `item_number` `item_description`, `pack`, `bottle_volume_ml`, `state_bottle_cost`, `state_bottle_retail`, `bottles_sold`, `sale_dollars`, `volume_sold_liters`, `volume_sold_gallons`.  
  
  I was interested in volume sold so I chose to make a line chart visualization for `volume_sold_liters`, reported by `date` filtered by `year`. It was interesting to see a significant spike in volume sold by liter in the year `2021` followed by a decrease in `2022`  
  
  ![Iowa_Liquor_Sales](images/Iowa_Liquor_Sales.png)

## Setup/Installation Requirements

* Clone by inputting following into terminal: 
  ```bash
  git clone https://github.com/Drewrwhite/data_week_7.git
  ```
* Navigate to directory:
  ```bash
  cd <directory>
  ```
* Open directory in VSCode:
  ```bash
  code .
  ```
</br>

## Known Bugs

* No known bugs

<br>

## License

[MIT](./license.txt)

_If you find any issues, please reach out at: **d.white0002@gmail.com**._

Copyright (c) _2022_ _Drew White_

</br>
