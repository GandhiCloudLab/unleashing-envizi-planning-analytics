# Unleasing Planning Analytics AddOn in IBM Envizi

Organizations are moving towards integrated planning that includes ESG(Environmental Social Governance) metrics. They are looking for a planning solution that can meet all their planning requirements. Existing planning and forecasting tools have not been designed to manage ESG data models. Also the ESG data management, planning and reporting is increasingly being integrated into existing business processes and required to meet rigorous standards. Expanding ESG reporting disclosure requirements and increased scrutiny on ESG performance organizations are looking for sophisticated, customized tools to support ESG planning and forecasting that helps them deliver integrated planning
   
Planning and Forecasting for ESG is at the intersection between Sustainability and Planning. This is where bringing together IBM Envizi ESG Suite and Planning Analytics can help Organizations on Integrated planning that can meet all the customer’s requirements where IBM Envizi ESG Suite looks at historical and the current ESG ledger for reporting + disclosure to demonstrate compliance and
IBM Planning Analytics helps in ESG planning for emissions reduction to meet KPIs and Net Zero targets.

Now lets look at how we can Accelerate decarbonization - Plan a low carbon future with Envizi’s planning & forecasting solution

IBM Planning Analytics (PA) for Envizi is an AddOn solution that enables customers to leverage the advanced forecasting and scenario modelling capabilities and apply those to their ESG data in IBM ESG Envizi Suite.

In this article you will understand about the following.

- How the data exchange happens via the API-based file exchange from Envizi to PA for secure, reliable and automated means for data transfer

- How data Cube replicates the Envizi data structure in a Planning Analytics environment and how it enables users to leverage their sustainability data to do custom modelling and forecasting.
- How to accelerate decarbonization and plan for a low carbon future using the Activity and Emissions Forecasting using scenario modelling. You will uncover how Envizi customers can leverage Planning Analytics to plan and forecast for ESG using Accelerator 1: Activity and Emissions Forecasting which gives you a starting point for planning and setting emissions reduction targets.


Let's start by launching the accelerator and getting familiar with the templates and dashboards available. And perform simple calculations on those forecasts to develop targets, which we will export and bring back into Envizi for performance monitoring.

## Prerequisite

1. Envizi Instance access with IBM Planning Analytics addon enabled.

## High Level Architecture

Here is the high level Architecture of the Integration of the Envizi and IBM Planning Analytics addon.

![img-11.png](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/SI-WUpzH-iy7W9uyhaSxWw/img-11.png)

 ## Objective

## 1. Envizi platform

Let's consider the Organization Hierarchy of Envizi is looking like the below.

1. Click and expand the `420 George St` Location.

![img-12.png](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/PT4i4B9mvD5ajEWfAaE2kA/img-12.png)

2. You can view the location details.

![img-13.png](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/h9GoQCEfakAh0SBaqM5QRA/img-13.png)

## 	2. Launch PA and Envizi accelerator

1. Launch PA platform using IBM Id.
2. Click the tile `Envizi Activity and Emissions forecasting`.

![img-21.png](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/lg9rerSUTqsN-1jJ8yDelQ/img-21.png)

3. Ensure the `Accelerator 1 – Account` on the left side

![img-22.png](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/s9ATXsoGHrpUgAEf1CMUgw/img-22.png)

4. Close the side-pane on the left side of the screen (to ignore other workbooks in the accelerator at this stage) 

![img-23.png](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/LClJZd8LU0yi3D3gmOkcew/img-23.png)

## 	3. PA Welcome Screen

The first screen of the accelerator provides an overview of the templates and dashboards available. For each tab, the following explanation are provided.
- the purpose
- capabilities to explore
- next steps

## 	4. PA Data Exploration & Forecasting 

- Exploration grid is like a flexible pivot table
- Add, edit or remove objects (dimensions) in your workbench to change how data is displayed and grouped in the exploration grid
- Envizi data is updated daily

The Data Exploration & Forecasting tab has a number of different elements in it.

The first to understand is the Exploration Grid.

1. Looking at the Exploration Grid, I can see my Envizi data has been brought in to Planning Analytics – there is no need for me to set up the cubes or any dimensions.
This is all handled by the integration’s automated processes, which also ensure data is updated daily, so that users are referencing the latest figures from Envizi. 
You can think of this grid as flexible pivot table.

![img-35.png](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/d6wOXfsuQMtIS4DjcLGFmw/img-35.png)

2. Above the exploration grid are several Filter Widgets. These can be used to select or filter on different dimension members.

![img-36.png](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/sv1kRH0OfE79VazrDKLjzQ/img-36.png)

Let’s change the filters on our dashboard now:

3. Select the `Property Group` member from the `Classifications` filter widget (You may need to drill down through the members to do so).

![img-37.png](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/vfTifnpFMy9KzmKBIdUxQA/img-37.png)

## 5. Set up forecast: Measures, Scenario

Let’s say I’m a Sustainability Manager, I’m responsible for demonstrating how the company can meet future GHG reduction targets. I might want to see what future projections of activity or emissions might look like based on historical patterns. 
I might then use those figures to make a case for investing in sustainability projects to bring down those figures further.
First let’s ensure we are forecasting emissions.

1. Set Envizi Measure Value to CO2e (kgCO2e)

![img-41.png](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/GcfCRDwzkMECZ0S13Tvmgg/img-41.png)

Let’s say I’m interested in emissions generated from electricity usage. Perhaps I’m looking to make a case for installing sensors that automatically control the switching on and off lights at a building I manage, say  `420 George St`.

2. Let’s drill down to that location so we can forecast on it. To drill down and filter data.  Select the `Classification` drop down in the filter and expand as below from 

`All > Property Group > Commercial -L1 > Portfolio A – L2 > 420 George St`

Note that we could also get to this level using the filter widgets at the top of the screen as shown.

![img-42.png](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/bN0seC0xAe5lX-GytsZdcg/img-42.png)

Now after expanding the building, we can see the individual accounts under it, currently there are 2 accounts: 
- Electricity account 
- Water account
Note that these accounts are named as they are in Envizi, but account numbers and other attributes can be shown as well.

![img-43.png](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/maEPMB7R6B4vKNKdk50jEw/img-43.png)

## 6. Create Sandbox

Creating your own sandbox let you to work in your private workspace

1. Click on the grid and highlight any of the row, I have highlighted same `420 George St.` record.
![img-46.png](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/dQFvtT2Vnee1gmg9_LJmXg/img-46.png)

2. Click on `Base` option in the menu bar to Create Sandbox

![img-47.png](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/2tpD2_TlbK4CVWwEo9Ai7A/img-47.png)

3. Give a name to sandbox 
4. Choose `Create sandbox` from Base as shown below 
5. Click `Create` button.

![img-48.png](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/Ccux2-gu9ZoXQkd_aFPokw/img-48.png)

6. Once you have created validate by viewing the menu bar to show your Sandbox name as highlighted below

![img-49.png](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/hjCvugJQ6P9Dwtmy0fTI0A/img-49.png)


## 7. Univariate Forecast

Now let’s demonstrate the AI assisted forecasting functionality in Planning Analytics. 
I can run a univariate forecast on the available actuals data (for demonstration purposes our data set has been loaded up until June 2024); and Planning analytics will use artificial intelligence to examine this data and determine trend, seasonality or other factors, and apply the most appropriate mathematical forecasting model to it.

To begin let’s ensure our account is selected in the grid:

1. Select `1263546 Elec` Account from the exploration grid

![img-51.png](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/r5SrqvSGo1hymnf6-YISxQ/img-51.png)

2. You can also reset already forecasted values for 2025 to 2030 as 0 if needed for the Electricity record

![img-52.png](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/DPcNbN1BwFnYG2tKtYJAbg/img-52.png)


I can then run a univariate forecast on this

3. Select `Forecast -> Univariate Forecast`

![img-53.png](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/zwlpkFZSaWd03Q28fgukIA/img-53.png)

4. I now need to determine options necessary for the forecast. 

#### Set Up
- Forecast Period Start = Jul-2024
- Forecast Period End = Dec-2030
#### Advanced
- Seasonality Auto Detect = On
- Use Historical Data in the TM1 Cube = On
- Confidence Interval = 95%
- Adjust Outliers = On
- Ignore Historical Time Periods = None selected
- Spread Forecast Values = Relative proportional (Seasonality)
#### Where to Save predicted values:
- Dimension = Model - Forecast
- Hierarchy = Model – Forecast
- Member = Baseline

![img-55.png](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/beqeJGqTGqDPyrT268g0vQ/img-55.png)

![img-56.png](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/3h8u2kug47SmVI5gCiO9Dg/img-56.png)

Once I am happy with this; I can run a preview of my forecast to see visually what it has calculated.

5. Select `Preview` from the above screen.

Note the chart shows a clear trend and seasonality in this data. I can also view the statistical and mathematical details of this forecast if I want.

![img-57.png](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/ClMneAuu7Bor78qNPeOLCg/img-57.png)

6. Select `Statistical Details`

![img-58.png](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/a3yzp_jeDDVffdbCP4gtUw/img-58.png)


Once I’m happy with this forecast, I can now calculate it and write it to the planning analytics database.

7. Close `Preview`
8. Select `Forecast` (note this can be done even if a forecast already exists for this account)

![img-59.png](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/er6TRpqUgqxGF5UYsZayxg/img-59.png)

9. You will get popup to confirm.  Click on `Continue`

![img-60.png](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/ib2gQkILkBGgVIzcgjJlQA/img-60.png)

10. Check the forecasted values for year 2025 – 2030 as highlighted

![img-62.png](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/KsA9ARcHaJ8800MynYXu7Q/img-62.png)

## 8. Rudimentary target setting

Let’s now make some adjustments to a forecast to develop a target.

Let’s assume that I’m a Sustainability Manager, and I want to develop targets appropriate to specific office locations or sites, so that I can bring those targets back into Envizi to monitor performance.

Performance calculation and data spreading
- Planning Analytics supports various calculations to enhance analysis
- Data spreading capability makes it easy to apply calculations across a range of cells
- Text-based commands provide a shortcut to data spreading calculations
Using my emissions forecast I’m going to set a rudimentary target of 5% reduction for the year of 2024, then reduce by an additional 5% for the 2H of the year.
To do that I’m going to perform a simple percent reduction calculation on 2024 values.
For this example, I’m going to use 420 George as my chosen location.
Note: a forecast has already been created for 2024
Next, I’m going to set up my calculation to apply to my 2025 forecasted values
 
1. On `2025` column, right click on `Level Options > level000` to get monthly view

![img-66.png](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/ohk5dFLBwfmKajBN1R22wA/img-66.png)

Highlighted is the monthly view.

![img-67.png](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/lOXtlG-VyZV2WVTNI3M-jw/img-67.png)

2. `Right-click` select the `first cell` containing a forecast for `2025-01-01`
3. Select `Spread data options` from the context menu

![img-68.png](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/p7V7WyyAQ9If4IaJn-6ojw/img-68.png)

4. I want a percent change, select `Percent change` from the left-hand list
5. I want that change to be 5%, type `5` in the text field
6. As a reduction, select `Subtract` as the `update action`
7. Select `Right` and `Down` as the `direction`
8. Select `Apply` button

![img-69.png](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/_bUM1r3cxAHpDv6ED1BcUw/img-69.png)

9. Adjust the filters now to reflect for `420 George St` as below: 
10. Select the `column 2025` on the top row, 
11. Right click and choose the menu > `Level Options > Level000`

![img-70.png](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/JiH8fPYYNZIW_Oruu2V8Ng/img-70.png)

Now you can see the monthly view of the forecasted values.

12. Looking at the grid, I can see my 2025 values drop.

![img-71.png](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/lI6VDr4_ldZ0ODOeVQheYw/img-71.png)


## 9. Populate the targets from PA to Envizi

Exporting the emissions targets into Envizi.

Now that I have my rudimentary targets, I want to use them to populate my Envizi fixed targets.
1. Narrow down to the data that you want to export using filters to narrow down for a specific location. 
2. `Highlight` the record on the grid 
3. Click on `Export icon` in the menu bar.

'![img-75.png](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/K9f_tIH-jg4KWdDBtL3aQQ/img-75.png)

4. If am I’m going to use the exploration grid to copy those values,  Copy 2025 values into Excel sheets

'![img-76.png](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/Q-aGRQX7LevY80P30qIGXA/img-76.png)

## 10. Load populated targets template

Loading target data simply involves uploading the pre-filled template

Now, let’s switch over to Envizi to load my targets
1. Launch Envizi window in a new browser tab
2. In the Main menu select `Manage >Targets and Rates > Fixed Targets` to Upload the populated emissions targets data 

'![img-77.png](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/2vt8lRCtscbZcDRSVcQj5Q/img-77.png)

3. Select the Target Name `420 George Street Emissions Target` created

![img-78.png](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/cT_v6pLkyNg4ClJyPiRfcg/img-78.png)

4. Right-click select `420 George Street Emissions Target` from the list
5. Select `Target data`

![img-79.png](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/YvrII24wlepmpJwvoQkPaw/img-79.png)

Verify the Monthly Target Data created, and you see the Target Data from 2024 out to 2030 based on the Target data that we exported from PA.

![img-80.png](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/lDTBQbxHRTRMaQCCgOXN0w/img-80.png)

## 11. View targets report

Let’s now open the report for 420 George St to see the targets in context in Envizi
1. In the Search bar, select `Reports` and type `420 George`

![img-85.png](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/vJ_vO1b0_jBEDiBGL50Vcg/img-85.png)

2. Click on `420 George Street Targets` PowerBI report to view the report

![img-86.png](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/wsBxtX5vN3X4SywG67tc-g/img-86.png)

Now I can see my emissions against my targets

![img-87.png](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/0D2r_ij1NOFVegQmzYQtIA/img-87.png)


On the Chart you can see the purple lines which represents the actual reportable data that is captured and managed in Envizi. 

We can also see the blue line which represents the forecast values that is created in PA that is now configured now as Targets in Envizi As the Target now resides in Envizi users can track the actual emissions compared to the target over time to understand if they are on the track to meet their targets.

The targets can be reviewed and remodelled in the PA at any time ( eg: To change in the business operations) and the Target in Envizi can be updated accordingly.

## Conclusion 

In conclusion, We have explored how Envizi addon with Planning and Analytics works. You also learnt how to leverage export from PA and ingest into Envizi to make more informed carbon reduction targets. With this entry-point solution you were able to develop an indicative forecast. With user-driven values and a linear regression model, you could also gauge the trajectory of future performance.

With this Addon capability that brings Envizi and Planning Analytics together enables Partners to build custom solutions
to provide customers with the flexibility to address their specific planning needs beyond general market requirements in the space of scenario modelling and forecasting.

For more information about IBM Envizi or to try it out yourself, start your 14-day IBM Envizi ESG Suite trial. You can also request a personalized IBM Envizi demo.
