## Introducing Tableau Desktop

### Meet Tableau Desktop

- The focus of this course is on **Tableau Desktop**, a segment of the Tableau creator business intelligence role, which offers data connection and visualization capabilities alongside online sharing.
- Tableau has maintained a leading position in the Gartner Quadrant for a decade, demonstrating a remarkable vision and execution ability. It stands tall against competitors like Microsoft, Click, and Thoughtspot, among others.
- **Salesforce**'s recent acquisition of Tableau is expected to further enhance Tableau's position in the market.
  
  - **Key features of Tableau include**:
      - A rich library of connectors allowing integration with various data sources including flat files, databases, cloud sources, and APIs. 
      - Tools to facilitate data understanding through sorting, grouping, and filtering, and enabling the creation of visualizations through a no-code interface.
      - The ability to perform robust custom calculations using Excel-like functions.
      - Renowned for visualization capabilities, helping to transform flat data into actionable insights with powerful dashboards and story elements.
      - A vibrant user community for networking and knowledge exchange.

### Tableau Desktop Interface & Workflow

- In this session, we delve into the **Tableau Desktop interface** which is structured into three key layers: **sheets, dashboards, and data sources**.
  - **Sheets**: 
    - The primary location for creating content, with each sheet representing a visualization. 
    - Sheets constitute the underlying elements of dashboards.
  - **Dashboards**:
    - Collections of sheets and other objects that enable users to interact with data and derive needed information.
    - It allows for previewing and understanding how different sheets and objects such as filters and images interact within the dashboard.
  - **Data Sources**:
    - Facilitates raw data that supports sheets and dashboards, with features allowing data manipulation and integration from various sources.
    - It permits visualization of tables used for analyses, the applied filters, and understanding how metadata is oriented.

- The **workflow in Tableau Desktop** is sequential:
  - **Starting with the data source pane**: Where connections to raw data are made, and initial preparations including joining and filtering are done.
  - **Moving to sheets**: For data analysis, calculations, blending, and visualization.
  - **Ending with dashboards**: Where sheets are combined to create interactive dashboards that offer end users actionable business insights through data analysis and drill-down functionalities.

- A demonstration was performed showcasing the features of these three layers, promising deeper insights in the upcoming sections.

### Tableau Community & Resources

- The **Tableau platform** is divided into **products** and **user roles**:
  - **Products** comprise applications such as desktop prep and server that are available for purchase.
  - **User roles** are categorized into:
    - **Creator**: Grants access to all Tableau applications including the robust data preparation software, Tableau Prep, and the primary focus of this course, Tableau Desktop. Creators can develop and publish content to Tableau Server for end users to interact and export data.
    - **Explorer**: Allows limited access to desktop features through web authoring on Tableau Server and enables content consumption on the server.
    - **Viewer**: Primarily for consuming content hosted on Tableau Server.
      
- The **Tableau community** stands as a vital support system offering a plethora of resources such as:
  - Social media channels, blogs, and forums to find answers to your queries and to stay updated with the latest developments.
  - Engaging in local, regional, and global contests.
  - Learning opportunities through Tableau Zen Masters — a group of 35 experts globally recognized for mastering the platform and aiding the community.
  - Attending regional and international Tableau conferences to gain insights from industry leaders and peers worldwide.
    
- **Essential resources for a Tableau learner**:
  - The **Discover pane** in the Tableau Desktop application offers insights into online trainings, additional resources, whitepapers, and community updates.
  - **Tableau Community Forums** to find detailed answers to your Tableau-related questions through various formats including text, workbooks, and videos.
  - **Tableau Zen Masters**’ blogs offer a rich resource pool to learn from the best in the industry.
  - **Local Tableau user groups** provide networking opportunities with fellow Tableau enthusiasts in your locality, offering experiences beneficial for your learning journey.
  
- Utilize these resources effectively to enhance your proficiency and to stay connected with the global community of Tableau users.

## Connecting & Blending Data

### Data Connection Types

- In this Tableau Desktop online course segment, the instructor covers data connection types available in Tableau Desktop and Tableau Public app, emphasizing the following:

  - **Tableau Desktop Connections**:
    - **Flat Files**: Enables connection to CSVs, Excel, Access, PDFs, etc., with examples focusing on Excel and CSV files.
    - **Database Servers**: Connects to various database servers like SQL, Oracle, Hadoop, etc. Allows unlimited connections, enhancing analysis scope.
    - **Pro Tip**: Users can open new connections anytime through the top ribbon in the tool.
    - **Data Interpreter**: An aid to clean and prepare data before analysis, available for both CSV and Excel files.

  - **Tableau Public App Connections**:
    - **Limited Options**: Database connections are unavailable; however, several flat file connections are supported, including Excel, text files, JSON, and PDFs.
    - **Special Public Server**: Allows connection to a restricted number of published sources available on the Tableau public site.

  - **Working with Different Files**:
    - **CSV Files**: Showcases connecting to a text file, highlighting a straightforward process with a preview of available data.
    - **Excel Files**: Discusses advantages such as multiple tabs within a workbook which can be joined or related, and the utility of named ranges in large Excel files.
    
  - **Database Connection (Tableau Desktop)**:
    - **Requirement**: Needs full version of Tableau Desktop for database connections, using a Postgres database for demonstration.
    - **Connection Details**: Describes input of various credentials depending on the database server type.
    - **Standardized Process**: Tableau ensures a uniform procedure across different data source types, facilitating easier usage for analysts.
    - **SQL Integration**: Though Tableau is essentially a "SQL free zone," it provides features to help users learn SQL by viewing or writing SQL codes through visual join processes or by converting these processes to custom SQL, offering insights into the backend processes.
    - **Visual Joins**: Allows users to create joins visually, selecting keys, and understanding SQL code generation through an extra option in the database connection window.

*Note*: The course stresses the ease of using Tableau for connecting to a wide array of data sources and the availability of utilities like the data interpreter for pre-cleaning data, enhancing the analytical process. It also hints at an upcoming detailed discussion on joins in Tableau.

### The Data Source Interface

- **Data Source Interface in Tableau**
  - Main tool for connecting and customizing data before visualization.
  - Comprises several components:
    - **Connections pane**: Located on the left, it lists the data source, sheets, schemas, tables, and views you are connecting to.
    - **Canvas**: Drag sheets or tables from the connections pane to here; represents joins, unions, and tables to be brought into the workbook. Supports both visual joins and custom SQL code.
    - **Data Grid**: Previews rows and columns in your data source, showing field type, data samples, and allows data manipulation.
    - **Metadata Grid**: A vertical display focusing on field names and properties, showing column references and origin details.
    - **Filters**: Positioned at the top right, applies filters at the data source level, unchangeable by end users.
    - **Connection Type**: Choose between live or extract connection (not available in Tableau Public due to bandwidth management). 

### PRO TIP: Data Interpreter

- **Using the Data Interpreter in Tableau**
  - **Purpose**: To clean "dirty data" with extra headers, merged columns, and unnecessary rows and columns automatically.
  - **Applicability**: Only for Excel and CSV workbooks.
  - **Operation**:
    - **Activation**: Select the "Clean with data interpreter" checkbox.
    - **Processing**: AI automatically processes the data, which usually takes less than 10 seconds.
      
  - **Output**:
    - An Excel file detailing the results of the cleanup:
      - **Key Tab**: Offers insights into how columns were viewed and manipulated.
      - **Before and After Tabs**: Allow you to compare the original data and the cleaned version. Differentiates data values (green), column headers (red), and ignored or cleansed parts (white).
      - **Final Tab**: Displays the cleaned data to be used in Tableau.
        
  - **Practical Application**: 
    - **Step 1**: Open Tableau and select the Excel file to clean.
    - **Step 2**: Drag the chosen sheet (e.g., "orders") to the designated area.
    - **Step 3**: Check the data interpreter box on the left to initiate the process and view the nicely formatted result post-processing.
    - **Step 4**: For detailed insights into the cleanup, click "review the results" to open the generated Excel file with various tabs representing different stages of data cleaning.
    - **Visualization**: After cleaning, the data is more readable and ready for analysis in Tableau.
      
  - **Conclusion**: A quick and user-friendly tool to automate data cleaning with a single click, enhancing the data visualization process in Tableau.

### Transforming Data

- **Data Transformation in Tableau Desktop:**

  - **Data Source Interface**:
    - Initial preview of data available in data grid
    - Columns and their respective data types visible
    - Options to manipulate data on the right-side using carat icon

  - **Field Types and Geographic Roles**:
    - Can be assigned to different fields
    - 98% of initial data type determinations by Tableau are correct, but users can adjust based on their needs
    - Field types can be changed later while building visualizations

  - **Data Manipulation Options**:
    - **Renaming Fields**:
      - Won't affect the initial data source; changes retained within Tableau
    - **Hiding Columns**:
      - Helpful to hide unneeded columns from end users
    - **Grouping Data**:
      - Creates a new field that combines different data pieces not originally in the data source
    - **Pivoting Data**:
      - Simplifies analysis by changing the data structure
      - Can select multiple columns for pivoting using control or command button
    - **Splitting String Fields**:
      - Uses automatic or custom delimiters
      - Similar to Excel's text to columns functionality
    - **Field Type Conversion**:
      - E.g., Changing "row ID" field to string to prevent Tableau from aggregating it
    - **Splitting a Field**:
      - E.g., Using custom split on "order ID" to obtain state and year data
      - Newly created columns indicated with an equals sign
      - Renaming the newly created fields for descriptive understanding
    - **Hiding Unnecessary Fields**:
      - E.g., Hiding unnecessary split results
    - **Creating Custom Groups**:
      - E.g., Grouping different shipping modes under a new category "Basics"
    - **Pivot Function**:
      - Demonstrated with sales, quantity, discount, and profit columns
      - Transposes data to have a pivot field name and value column
      - Important for various analyses, although not used in the current context
      - Offers an "unlimited" undo option to revert changes made since the workbook was opened, including reverting saved changes.

### Unions & Joins

In this section of the Tableau Desktop online course, you will learn how to effectively utilize unions and joins to combine and manipulate data sources. Here's what was covered:

- **Unions**:
  - Appends rows of data from one table to another.
  - The process involves dragging tables/views under your primary table in the data view.
  - Offers customization options:
    - Specific manual configuration for choosing individual tables, views, or files.
    - Wildcard configuration for selecting files based on naming conventions.
  - Benefits include facilitating data union with different date separations and similar file names in a directory.

- **Joins**:
  - Combines data sources using keys rather than appending data.
  - Types of joins:
    - Inner join: returns only matching records from both tables.
    - Left join: retains all data from the left table and matching records from the right.
    - Right join: the opposite of left join.
    - Full outer join: combines all data, including non-matching records, creating nulls for non-matching values.
  - Creating a join involves dragging table views or tabs into your canvas and selecting a key if Tableau doesn't automatically find one.
  - Offers the option to create calculated fields in the join window to help create join keys.
  - Expert tip: Utilize custom SQL for more complex data joining.
  
- **Practical Application**:
  - Union extra records using the “Orders Add On” tab in your data source.
  - Customizing unions through editing options to ensure correct data amalgamation.
  - Joining the “Returns” table to the main orders data source to track returned orders using preferred keys and join types.
  - Essential to use unique join keys to avoid data distortion in your analysis.

Remember, in creating both unions and joins, you must understand your data source well, particularly field names and types, to ensure a successful and smooth process. It would be best to utilize the practical tips discussed here when you perform these actions in Tableau Desktop.

### Data Blending

In this section, you were introduced to the concept of data blending in Tableau Desktop, an essential technique used to combine data from various sources at the individual sheet level while keeping the sources fundamentally separate. Here are the key points to retain:

- **Data Blending Basics**
  - Combines data from multiple sources into a single view at the sheet level while keeping the data sources separate and independent.
  - The **primary source** is determined by the first field pulled into a sheet, and it generally holds all the dimensions for your views.
  - The **secondary source** should mainly be used to bring in measures, not dimensions.
  
- **Working with Primary and Secondary Sources**
  - Primary sources are marked with a blue check, and secondary ones with an orange check.
  - Fields sharing the same name and data type across primary and secondary sources automatically become available for blending.

- **Blend Relationships**
  - You can manually define how fields map between two sources using the "Edit Blend Relationships" menu.
  - Fields to blend need to have the same data type, though not necessarily the same name.
  - If fields have different data types, modify them to match before blending.
  - The data type holds more weight than the field name in the blending process.

- **Understanding Grain in Data Blending**
  - Ensure the secondary source dimensions are present in the primary source to facilitate blending at that level.
  - Blending is applied per sheet, and changing the primary source requires starting on a new sheet.
  - Understanding the grain of your data sources before starting is vital to avoid mistakes in selecting the primary source.
  - Recognize when blending is necessary, as many analyses can be performed with just joining and unions.

Remember that this is an initial discussion and you'll delve deeper into more advanced topics in future sessions. To effectively use data blending in Tableau Desktop, familiarize yourself with functionalities such as modifying data types, creating calculated fields, and understanding blending at different levels (like segment and region in the example). Moreover, the data blending concept can be likened to performing sums in Excel under certain conditions. Now, practice blending by creating a sheet in Tableau Desktop, considering the insights shared during the session.

### Live Connections vs. Extracts

In this Tableau Desktop online course module, the differentiation between live connections and extracts when working with data in Tableau Desktop is elucidated.

- **Live Connections**
  - Queries the underlying database or flat file every time a field is utilized — a factor that requires considering the performance of your data source.
  - The process involves significant interaction with the database, especially when multiple users are accessing a dashboard.
  - Identified with a single cylinder symbol in the dashboard.
  - Not supported in the Tableau Public app, exclusive to Tableau Desktop full application.

- **Extracts**
  - Allows data to be saved in Tableau’s proprietary hyper extract file format for regular refreshes.
  - Enhances performance and functionality while working with legacy systems or offline environments.
  - Comes with a set of limitations, accessible in Tableau Help documentation.
  - Supports large datasets and is faster to create, aiding in swift dashboard development.
  - Offline access is a beneficial feature, especially in environments not suited for Tableau Server or Tableau Online infrastructure.

Exploring further into extracts, the following points were covered:

- **Extract Options in Tableau Desktop Software**
  - **Data Storage**: Offers the choice between a single table (consolidates all data, beneficial for performing joins) and multiple tables (enhances efficiency and secures sensitive data).
  - **Extract Filters**: Limits the data to be pulled into your extract but demands careful application as reversing it is a meticulous task.
  - **Data Aggregation**
    - Aggregating visible dimensions can enhance performance but needs meticulous application to prevent affecting calculations adversely.
    - Aggregation is suggested after the dashboard is fully developed and optimized.

- **Customization of Data Extraction**
  - **Row Specifications**: Options to pull all rows or a specified number of rows are available, along with incremental extracts that only add new records based on a specific field.
  - **Testing Phase**: In initial phases, top or sample functions are useful to work with a specific sample of a large dataset for visualization trials.

Towards the end of this module, there's a mention of saving the work in Tableau Desktop which hints at the topic to be covered in the following sessions.

### Opening & Saving Workbooks

Handling work files in both Tableau Public and Tableau desktop applications requires different approaches:

**Tableau Public:**
- **File Menu**: Found at the top left, facilitates the opening and saving of projects.
- **Open an Existing File Locally**: Requires the workbook to be a stored Tableau public online version first before it is saved to your local desktop.
- **Open from Public/Save to Public/Save to Public as**: Requires Tableau public profile. You will be prompted to log in to choose or save workbooks directly from/to your profile.
- **Profile Creation**: Essential for saving and downloading your work. The sign-up option is at the top right corner where you input recognizable name, email (not necessarily work email), and agree to the terms.
- **Profile Overview**:
  - **Visualizations**: Can be listed or hidden based on your preference. 
  - **Followers and Following**: View people you follow and those following you.
  - **Favorites**: Enables you to reference and download visualizations you find compelling.
  - **Settings**: Allows editing profile settings including hiding content and disabling the download option for others.
- **Saving Work to Your Profile**: Navigate to 'File' and choose 'Save as' for safety. It can overwrite existing visualization or save as a new file.
- **Opening Work from Tableau Public**: Through 'File' and 'Open from Tableau Public', you can access and open any dashboard available in your profile.
- **Sharing and Downloading**: Workbooks saved to Tableau Public server can be downloaded and shared offline.
   
**Tableau Desktop:**
- **File Types**:
  - **WBKZ**: Robust file type that is predominantly used and available in Tableau Public.
  - **WBS**: Holds sheets, dashboards, and stories without data attached.
  - **TWB**: Similar to WBS but carries raw data in Tableau Hyper files. Preferred for sharing as it contains the data.
- **Export as Other Versions**: Useful for sharing files with users operating different versions of Tableau software.
- **Opening Localized Workbook**: Can be done directly without the need for saving it to Tableau Public first.

_Remember to set up a Tableau public profile for a smooth and effective management of your files during the course. Use the save as option for safer saving, and leverage the different file types based on your data sharing preferences in the full Tableau desktop application._

## Sorting, Filtering & Grouping

### The Sheet Interface

In the Sorting Grouping and Filtering section of the Tableau Desktop online course, students will delve into using Tableau's tools to manage and enhance data for analytics. The section is divided into three parts, where students will learn:

- **Data and Field Types**: Understanding the core of analytics in Tableau, which includes an in-depth exploration of the differences between dimensions, measures, and the discrete and continuous fields.
- **Data Organization and Combination**: This includes handling "dirty data," and utilizing Tableau tools such as sorting, grouping sets, and hierarchies to refine raw data for deeper analysis and visualizations.
- **Dynamic Filtering**: Students will learn to unveil hidden patterns in data through dynamic filtering in Tableau Desktop.

Following the overview, the course guides students in navigating the sheet interface, the main workspace in Tableau Desktop, highlighting:

- **Data Division**: Distinguishing between dimensions (qualitative and descriptive) and measures (quantitative and can be aggregated).
- **Marks Card**: Customizing visualizations using different features including color, size, and labels to create dynamic and intuitive representations.
- **Filter Shelf and Pages Shelf**: These tools help in filtering data and trending data over time, respectively.
- **View/Canvas**: The central space where visualizations are created and viewed.
- **"Show Me" Feature**: A tool that suggests visual ideas based on the selected fields, aiding in the initial stages of analytics.
- **Quick Access Toolbar**: Positioned at the top for easy access to frequently used actions.
- **Lower Toolbar**: Helps in adding new elements like sheets and dashboards quickly, and navigating to the data source menu.

Towards the end of this section, there is a detailed walkthrough of how fields interact during visualization creation, including the application of filters and crafting of custom calculations. This foundational knowledge equips students to start creating detailed and dynamic visualizations using Tableau Desktop.

### Dimensions & Measures (Discrete vs. Continuous)

In this lesson on Tableau Desktop online course, you were introduced to key concepts central to using Tableau effectively:

- **Dimensions and Measures**: 
  - **Dimensions**: Qualitative fields used to categorize, segment, or filter data, such as names, IDs, geographic fields, dates, and times. They answer "who," "what," "where," and "when."
  - **Measures**: Quantitative fields representing numerical data that can be counted or aggregated, like sales, profit ratios, percentages, and quantities. They answer "how much."
  - **Manipulating Dimensions and Measures**: These can be interchangeable depending on what you want to showcase in your data visualization. For instance, you can drag a dimension to measures and vice versa, to alter how they represent data. Tableau can automatically apply suitable aggregations when changed.
    
- **Sheet Interface**: 
  - **Exploration**: You explored the representation of dimensions and measures in the sheet interface, including seeing how the same data field can behave differently depending on whether it is treated as a dimension or a measure.
  - **Field Type Reaction**: It was shown that fields react differently in the view when dragged based on their type, and how this can be manipulated to suit your visualization needs.
    
- **Discrete and Continuous Fields**:
  - **Discrete Fields**: Represent a finite set of distinct values, often used to "bucket" your data, e.g., separating sales data by year or category.
  - **Continuous Fields**: Contain an infinite range of values and often resemble measures, representing data points like age, temperature, and sales.
  - **Interchangeability and Exceptions**: While dimensions tend to be discrete and measures tend to be continuous, there are exceptions. Understanding the nuances of when to use each type, and how they can be interchanged, allows for more precise data visualization. 

During the practical portion, you were encouraged to explore the functionalities of dimensions and measures and how they interact with discrete and continuous fields in the Tableau desktop, including manipulating data fields and observing how they behave when changed between dimensions and measures, and between discrete and continuous settings. This is to prepare you for the following sessions where you will delve deeper into these concepts.

### Sorting Data

In this Tableau Desktop online course, the focus is on the different methods you can use to sort your data, aiding in the swift identification of patterns and key insights in your visualizations. Here are the different sorting options available in Tableau:

- **Axis Sort**
  - **Usage**: The simplest and most frequently utilized method where you select a continuous axis to automatically sort the data either in ascending, descending, or according to the data source order.
- **Toolbar Sort**
  - **Quick Access Toolbar**: Houses common sorting options including ascending and descending orders.
- **Sort Menu**
  - **Access**: Click on the "carrot" on the right side of your dimension pill to open the robust sort menu.
  - **Features**:
    - **Sort by Different Fields**: Allows sorting by any field in your data source, including those not visible in your view, offering more flexibility compared to axis or toolbar sort.
    - **Custom Calculation**: Enables sorting based on custom calculations created by you.
    - **Sort Order and Field Name**: Define what you are sorting by and determine the sorting order.
    - **Aggregation Type**: Choose different types of aggregations for sorting, not confined to the one used in the view, providing a more tailored sorting option.
    
Next, you are encouraged to explore these sorting options practically in Tableau Desktop to understand better how each method works and identify the one that suits your needs best for different situations. It underlines that understanding and utilizing the various sorting options effectively can be a pivotal skill in creating insightful visualizations.

### Grouping Data

In this Tableau Desktop online course, the session covers the essentials of grouping data to enhance your visualizations. Here is the breakdown of the relevant points:

- **Objective**: Grouping aims to unite related members within a specific field, typically dimension fields, into buckets which can be customized further.
  
- **Applications**:
  - **Rolling up data to a different detail level**: Allows the grouping of product names into categories or subcategories even when hierarchical data isn't available.
  - **Correcting data inconsistencies**: Helpful in cleaning data and resolving inconsistencies arising from user inputs, promoting uniformity in dashboards.
  - **Creating "what if" scenarios**: Facilitates ad hoc grouping to analyze different scenarios without back-end data alterations.
    
- **Creating Groups**:
  - **Standard Field Grouping**:
    - **Process**: Right-click on a dimension to create a group through the dialog box, where groups can be named and maintained.
    - **Nature**: Groups are static, requiring manual updating to include new records.
      
  - **Regrouping**:
    - **Process**: An easier method where two or more dimensions are selected and grouped using the group members icon resembling a paperclip, bypassing the renaming step initially.
    - **Customization**: The group name can be changed later to something more descriptive.
      
- **Practical Application**:
  - **View Grouping**: Demonstrated using subcategories on an axis to group closely related items like "paper" and "labels" into one.
  - **Modifications**: Following the creation of a group, it is advised to revisit sorting options and labels to maintain the visualization's readability.
    
- **Upcoming Session**: The subsequent section will delve into the topic of "sets" to distinguish them from groups.

Get hands-on practice in the Tableau Desktop interface, focusing on creating and modifying groups effectively to improve your dashboard designs.

### Creating Sets

- This section introduces **sets** in Tableau Desktop, emphasizing their role in defining subsets of data based on certain conditions.
  
- **Types of sets**:
  - **Constant sets**: Remain unchanged unless modified by the user; created from fields or views.
  - **Computed sets**: Dynamically change according to specified conditions and thresholds; can be adjusted with set actions (detailed in the advanced course).
    
- **Creating sets**:
  - **From the field**: Right-click a dimension and choose "create set".
  - **From the view**: Select desired dimensions, open the command menu, and opt to create a set next to the group icon.
    
- **Deep dive into constant and computed sets**:
  - **Constant sets**: Found in the 'General' tab during creation, these sets house chosen dimension values which only change if altered by the user.
  - **Computed sets**: Governed by rules under 'condition' or 'top' tabs; can be constructed using guided setups or conditional formulas, allowing flexibility in defining the set’s scope based on criteria like sales thresholds or top-performing entities.
    
- **Differences between groups and sets**:
  - Groups help in defining specific categories while sets are about distinguishing dimensions that either meet or do not meet the predetermined conditions, offering a binary “in or out” classification.
    
- The section ends with a teaser that encourages the learner to proceed to the hands-on demonstration in Tableau Desktop for practical understanding and application of creating sets.

### Defining Hierarchies

- Understanding custom hierarchies in Tableau Desktop:
  - Hierarchies allow users to define custom levels of detail and drill-down functionalities.
  - Existing automatically for date fields, enabling various levels of aggregation.
  - Users can create hierarchies independent of the data source.
  
- Creating a custom hierarchy:
  - Drag fields over one another in the correct order to create a hierarchy.
  - For instance, to create a hierarchy with “Category” and “Subcategory”, drag the “Subcategory Group” field over “Category”.
  - A hierarchy symbol with a dropdown appears, showcasing the hierarchy levels.

- Utilizing hierarchies in views:
  - Dragging an element of the hierarchy into the view enables drilling up or down at any time by clicking plus or minus signs.
  - It facilitates a high-level initial view with easy drill-down options for detailed data.

- Live demonstration in Tableau Desktop:
  - Creation of a “Product” hierarchy with “Category” and “Subcategory” as levels.
  - Renaming and reordering of levels is possible post-creation.

- Visualizing hierarchies:
  - Add the top level of the hierarchy to the column shelf for visualization.
  - To replace fields in visualization, drag the new field over the existing one until a black outline appears.
  - Hierarchies allow multi-level drill-down through plus and minus system, offering a flexible tool for users.

- Modifying hierarchies:
  - Easy addition and removal of fields in a hierarchy to suit visualization needs.
  - Mistakes, like adding the wrong field to a hierarchy, can be corrected easily by dragging and dropping the correct fields.

- Sorting in hierarchies:
  - The latest Tableau version supports automatic nested sorting.
  - Sorting preferences apply globally to all hierarchy levels, with options for more complex actions to be covered later in the course.

*Note:* Remember that all items in a hierarchy expand fully when using the plus sign, and further actions for selective expansion will be discussed later in the course. The tutorial seamlessly leads to the next section on Tableau Order of Operations to delve deeper into organization, filtering, and sorting data.

### The Tableau Order of Operations

- **Tableau Order of Operations**: 
  - Governs the sequence of computations, actions, filters, and view renderings in Tableau Desktop and Tableau Server.
  - Provides structure to operations running behind the scenes in Tableau.
  - Needs to be read from top to bottom in the diagram, depicting the sequence of processes happening.
  - While every function in Tableau adheres to an order of operations, the focus here is on the most pertinent ones, including:
    - **Primary filters (dark gray in the diagram)**:
      - Data source filters
      - Context filters
      - Dimension filters
      - Measure filters
      - Table calc filters
    - Note that "X filters" are applied first, followed by others in the mentioned order.
  - **Not covered in this section**:
    - Certain layered functions between the main filtering functions.
    - Extract filters: Already discussed in the "connecting to data" section; these are topmost, applied first, and require revisiting the data source pane for alterations.

### Data Source Filters

- **Data Source Filters in Tableau**:
  - **Definition and Importance**:
    - High-level filters applied in Tableau.
    - Can be modified while working on the dashboard.
    - Any sheet created from a filtered data source will inherit those filters.
    - Positioned under extract filters but above other types like context, dimension, and measure filters in the order of operations diagram.
      
  - **Application**:
    
    - **From Data Source Page**:
      - Find and click the 'Add' button in the filter section on the top right corner.
      - Choose to add filters on dimensions or measures.
      - Impacts all sheets connected to the data source.
        
    - **From Sheet**:
      - Right-click data source under data pane and choose ‘Edit Data Source Filters’ to add new filters.
        
  - **Adding Filters to a Project**:
    - Can be added from any page as they affect the data source, not individual sheets.
    - Involves selecting fields and setting criteria for the filter (e.g., a specific date range).
    - Special options available for date filters, including relative and range date filters.
      
  - **Considerations**:
    - Date filters should be dynamic to accommodate ongoing analysis and avoid data loss with time changes.
    - Current example focuses on the years 2017 and 2018 to simplify the data set for the tutorial.
      
  - **Impact**:
    - Changes in data source filters affect all related sheets, altering the results of analyses.
    - Great tool for enhancing dashboard efficiency by reducing data volume, without altering the original data source.
    - However, balance needed to maintain dashboard functionality and a good end-user experience.

*Note*: You should be aware of how these filters can change the analysis results and leverage them strategically to optimize performance without compromising the dashboard’s functionality.

### The Filter Shelf

- **Understanding the Filter Shelf in Tableau**
  - **Definition and Function**:
    - A space in Tableau Desktop showing all filters applied to each sheet, excluding data source and extract filters.
    - Utilized to track filters applied in a view.
  - **Adding Filters to the Shelf**:
    - **Right-click Method**:
      - Right-click on a dimension or measure and select "show filter".
      - Also shows a filter menu on the sheet’s right side.
    - **Drag and Drop**:
      - Drag a dimension or measure directly to the filter shelf.
      - Brings up a filter menu without showing the extra filter box on the sheet’s right side.
    - **Viz Filtering**:
      - Useful for ad hoc analysis and for dashboard users during analysis.
      - Involves selecting dimensions in the view and using commands "keep only" or "exclude".
      - Results in a pill appearing on the filter shelf.
  - **Considerations and Tips**:
    - **Calculated Fields**:
      - Can be used to apply filtering conditions affecting only the associated pill.
      - Involve logical statements in fields that limit or restrict displayed values.
      - To be discussed more in a future section.
    - **Troubleshooting**:
      - If displayed values seem incorrect, check for hidden filters in calculated fields or at data source/extract levels.
      - Understanding of filtering processes is essential for both developers and users to avoid misunderstandings and errors.
      - Comparisons should consider different filtering applied in different sources to avoid “apples to oranges” situations.
    - **Next Steps**:
      - The discussion to be followed by a hands-on session of applying filters in a dashboard.

*Note*: In essence, the filter shelf is central in Tableau for managing and visualizing the different filters applied to a specific analysis, serving as a tool for developers to maintain accuracy and streamline analysis processes. It is advised to always cross-verify any calculated fields and be well-acquainted with the filter order operations to manage data efficiently and accurately.

### Dimension Filters & Card Modes

- **Understanding Dimension Filters in Tableau**
  - **Overview**
    - Dimension filters are primarily used to filter categorical data.
    - Constitutes 75-90% of filters utilized in dashboard creation.
    - Focus on selecting specific categories to filter data.
  - **Relation to Other Filters**
    - Positioned before context filters in the order of operations; context filters are essentially elevated dimension filters.
    - An understanding of dimension filters is prerequisite to learning about context filters.
  - **Types and Applications**
    - **General Dimension Filters**
      - Manually select what to filter.
      - Commonly used and already applied in previous section about the filter shelf.
    - **Conditional Logic Applications**
      - **Wildcard**:
        - Allows filtering based on specific pattern types.
        - Useful for searching specific texts in large categories.
      - **Conditions**:
        - Enables the application of specific logic to narrow down data.
        - Can be executed through the filter menu or a custom conditional formula.
      - **Top Functions**:
        - Variations on condition functions, optimized for end users to choose either a top or bottom function.
        - Involves selecting measures that facilitate the top function.
  - **What to Expect Next**
    - Detailed discussion on the application of dimension filters in future sections.
    - Assurance of covering context filters in upcoming parts.

*Note*: Dimension filters hold substantial importance in Tableau for segmenting categorical data effectively. These filters are versatile, offering general and condition-based filtering, including wildcard and top function utilities to enhance the depth of analysis. Understanding them is foundational to grasping context filters that will be covered later in the course, offering a comprehensive grasp of Tableau's filtering functionalities.

### Filter Customization Options

- **Dimension Filter Customization in Tableau**
    - **Introduction**
        - Tableau offers extensive customization options for dimension filters concerning appearance, functionality, and filter relativity.
    - **Key Features and Tips**
        - **Edit Filter**
            - Accessed through the dimension filter card.
            - Allows for altering filter parameters.
        - **Formatting**
            - Adjust font, color, and border.
            - Option to show, hide, or modify filter titles.
            - Utilize text boxes to overcome title wrapping issues.
        - **Relevant Values**
            - Two main options: “all values in the database” and “only relevant values.”
            - “Only relevant values”: Displays values in line with other applied filters, enhancing user convenience but possibly affecting dashboard performance.
            - “All values in the database”: Shows all distinct field values within the filter.
            - Note: adding context filters introduces a third option, “only values in context.”
        - **Include/Exclude Options**
            - Default is “include,” selecting values to retain in the view.
            - Use “exclude” carefully; indicates values to be omitted from the view.
        - **Additional Settings**
            - “Include values when empty”: Displays null or empty records, useful for data validation and addressing data gaps.
            - “Hide card”: Maintains the filter without displaying it to the end users.
    - **Future Discussions**
        - Detailed exploration of formatting options and context filters in upcoming sections.

_Note_: The session unpacks the variety of customization options available in Tableau Desktop for dimension filters, touching upon essential functionalities such as editing, formatting, and setting relevant values. It cautions new users on potential pitfalls like dashboard performance issues with using “only relevant values” and advises prudence with the “exclude” function to prevent misinterpretations. It also hints at further details on context filters to be covered in subsequent sessions, promising a rounded understanding of Tableau’s filtering options.

### Context Filters

- **Understanding Context Filters in Tableau**
  - **Introduction**
    - Context filters allow for altering the regular order of operations in Tableau, giving priority to certain filters over others.
    - Predominantly used with dimensions; measures and other aggregated fields cannot be used.
  - **Working with Context Filters**
    - **Dependent Top-End Filter**
      - Facilitates creation of top lists in views, resolving conflicts between filters that can affect the displayed numbers.
      - Avoids the scenario where the number of displayed subcategories is less than selected in a top filter due to non-contextual filtering.
    - **Standard Top-End Filter**
      - Normally filters subcategories first, then the city; may not always yield the expected top results for the end user.
    - **Applying Context Filter**
      - Elevating a filter (e.g., city) to the context level allows it to precede other filters, thereby meeting the user’s expectations for top results.
    - **Benefits**
      - Enhances dashboard performance by creating a temporary table that narrows down data based on the selected context filter.
      - Offers more flexibility compared to data source filters as they can be applied at the sheet level.
  - **Practical Demonstration**
    - Showcased using Maven supplies data:
      - Applying a top filter for identifying top five subcategories by sales.
      - Problem encountered when narrowing down to a specific category, resulting in fewer subcategories than expected.
      - Resolved by adding the category filter to context, hence prioritizing it over the subcategory filter.
      - Noted that the number of results might still be less than the top filter value due to the limited applicable data in the chosen category.
  - **Conclusion**
    - Context filters are vital in enhancing filter functionality and dashboard performance.
    - Recommended for top ends and filtering substantial data chunks, but cautioned against excessive usage to prevent performance downturns.
    - Upcoming: Detailed insights into measure filters.

*Note*: The section delves into the advanced utility of context filters in Tableau, spotlighting their role in refining data visualization through a nuanced control of filter operations. Through a practical demonstration using Maven supplies data, it elucidates the problem-solving capability of context filters in achieving desired top-end results, and their efficacy in optimizing dashboard performance by reducing data load. The tutorial steers learners to apply these filters judiciously, balancing the benefits with potential performance impacts. It sets the stage for an upcoming discussion on measure filters, promising to extend the learners’ mastery over Tableau’s filtering options.

### Measure Filters

- **Measure Filters** in Tableau Desktop work exclusively with quantitative data, allowing users to select a range of values within specified boundaries. These filters are applied last in the filter hierarchy, following extracts, datasource filters, context filters, and dimension filters.

- **Setting Up Measure Filters:**
    - **Aggregation:** Users select an aggregation type (e.g., sum, average) while dragging a measure to the filter shelf. Aggregation isn't available for calculated fields with built-in aggregation.
    - **Interface:** Four main types are available:
        - *Range of values:* Users define upper and lower limits.
        - *At least:* Only the lower limit is defined, the upper limit reaches the maximum value of the field.
        - *At most:* Only the upper limit is defined, the lower limit goes to the minimum value of the field.
        - *Special:* Filter null, non-null, or all values.
    
- **Performance Concerns:** 
    - Using too many measure filters can decrease dashboard performance.
    - *Solution:* Use conditional sets instead of measure filters to enhance performance.

- **Measure Filter Card Modes:** 
    - They can be customized to suit developer preferences, offering similar options to the interfaces but presented to the end users.
    - *Advice:* “Range of values” is generally the safest option, offering control over both ends of the range.

- **Application in Practice:** 
    - Users can drag measures like sales to the filter shelf and choose the appropriate aggregation (e.g., Sum) and interface (e.g., range of values) to visualize specific data in a workbook.
    - *Tip:* To reset the filter to its original state, use the clear filter option to show all values and avoid data exclusion.

### Date Filters

- **Date Filters in Tableau**:
    - **Types**: Can be either continuous or discrete.
    - **Distinct Feature**: Relative date function, allowing dynamic filtering based on various time intervals such as days, weeks, months, etc.

- **Relative Date Filters**:
    - **Use**: Dynamically filter data based on different time intervals — highly popular for dashboard filtering.
    - **Complexity**: 
        - The accuracy is influenced by the freshness of the data; stale data can affect the functionality over time.
        - Users can anchor the filter to a specific date, albeit this is not dynamic in the current setting.
    - **Advice**: Ensure data freshness in your source before applying relative date filters.

- **Continuous Date Filter Options**:
    - **Range**: Offers sliders to select minimum and maximum dates.
    - **Starting and Ending**:
        - *Starting*: Lets you pick a start date, while the end point is automatically set.
        - *Ending*: Allows the selection of an end date with an automatic start point.
    - **Special**: Filters special values such as null, non-null, or all dates.
    - **Pro Tip**: Right-click and drag a date field into the filter shelf to choose between discrete or continuous filters before accessing the filter menu; each type has a significantly different menu, hence it is beneficial to make a choice beforehand.

## The Marks Card

### What is a Mark?

- **Marks Card Section in Tableau**:
    - **Definition**: A mark represents any visual element rendered in a user-constructed view in Tableau Desktop, including charts, labels, legends, etc. Any piece of data making visual ink on the screen is a mark.
    - **Quantity and Performance**:
        - More marks require more computational power to render, potentially slowing down Tableau Desktop or Server.
        - It's essential to strike a balance, having enough marks to convey information without hindering performance.

- **Identifying the Number of Marks**:
    - **Location**: Find the mark count at the bottom left-hand corner of the screen when working on a sheet in Tableau Desktop.
    - **Examples**:
        - *Bar Sales by Subcategory Sheet*: 16 marks present, representing 16 bars created from one row supported by 16 columns.
        - *Bars Top Customer Sheet*: Contains 773 marks, equivalent to 773 rows by one column.
        - *Table Sales Versus Goal*: Features 36 marks, derived from multiplying nine rows by four columns.

- **Performance Optimization**:
    - **Issue**: Accumulation of many marks across sheets can slow down the dashboard.
    - **Solution**: Enhance performance by filtering data sources or displaying fewer data pieces simultaneously.
   
- **Upcoming Lesson**:
    - Focus on creating visualizations using marks in Tableau.

### Adding Quick Visuals in Two Ways

- **Creating Visuals in Tableau Desktop**:
    - **Ways to add visuals**:
        - **Show Me gallery**:
            - Common method.
            - Select fields (dimensions/measures) from the left-hand side.
            - Open the "Show Me" visualization menu to see and select visualization options, guided by Tableau's recommendations highlighted in red.
        - **Directly in row or column shelves**:
            - Double click or drag fields into the row or column shelves at the top of the worksheet.
            - Allows quick visual creation and offers flexibility in dashboard building.

    - **Walkthrough**:
        - Opened a new sheet to experiment with creating visuals using both methods.
        - **Using Show Me**:
            - Selected "sales" and "subcategory", opened the Show Me menu, and explored different visualization options including bar charts and tree maps.
        - **Using direct method**:
            - Double-clicked on fields to create visuals and observed how the order of selecting dimensions and measures affects the visualization type (e.g., bar chart or cross tab).
            - Highlighted that one could revert to the Show Me menu or use the Marks card for more control over visualization type.

    - **Organizing Work**:
        - Created an "ad hoc" sheet for temporary work to maintain organization.
        - Emphasized the need for keeping the workflow organized as the course progresses.

### The Marks Card

- **Controlling Mark Types Using the Marks Card**:
    - **Introduction**:
        - Marks card appears like a stack of playing cards.
        - Each card represents a measure that creates an axis in the visualization.
    - **Modifying mark type**:
        - Done using the Marks card dropdown.
        - Default setting: automatic, choosing the best visualization based on several factors including the field types and their positions on rows or columns.
        - Other options: bar, line, area, circle, shape, text maps, pie charts, Gantt bars, density, and more; catering to extensive customization needs.
        - **Automatic setting**:
            - Primarily chooses the visualization based on the innermost field in the rows or columns.
            - E.g., subcategory at the innermost position defaults to a bar chart, whereas having order date at the innermost position generates a line chart.
            - Aligns with standard best practices for data visualization.
    - **Utilizing the Marks card**:
        - Allows changing and customizing the visualization after its creation, enhancing adaptability to individual needs.
    - **Practical Demonstration**:
        - Used the ad hoc sheet in Tableau desktop to create marks.
        - Altered the order date to a discrete month, distinguishing between discrete and continuous fields.
        - **Changing visualizations**:
            - Visualization can shift from a line chart to a bar chart depending on whether a date field or a non-date segment is in the innermost position.
            - Adjusting the order of dimensions can assist in achieving the desired visualization, avoiding frustrations due to Tableau’s default settings.
    - **Conclusion**:
        - Highlighted the role of innermost fields in determining automatic visualization settings.
        - Encouraged experimenting with the arrangement of dimensions for desired outcomes.
        - Future lessons will further explore building core visualizations for dashboards.

### Marks Card Properties (Part 1)

- **Deep Dive on Marks Card Properties**:
  - **Overview**:
    - The Marks card offers control over the context and detail of the marks in the view, including aspects such as color, size, labels, detail level, tooltips, shapes, and lines.
  - **Top Section of Marks Card Properties**:
    - **Color**:
      - Applicable to both measures and dimensions.
      - Allows control over color range, opacity, border lines, and halo effects.
      - The menu changes based on whether a measure or a dimension is dropped on it.
    - **Size**:
      - Generally used for measures, using it for dimensions can be unintuitive.
      - Manipulated through a slider and a size range which can be inverted based on display needs.
      - Tip: Utilize absolute values for negative values to maintain impact magnitude, while using color to indicate positivity or negativity.
    - **Labels**:
      - Can be turned off entirely or customized for different scenarios including highlighting, selection, min/max value, etc.
      - Allows the combination of fields and flat text for dynamic story telling.

### Marks Card Properties (Part 2)

- **Marks Card Property Section (Part 2)**:
  - **Detail**:
    - The detail in a view is determined by the dimensions placed in it, with adding dimensions increasing the granularity and level of detail.
    - Adding dimensions can be done through row shelf, column shelf, or the marks card section.
    - Measures, tooltips, and filter shelf do not affect the level of detail.
  - **Tooltips**:
    - Found in the Marks Card Properties Menu, they are the boxes that appear when you hover over marks in the view.
    - They can display flat text, field values, and entire visualizations.
    - To avoid asterisks appearing in tooltips for dimensions lower than the view's detail level, they should be added to the level of detail section of the marks card or in rows or columns, not just in tooltips.
  - **Shapes**:
    - Shapes can be assigned to different dimension categories and Tableau offers a robust set of standard shapes.
    - Custom shapes can be uploaded into the Tableau repository, with each user having a "My Tableau repository" in the documents folder for this purpose.
    - Custom icons for dashboards can be sourced from various websites offering free assets.

### Stacking Marks

- **Stacking Marks in Tableau**:
  - **Introduction to Stacking Marks**:
    - Located in the analysis menu, it allows you to layer dimensions along a continuous axis.
    - When turned on, it visually sums up values giving an additive total visual representation.
    - Disabling it separates dimensions which are then layered behind each other, and it incorporates transparency to show that the values are not additive but independent.

  - **Practical Application in Tableau Desktop**:
    - **Creating a Stacked View**:
      - Utilized measures like sales and segments along with order date to create a visualization.
      - Adjusted the view to a more dynamic one by expanding the year to quarter.
      - Noted that the visualization might be confusing as it showcases a cumulative value, not an individual segment value.
    - **Unstacking Marks**:
      - Through the analysis menu, the stack marks option can be turned off to unstack the dimensions.
      - Advised to arrange larger values at the back and smaller at the front for better visualization.
      - Emphasized the importance of understanding the visualization to correctly interpret the data being displayed.
    - **Stacking and Unstacking with Different Visualization Types**:
      - Demonstrated that unstacked visuals can be used in various visualization types, including bar charts.
      - Utilized dual axes and other methods to aid in visual representation.

  - **Conclusion**:
    - Highlighted the necessity to understand the pros and cons of stacking and unstacking to effectively use them in data visualization.
    - Mentioned the upcoming topic on utilizing the Pages shelf for dynamic trending.

### The Pages Shelf

In this Tableau Desktop online course module, you learn about the functionalities of the pages shelf and how to use it to create animated visualizations that depict changes over time. Here is a summary of the key points:

- **Pages shelf overview**:
  - Situated at the top left of the workspace.
  - Facilitates the creation of animated, separate, and filtered views/pages showing trends or time-based changes.
  - It accommodates both measures and dimensions, defaulting to discrete fields.
  - Best utilized with date options.

- **Using the pages shelf**:
  - Drag a field to the pages shelf to activate the pages for the current sheet.
  - Configure the playback controls appearing on the right side for manual cycling through options with varying speeds (slow, medium, fast).
  - The history option can be adjusted to display trails of the marked progress, with customization available for type of marks, trails, and formatting.

- **Creating a visualization with pages**:
  - Choose measures and dimensions, opting for sales and quantity alongside the segment under dimensions.
  - Select Scatter Plot as the suggested visualization.
  - Adjust the visualization through the Marks card with segment pills for color variations and sales field controlling the segment size.
  - Apply additional refinements like increasing circle size for better visibility and setting opacity to around 75%.
  - Drag the order date field to the pages shelf and adjust the aggregation level to quarter, enabling year and quarter combination in pages.

- **Fine-tuning your visualization**:
  - Adjust speed settings and enable history to show both marks and trails for better tracking of paths during playback.
  - Customize trail format for better visualization.
  
- **Playback and tracking**:
  - Utilize the play button to animate the visualization and track changes over time.
  - Individual segments can be traced back to their origin by clicking on them, showcasing their paths vividly.

- **Server publication and compatibility**:
  - Full automated playback is available in Tableau Server 2021 and later versions.
  - Manual cycling through pages is possible in earlier versions.

- **Application in presentations**:
  - Pages are effective in creating quadrant analyses and date trending views, helping to narrate a dynamic story in presentation settings.
  - Though not used in the main dashboard in this course, pages are a potent tool for daily analytical work. 

Remember to practice using this feature to enhance your Tableau Desktop skill set.

### The Analytics Pane

The segment discusses the functionalities of the analytics pane in Tableau Desktop. Here's your summarized content:

- **Analytics Pane in Tableau Desktop**
    - **Key Functions**
        - Drag-and-drop analytics tools (e.g., reference lines, totals, forecasts).
        - No need for manual calculations; drag elements directly into the view.

    - **Usage Tips**
        - Some tools may be unavailable depending on the data view configuration.
        - Three application levels for analytics tools:
            - Table level: applies across all panes ignoring the vertical or horizontal lines.
            - Pane level: analytics will be split based on the number of panes present.
            - Cell level: applies analytics to every cell reference; less commonly used but useful in specific scenarios.

    - **Demonstration**
        - Cleared the initial sheet to start a new visualization, creating a line chart using sales and order date details.
        - The analytics pane is accessible behind the data pane.
        - The pane presents various options with some potentially grayed out based on the current data configuration.
    
    - **Application of Tools**
        - **Forecast tool**
            - Drag it to view to predict trends based on existing data; limited in robustness.
        - **Constant Line**
            - A static reference line applied to chosen measures; it doesn't change with the view.
        - **Average Line**
            - Can apply at table, pane, and cell levels, each offering a different perspective of the data.
            - Cell level: least useful for individual data points but can be handy for other visualization types.
    
    - **Customization**
        - Lines can be edited to change scope, aggregation type, label, and tooltip.
        - Can alter line style and add fills above or below the line for clarity.

- **Wrap Up**
    - The analytics pane offers a way to enhance analytics visually.
    - Advanced details to be covered in a future advanced topics course.

Note: Make sure to explore different options in the analytics pane to utilize its full potential and enhance your Tableau Desktop analytics visually.

### PRO TIP: Getting the Viz You Want

Creating the desired visualization in Tableau involves both science and art. Here, we outline a four-step process to aid in quickly attaining the visuals you aim for:

- **Step 1: Use 'Show Me'**
   - The simplest and most straightforward method to initiate your visual creation.
   - Select the appropriate dimensions and visuals to automatically generate a chart.
   
- **Step 2: Adjust Field Types**
   - If 'Show Me' fails to produce the needed visual, the next step is to explore altering the field types.
   - A change in field types can potentially impact the visualization significantly.

- **Step 3: Modify Field Properties**
   - Switching between discrete and continuous options in field properties might help in getting the right visual.
   - The visual outcome can vary greatly based on the fields being adjusted and their positions in the visualization.

- **Step 4: Alter Mark Properties**
   - As a last resort, tweaking mark properties might be necessary to achieve the desired visual.
   - It might be essential to utilize all the above steps iteratively to reach the final visualization.

Next, the discussion transitions into a practical demonstration in Tableau Desktop where these steps are utilized to create a visualization, starting by clearing the current analytics pane example through the 'clear sheet' option. This walkthrough aims to illustrate the efficient use of the four-step process in building the necessary visualization, including techniques to craft visuals that are not readily available in Tableau.

## Calculated Fields, Table Calcs & Parameters

### Calculated Fields

In this part of the Tableau Desktop online course, you will delve deeper into the concept of calculated fields which assist in more sophisticated data analysis. Here are the main topics that will be covered:

- **Introduction to Calculated Fields**
  - Facilitates creating new columns not present in your original data source.
  - Useful for data segmentation, type conversion, aggregation, filtering, and computing new metrics.

- **Types of Calculated Fields**
  - **Basic Calculations**
    - Handles regular calculation needs similar to functions in Excel, including simple aggregation and filtering.
    - Has some unique aggregation applications and different syntaxes but largely familiar to most analysts.
   
  - **Level of Detail (LoD) Expressions**
    - Allows control over the calculation's level of detail, bypassing the restriction of view level dimensions.
    - Considered advanced and will be discussed further in a separate advanced course.

  - **Table Calculations**
    - Calculations are done directly in your Tableau Desktop view and not reverted back to the data source, offering flexibility in analytics.
    - Allows on-the-fly calculations without affecting the original data source.

- **Utilization of Calculated Fields in Visualizations**
  - Operates similarly to regular data source fields in building visualizations.
  - Differentiated from regular fields by an equal sign next to the field symbol.

This section aims to equip you with the knowledge to enhance your analytics through the proficient use of calculated fields, with detailed guidance provided every step of the way, despite the expected increase in technicality and the mathematical approach involved.

### PRO TIP: Selecting a Calculation Type

In this part of the Tableau Desktop online course, a decision tree is introduced to help choose the appropriate type of calculation for different analyses. The primary steps and considerations in this decision-making process are:

- **Determining the Need for Table Calculations**
  - Consider if your question requires ranking, recursion, moving, or intro calculations, which are often necessary for creating table calculations. 
  - If your visualization contains all the necessary data for your analysis, table calculations can still be a viable option for simple tasks like running totals and basic math.
  
- **Analyzing Granularity**
  - Assess whether the granularity of your data matches the granularity required for your question. 
  - If your current granularity is sufficient, basic calculations can be employed to conduct most analytics.
  
- **Utilizing Level of Detail (LoD) Expressions**
  - In cases where your data's granularity does not suit your analysis needs, LoD expressions come into play to allow adjustments in the granularity to perform the necessary analytics.

- **Flexibility in Choosing Calculations**
  - It is highlighted that different types of calculations might be used interchangeably in some scenarios, leaving room for personal preference based on comfort and trust in a particular method.

By systematically following this decision tree, you will be equipped to make informed decisions on the calculation type best suited for your analytics needs, although it may initially seem complex. It is stressed that, ultimately, the choice of calculation type can boil down to personal preference, and you are encouraged to choose what you find most comfortable and reliable.

### Calculation Syntax

In this part of the Tableau Desktop online course, the anatomy of creating calculations with different components in Tableau is dissected using an example. Here are the critical parts and their roles:

- **Comments**
  - Initiated using a double backslash.
  - Turn light gray to indicate inactive text.
  - Useful for documentation or noting test variations.
  - Maintaining clarity and consistency in comments is advised.

- **Calculation Name**
  - In the example: "sales/profit multi."
  - The setup allows users to select either sales or profit to display in a chart through a parameter dropdown box, facilitating a dynamic field in the dashboard.

- **Parameters (Purple Text)**
  - Dynamic fields significantly impacting calculations, filters, etc.
  - Can be populated from various sources and drive different functionalities in Tableau.
  - Need to work in conjunction with other elements to be functional.

- **Operators (Black Text)**
  - Represent mathematical or logical symbols utilized in various programs, including Excel.
  - Utilized in mathematical and logical functions.

- **Literal Expressions**
  - Constant values, like numbers or dates, hardcoded into your calculations.
  - Requires careful use to maintain the intended function over time.

- **Fields (Orange Text with Square Brackets)**
  - Refer to either raw or calculated columns used for dimensional or aggregated values.
  - Can undergo different types of aggregations derived from functions.

- **Functions (Blue Text)**
  - Represent actions performed on fields, literal expressions, and operators.
  - They encompass various calculation functions, including numeric, string type, date logic, etc.

Having familiarized with the essential components and their visual representations in Tableau's calculation syntax, the following lessons will delve deeper into creating a calculated field to foster hands-on experience in crafting your analytic fields. This segment ensures a foundational understanding before moving onto practical application.

### Creating Calculated Fields

In this section of the Tableau Desktop online course, you'll learn how to create and use calculated fields, a fundamental skill in building dynamic and intricate dashboards. Here are the key takeaways:

- **Creating calculated fields:**
  - **From an existing field**: Right-click a dimension or measure and select 'create calculated field' to open the dialogue box, where the chosen field will automatically appear. You can also initiate this process from a white space, but you'll need to manually add fields.
  - **Directly in your view**: You can quickly generate temporary calculations in rows, columns, or the marks card by double-clicking and typing out your calculation. To save them for future use, drag them into the dimensions or measures section. 

- **Working with calculations:**
  - **Naming**: After typing your calculation, name it appropriately for easy identification.
  - **Adding fields to the calculation window**: Either drag fields from the dimensions or measures section into the window or start typing to find and add them.
  - **Building a calculation**: For instance, to create a profit percent calculation, you would divide the profit field by the sales field. It's advised to use aggregation wrapping to allow the field to adapt to different levels in your view.

- **Using calculated fields:**
  - **Aggregation**: Understand the role of aggregation in calculated fields, especially how it influences the calculation depending on the view's detail level. More on this will be covered in the next sections.
  - **Nesting calculations**: You can incorporate existing calculated fields into new ones to develop intricate analyses. For instance, modifying the profit percent field to display as a full percentage value for better user understanding.
  - **Saving and reusing**: After creating a calculation in your view, drag it into the dimensions or measures area to save and rename it for future utilization.

Stay tuned for deeper insights into aggregation and its role in calculations in upcoming sections. Note that this tutorial is directed towards crafting efficient and detailed dashboards by harnessing the full potential of calculated fields in Tableau Desktop.

### Aggregation Types

- **Aggregation in Tableau**
  - Definition: Combining or summarizing data into a single value to represent the data succinctly.
  - Applicable to both dimensions and measures but using different methods.
  - Influenced by:
    - The dimensions in the view
    - The type of calculation used
  - Helps in making analytics clean and accurate.

- **Aggregating Measures**
  - Commonly used functions: sum, average, median, max, etc.
  - Default aggregation for sales: sum
  - Tableau aggregates data dynamically based on what is inside your view.

- **Aggregating Dimensions**
  - Does not happen by default.
  - Uses terms like min, max, count, and count distinct for alphanumeric sorting.
  - Methods:
    - Dragging the field with a right click to access aggregation options from the start.
    - Changing a field to a measure after bringing it into the view via right-click menu.
  - Considerations: Be aware of the data you bring in, as it affects the calculation place.

- **Adjusting Default Aggregation**
  - Some fields may require different default settings.
  - Set default aggregation through the default properties menu in the data field.
  - Benefits: Avoid repetitive adjustments across different sheets.

- **Turning Aggregation Off**
  - Unchecking the "Aggregate Measures" option under the analysis dropdown leads to a disaggregated view, showcasing individual data points.
  - Applicability: Allows visualization of data distribution at the order level and analyzing individual orders.
  - Tips:
    - Utilize index function to spread out data points in a disaggregated view.
    - Remember to re-enable aggregation to avoid confusion in regular views.
  
- **Upcoming Topic**
  - Exploration of how aggregation functions inside calculated fields.

Remember to always refer to actual examples and practice in your Tableau desktop to get a hands-on understanding. Adjust the aggregation settings as per your data and visualization needs.

### Aggregation Types (Part 2)

In this section, the tutorial discusses the different types of aggregations that can be used in Tableau Desktop while creating calculated fields. Here are the main points covered:

- **Types of Aggregations**
  - **Row-level Aggregation**
    - It operates at the lowest grain of the data.
    - Tableau assumes this type of aggregation if none is specified in your calculated field.
  - **Dynamic Aggregation**
    - This type involves wrapping each part of your calculation with an aggregation.
    - Automatically aggregates to the level of whatever is brought into the view.
  - **User-Defined Aggregation**
    - Utilizes level of detail (LOD) calculations to include, exclude, or fix certain dimensions during the calculation process, independent of how the view is constructed.
    - They are highly useful for solving various problems once you are comfortable with the logic applied.

- **Common Issues and Tips**
  - Mixing aggregated and non-aggregated fields in the same calculation will result in an error.
  - To avoid errors, maintain consistent aggregation levels throughout your calculation.
  - It is essential to understand the kind of aggregation required based on the context to get the accurate results.

- **Hands-On Demonstration**
  - **Creating a Row-Level Aggregation**
    - Created a calculated field with a formula for "profit percent row level".
    - Demonstrated the issue with sum aggregation, showing an incorrect result.
    - Adjusting the aggregation to average yielded a more logical result, but it raised questions about the exactness of the approach.
  - **Creating a Dynamic Aggregation**
    - Created a new calculated field named "profit percent dynamic aggregation".
    - Illustrated the error encountered when only one part of the formula is aggregated, emphasizing the necessity to aggregate both parts.
    - Showed that using sum on both sides of the formula gives the true profit percent for the entire dataset, which differed slightly from the average obtained in row-level aggregation.

- **Understanding Output Differences**
  - The output changes based on where the aggregation is applied – inside or outside the calculated field.
  - The prefix “agg” indicates that aggregation is already done inside the calculated field, and further aggregation is not permitted, with a few exceptions in the case of LOD calculations.

- **Conclusion**
  - The section clarifies the fundamental concept of aggregation in Tableau and sets the ground for discussing common calculation functions in the next part of the course.

This summary is streamlined for incorporation into your Obsidian notes, removing the introductions and conclusions to focus on the substantial content of the tutorial.

### Common Calculation Functions

In this part of the course, the focus is on the common calculation functions used in Tableau Desktop. Here is a concise summary of the primary concepts discussed:

- **Aggregate Functions**: Central to calculation functions you'll use in Tableau. They summarize or alter the data granularity. Examples include SUM, AVG, MIN, MAX, etc., and Level of Detail (LoD) expressions, which are not bound by the view's granularity.
  
- **String Functions**: Useful for manipulating text-based data, resembling functionalities found in Excel. They permit operations such as changing text case, finding string length, and using regular expressions to conduct advanced features without needing external help.

- **Logical Calculations**: Familiar to Excel users, these functions help in determining the truth value of conditional statements. They can be blended with aggregate and string calculations to create dynamic fields.

- **Date and Time Calculations**: These functions are used to alter date fields by breaking them down, creating new ones or modifying existing ones to enhance the analysis by utilizing various aspects packed in date fields.

- **Type Conversions**: Changing a field from one type to another is facilitated through this function, and it is essential when working with multiple non-conformed data sources.

The discussion transitions into a practical session on how to access and use these functions in the Tableau Desktop, emphasizing the calculated field dialog box where users can explore different calculation function types and preview the construction of various calculations, serving as a vital tool for both beginners and experienced users. The upcoming section promises a deep dive into each calculation section starting with aggregates.

### Common Aggregate Functions

- **Core aggregate functions in Tableau Desktop** are essential in performing complex calculations.
  - **Sum function**: 
    - Default function for every measure brought into Tableau.
    - Returns the sum of all numeric values in an expression (ignores nulls).
    - Usage: wrap the field with `SUM()` function.
  - **Average function**:
    - Returns the average of all numeric values in an expression (ignores nulls).
    - Adjusts according to the level of detail in your view.
    - Usage: wrap the field with `AVG()` function.
  - **Max function**:
    - Returns the highest value across all records.
    - Useful for finding the ceiling of your data or isolating specific values.
    - Can work with both measures and dimensions.
  - **Min function**:
    - Returns the lowest value across all records.
    - Similar uses as the Max function but finds the floor of your data instead.
  - **Count function**:
    - Returns the number of items in a group (ignores nulls).
    - Includes duplicates.
    - For a distinct count, use the Count D function (`COUNTD()`), which returns the number of unique items in a group.

- **Creating basic aggregation calculations**:
  - **Creating average sales**:
    - Create a calculated field and wrap the sales field with `AVG()` function.
    - You can further split the data by bringing in another dimension like "segment" for comparative analysis.
  - **Aggregating discrete dimensions**:
    - Perform counts on discrete dimensions like "order ID".
    - Create different calculated fields for count and distinct count to understand the granularity of your data.

**Note**: The foundational knowledge of these basic functions is vital for working efficiently with Tableau Desktop, and understanding the differences between them can aid in detailed analysis. Next, the course will cover string functions.

### String Functions

- In this Tableau Desktop course segment, several critical string functions are explained. Here are the main points:
  
  - **Contains function**: Helps identify if a specific text is found in a field. It is particularly useful when working with messy datasets and can be paired with other logical and numerical functions.
    
  - **Length function (LCN)**: Determines the number of characters in a field, assisting in maintaining consistency in fields like order ID.

  - **Replace function**: Allows for the replacement of old text with new text in a specified field, facilitating the update of stale data segments without altering the database directly.

  - **Split function**: Splits a text string based on a delimiter and start position. This function can define the specific parts of the split you wish to take and is comparable to a function seen in Excel.

  - **Trim function**: Cleans up data by removing extra leading or trailing spaces that could distort data displays and aggregation.

  - **Upper and Lower functions**: Convert text to uppercase or lowercase respectively, aiding in data synchronization across various sources.

- Towards the end of the segment, an interactive demonstration is conducted where a calculated field named "purple products" is created using the "contains" function. This field was devised to identify product names containing the word "all", using it successfully to highlight a product in the dataset. The segment emphasizes the practical utility of string functions in enhancing data analyses and visualization in Tableau.

### Logical Functions

In this Tableau Desktop online course segment, the focus is on understanding and utilizing logical functions, which are crucial in evaluating data and creating new measures and dimensions in your dataset. Here are the key points covered:

- **IF statement**:
  - Similar to Excel but without commas.
  - Structure: `IF [logical test] THEN [result if true] ELSE [result if false] END`.
  - Allows for a single logical test, returning results based on the truthiness of the statement.

- **ELSEIF**:
  - An extension of the IF statement to include multiple logical tests sequentially.
  - Helpful to categorize data in different groups based on different conditions.
  - Be mindful of the order of logical tests to avoid errors.

- **CASE statement**:
  - Facilitates the return of different results based on corresponding conditions.
  - Can involve fields or parameters, offering a flexible approach to defining conditions.
  - Suggested to format with `WHEN` and `THEN` pairs on separate lines for readability.

- **Zn function (tsne)**:
  - Converts null values to zero to aid in calculations involving fields with null values.
  - Essential tool when dealing with nulls in numeric calculations, helping to avoid disruptions in aggregations.

- **Applying Logical Functions**:
  - Practical example demonstrated involving the creation of a calculated field named "sales versus goal color" using blended fields.
  - Utilized a Boolean function to compare sales against goal values.
  - Demonstrated how to use this function to apply color formatting to a dashboard for quick insights.

The lesson emphasizes the utility and flexibility of logical functions in Tableau Desktop, encouraging learners to explore and practice using these functions to enhance their dashboards and data analysis. It finishes with a hint at the next segment focusing on date functions.

### Date Functions

In this session, various date functions available in Tableau Desktop were discussed. Here is a summary:

- **Date Functions Overview**
    - **Dynamic Use**: Allows dynamic manipulations for creating visualizations and filters.
    - **Hierarchical Drill-Down**: Enables breaking down dates from years to minutes.
    - **Use Cases**: Useful in comparative year-over-year analysis and other operations involving date fields.

- **Specific Functions**
    - **Day, Week, Month, Year**: Retrieve the respective integer values from a date field.
    - **Today/Now**: Gives the current date or the current date and time respectively.
    - **Date Add**: Adds or subtracts a specified interval from a date field; can work with positive or negative values to adjust dates forward or backward.
    - **Date Diff**: Finds the difference between two dates based on a specified interval without altering the original date fields.
    - **Date Name**: Extracts the string name of the specified part of a date (like the name of a month).
    - **Date Trunc**: Trims the date to a specified level, such as the start of the month or the start of the year.

- **Applications and Combinations**
    - **Dynamic Field**: Can create a field that automatically updates to maintain a rolling time period without needing to apply a new filter.
    - **Delivery Timeline**: Useful in calculating and analyzing delivery timelines by finding the difference between start and end dates.
    - **Year-over-Year Analysis**: Can facilitate dynamic year-over-year analyses using logical statements that incorporate the current year and previous year derived from date functions.

- **Practical Implementation**
    - **Field Creation**: Demonstrated how to create new fields that show current and prior years based on "today's date".
    - **Calculations**: Discussed the use of newly created fields in various calculations, including creating a current year sales field through logical statements involving the ship date and current year data.

The session highlighted the flexibility and numerous possibilities of combining these functions to derive valuable insights from date fields in Tableau Desktop. It encouraged users to experiment with these functions to enhance their data analyses.

### Type Conversion Functions

In this Tableau Desktop online course segment, you learned about type conversion functions which are crucial when working with different data types in your fields:

- Type conversion functions help in changing the data type of your field without altering the underlying data source, facilitating diverse calculations.
- Common type conversion functions include:
  - **Date and DateTime function**: It allows for manipulating date fields, temporarily changing them into date types just for specific calculations, thus avoiding the creation of extra fields.
  - **Float function**: Converts a field to a numeric value with decimals, providing granularity in numerical data.
  - **INT function**: Changes a field to an integer, truncating to the closest integer to zero.
  - **STR function**: It is used to convert fields to strings, often utilized in logical and operator functions.
- Examples of applying type conversion:
  - **Converting to float**: For instance, making a “quantity partial” field to represent fractional quantities, where the float function can be applied to the quantity field.
  - **Converting to string**: Creating a string version of date fields to display them as discrete dimensions, useful in showcasing details to the finest granularity.
- Practical utilization involves wrapping the field with the respective function (like date, float, str) in the calculated field to achieve the desired conversion, simplifying data representation and facilitating specific calculations without cluttering your workbook with duplicate fields.

These functions are elemental in crafting diverse and complex calculations, paving the way to delve deeper into the potent level of detail expressions in upcoming modules. Keep in mind that understanding and utilizing these functions will help in maintaining a clean and efficient workbook.

### Level of Detail (LOD) Expressions

In this lesson, you explored Level of Detail (LoD) expressions, which are advanced calculations that allow users to control the granularity of their analysis in Tableau, overriding the default aggregation level set by the dimensions in your view. Here are the essential details:

- **LoD Expressions Overview**
  - Allow control over the granularity of calculations.
  - Can override default aggregation levels set by dimensions in the view.

- **Types of LoD**
  - **Fixed**: Specifies exact dimensions for the calculations, unaffected by dimensions in the view, except when higher in the order of operations, like context filters.
  - **Include**: Adds a dimension to the declaration while considering other dimensions in the view.
  - **Exclude**: Excludes a specific dimension from the calculation, allowing for higher-level aggregations.
  
- **Creating an LoD Expression**
  - **Syntax**: Consists of LoD type, dimension declaration, and aggregate expression.
  - **Example**: Creating a "sales exclude city" calculation to find the percent of total state sales a city represents.

- **Utilizing LoD in a Dashboard**
  - Created a calculated field "sales exclude city" using an exclude LoD to remove city impact from the sales data.
  - Created a field "city sales percent of state" to find the city’s sales as a percentage of the state's sales using the "sales exclude city" field.
  - **Tooltip Adjustment**: Adjusted tooltip to include the new field and display the city's sales as a percentage of the state's sales, enhancing data presentation on the dashboard.

- **Takeaway**
  - LoD expressions are a powerful tool in Tableau to fine-tune the granularity of your data analysis.
  - It's a crucial skill to leverage in building more dynamic, insightful dashboards.

Next, you will delve deeper into table calculations. Remember, this is a foundational understanding of LoD expressions, and a separate, detailed course on advanced topics is in line to enhance your knowledge further.

### Table Calculations

In this segment, you delve into table calculations in Tableau Desktop, emphasizing their vital role in creating data visualizations. Key details include:

- **Definition and Importance**
    - Table calculations are sheet-specific computations occurring within Tableau, not affecting the original data source. 
    - Operate after all other operations like filtering and defining have been carried out, using the resultant values as a base for their computations.

- **Creating Table Calculations**
    - **Quick Table Calculations**: Accessible from the pill menu, offering common calculation options.
    - **Manual**: Offers more customization by selecting 'add table calculation' from the menu to open a dialog box with different parameters.
    - **Calculated Field**: Allows adding calculations directly in a calculated field, facilitating the insertion of basic table calculations by typing them in.

- **Working with Table Calculations in Tableau**
    - **Example Walkthrough**: You demonstrate creating a line chart and applying different methods to add a running total table calculation to it. 
    - **Visualization**: You elaborate on visualizing the table calculations and how different table calculations can exist in the same sheet.
    - **Adding Table Calculations in Calculated Field**: Involves creating a new calculated field and selecting or typing the required table calculation function, followed by defining the aggregation method.

- **Customization**
    - Note the flexibility in choosing computation methods and restarting options, albeit advising to avoid the default table calculation window for its complexity.

In the upcoming module, you'll explore the different types of table calculations and their application process. This summary provides a concise overview of the introduction to table calculations, setting the stage for deeper learning in subsequent modules.

### Table Calculation Types

In this Tableau Desktop online course segment, the focus was on the deep understanding of various table calculation types, namely:

- **Difference from/Difference from DU**: This helps in calculating the difference between each value and another value relative to it in a table, eliminating the need for creating separate calculated fields for each column. Additionally, it allows calculating percent difference from, giving a different perspective on the impact of change from one value to another.

- **Percent from**: Divides one value by another, providing a different way to analyze increase percentages over a period (e.g., year over year).

- **Percent of total**: A useful calculation that computes a value as a percentage of the total rather than just one reference point. 

- **Rank**: This calculates each value's rank among all values in a table, useful in various business scenarios, and allows different methods to handle ties.

- **Percentile**: It computes the percentile rank of each value in a table, widely used in medical contexts, for instance, to understand a child’s growth percentile.

- **Running total**: Allows viewing running totals for specific periods without creating separate calculations, offering different aggregation methods including average, minimum, and maximum.

- **Moving calculations**: Used to determine a mark’s value by aggregating a specified number of values before or after the current value, frequently utilized in the financial sector to smooth out data trends.

Furthermore, participants learned to apply these calculations in Tableau by creating various visualizations, including line charts and text tables, and manipulating these through options available in the table calculation window. The session encouraged experimenting with these functions to choose the one that suits the users' needs best, with examples illustrating how to apply these calculations in real-world scenarios.

Towards the end, attendees were guided on how to clear, edit, and validate table calculations, with tips on ranking data effectively according to specific use cases. Upcoming sections promise a deeper insight into addressing and partitioning data using table calculations.

### Table Calculation Computation

Here's a streamlined summary optimized for your Obsidian notes app:

- **Table Calculation Compute Options**
  - **Direction of Application**
    - **Table Across**: Affect an entire row in a table or a row within a pane in the table
    - **Pane Across**: Affect a row within a pane
    - **Cell**: Apply to an individual data point
  - **Access**: Found in the main table calculation dialog box and within the application window for table calculations
- **Adjusting Table Calculations**
  - **Process**:
    - Right-click on the relevant pill
    - Navigate to "compute using" option to select the direction of the calculation
  - **Example**: Using "table down" computes from top to bottom in the table, providing a percent of total for each column
- **Real-time Example in Tableau Desktop**
  - **Setup**:
    - Navigate to the ad hoc view with your table calculation
    - Drag out another field into columns to split data (e.g., order date by year)
  - **Adjusting Calculation**:
    - Go to "quick table calculation" menu to change type (e.g., to percent of total)
    - Direction verification: Click in table calculation field, then go to "compute using"
  - **Preview Feature**:
    - Find under "edit table calculation" option
    - Allows you to see how the calculation applies with a yellow highlight indicator
  - **Other Options**:
    - **Pane**: Equivalent to Table when there's only one pane
    - **Cell**: Each cell equals 100%, not generally useful
- **Upcoming**: Deep dive into controlling specific dimensions in "Addressing and Partitioning" section.

Note: This summary was created focusing on the most relevant material, disregarding introductions and conclusions. It includes detailed information on how to set up, adjust, and preview table calculations in Tableau Desktop, preparing learners for a deeper dive into specific dimensions in a future section.

### Addressing & Partitioning

In this Tableau Desktop online course module, the deep dive into table calculations continues, focusing on addressing and partitioning. Here are the key takeaways:

- **Addressing and Partitioning**: Understanding these concepts is essential when working with table calculations.
  - **Addressing Fields**: These are the checked fields in the table calculation dialog box defining the direction of a calculation (across, down, etc.). You can change the calculation direction by reordering these fields.
  - **Partitioning Fields**: The unchecked fields in the dialog which dictate the level or group at which the table calculations stop. They set boundaries in the data, creating a kind of 'brick wall' where calculations will not pass.
- **Specific Dimensions**: This feature in the dialog box allows for more refined control over the table calculations, facilitating very particular applications by designating specific dimensions as addressing or partitioning fields.
- **Visualization and Assistance**: Utilizing the visualization and calculation assistance features in Tableau can aid in understanding how calculations are being applied.
- **Compute Using Options**: Though specific dimensions offer precise control, 90-95% of scenarios can be covered using the ‘compute using’ options, which are simpler to use.

The lecture emphasizes a practical approach where you should actively try various options to see which suits your needs, guiding through changing settings in a hands-on example. Remember to differentiate clearly between your addressing and partitioning fields to manage the direction and stopping points of your calculations effectively. The session ends with an introduction to the upcoming topic, "parameters."

### Basic Parameters

- **Table Calculations**: The lesson discussed how to use and customize table calculations in Tableau Desktop, focusing on the concepts of partitioning and addressing.
   - **Addressing**: Defines the direction of calculation. It is determined by the checked fields in the Table Calculation dialog box. You can reorder these fields to change the direction.
   - **Partitioning**: Determines the group or level where the calculation is evaluated. It is influenced by the unchecked fields in the dialog box. It can be at the cell, pane, or table level.
   - **Practical Application**: The tutorial demonstrated how to change table calculations by selecting different partitioning and addressing fields in a practical scenario.
   - **Tips**: 
      - Frequently check and uncheck options to find the best calculation method.
      - Using 'compute using' options can cover most needs, but for specific needs, customize dimensions.

- **Parameters**: The lesson progressed to a detailed explanation of parameters in Tableau Desktop, a tool that allows for dynamic and customized dashboards.
   - **Definition**: Parameters are dynamic values that can replace constants in calculations, filters, or reference lines. They can be seen as "fake fields" created from existing data sources or defined values.
   - **Advantages**:
      - Operate independently of data sources.
      - Enhance performance compared to regular filters.
      - Can update dynamically in Tableau versions 2021 and later.
      - Work well with parameter actions for interactive visualizations.
   - **Limitations**:
      - Single-select only.
      - Cannot embed logic.
      - Lacks an "all" option seen in filters but can be bypassed with calculated fields.
   - **Creating Parameters**:
      - From the top menu within a filter.
      - From a field through the context menu.
      - In white space, though it doesn’t pre-populate information.
   - **Upcoming Topics**: The lesson hinted at exploring parameter actions in an advanced course and mentioned that the following segment would cover the practical usage of parameters.

**Next Steps**:
1. Understanding the common uses of parameters.
2. Learning to apply parameters effectively in Tableau Desktop.

### Common Parameter Use Cases

- In this Tableau Desktop online course section, the tutorial covers two main uses of parameters in your dashboard, enhancing user interactivity and reducing rework:
  - **Creating custom thresholds through calculated fields**:
    - You can set parameters inside calculated fields for logical operations that end-users can modify, such as defining sales buckets (upper, mid, lower level) based on the sales sum values.
    - Changes can be applied dynamically, altering visual elements like colors in the view, enabling users to set and alter thresholds as needed.
  - **Implementing dynamic top-end filters**:
    - Rather than fixed numbers, parameters allow end-users to set dynamic ranges for top-end filters, presenting a drop-down menu for them to input or select values, enhancing the dynamism of the filter function.
    - You can embed parameters in raw SQL pushed to your data source, a feature unique to parameters.

- **Hands-on demonstration**:
  - Creating a bar chart named "Top customers by sales" by selecting appropriate measures and dimensions, followed by sorting and setting up a horizontal bar chart.
  - **Setting up a dynamic top filter**:
    - A "Top N customers" parameter is created to allow users to dynamically select the top N customers based on sales.
    - Demonstrated how changing the parameter value dynamically alters the visualization.
  - **Setting up a dynamic tier threshold**:
    - Created a new parameter named "top tier customer threshold" to classify customers based on a sales threshold.
    - Introduced a calculated field named "top tier color" to apply colors based on the tier classification dynamically.
    - Highlighted that parameters need to be connected to a tool, like a calculated field, to become functional.

- The demonstration clarifies that parameters increase dashboard interactivity, allowing for dynamic adjustments and analyses. It ends by noting that parameters will be discussed in more depth in an upcoming advanced topics course.

### Customizing Parameters

In this Tableau Desktop online course section, the focus is on customizing parameters to enhance the utility and efficiency of your dashboard. Here is a summarized breakdown:

- **Naming Parameters**: Choose descriptive and possibly alphanumeric names for easy sorting and retrieval.
  
- **Data Types**: Parameters support various data types including float, integer, string, boolean, and date/time. Your choice depends on the particular needs of the parameter.
  
- **Default Value on Workbook Opening**: Introduced in version 2020.1, this feature lets you set a custom default value, possibly derived from a calculated field, to appear whenever the workbook is opened, avoiding data stagnation and frequent republishing.
  
- **Display Format**: This dictates how data is presented to the end user without altering the underlying data. It allows for customization such as setting the display to dollars or adding multiple decimal points.
   
- **Allowable Values**: You can define the range of values that users can pick from; opting for 'all' grants complete freedom, while 'range' restricts choices to a predetermined set. Dimensions usually utilize the 'list' option.
   
- **List Option in Allowable Values**: Here you can define raw values and their aliases for user-friendliness, making adjustments without affecting the existing data source.

- **Parameter Updating**: Options include a fixed value or automatic update upon workbook opening, the latter keeping parameters current according to changes in the referred data source. It requires a compatible, single-value, and present data field to function properly.

- **Parameters in Advanced Analysis**: Though this session equips you with basic knowledge, there is more to learn about parameters in upcoming advanced topics.

Remember, naming parameters well and wisely using the data type and allowable values options will aid in efficient parameter setup, fostering a dynamic and user-friendly dashboard. It's advised to upgrade to newer Tableau versions to leverage the full potential of parameters, including automatic updates, promoting a dynamic and enriching data visualization experience.

## Dashboards & Stories

### Tableau Dashboards

In this part of the Tableau Desktop online course, you will learn about the intricacies of creating dashboards, which are vital tools in visualizing a comprehensive view of data sources by uniting sheets, objects, images, and web content. Below is a summarized guide to ponder as you embark on creating dashboards:

- **Purpose of the Dashboard**: Always be guided by the main objective of your dashboard. Understand what you wish to convey — be it a conclusion or raising a question. 

- **Understanding Your Audience**: Know who will be using the dashboard as it guides the level of detail and the functionalities to incorporate. 

- **Data Recency and Volume**:
  - **Recency**: Ascertain the freshness of the data required, which may vary from live data to weekly updates, impacting the design.
  - **Volume**: Consider the extent of data needed, whether it spans over years or geographical limits, to efficiently manage data pulling and usage.

- **Method of Consumption**:
  - **Device**: Acknowledge the variety of devices (like laptops, desktops, or phones) your end users will employ to access the dashboard.
  - **Location**: The users might be accessing the dashboard from different locations — field, home office, or via shared drives — influencing the design.

Being aware of these aspects will aid in crafting dashboards that not only satisfy users' needs but are also efficient and purpose-driven. Having deliberated these concepts, the next step is to delve into the practicality of dashboard creation in Tableau Desktop to become adept at utilizing this tool to its fullest potential. Remember, a well-planned approach to dashboard creation, keeping in mind the audience and purpose, is pivotal for success.

### Dashboard Layouts

In this section of the Tableau Desktop online course, we delve deeper into the specific functionalities and features of the dashboard and layout panes in Tableau Desktop. Here are the essential details:

- **Dashboard Pane**:
  - **Device Preview**: Allows preview of how dashboards appear on various devices before publishing, ensuring a functional design for all device types.
  - **Dashboard Size**: Defines the principal size of your dashboard, which can be set to fixed, automatic, or a range.
  - **Sheets**: Facilitates preview of workbook sheets before inclusion into the dashboard; proper naming convention aids in easily locating the necessary sheets.
  - **Objects**: Assist in organizing sheets and enhancing design through features like containers, navigation buttons, text web pages, etc.
  - **Tiled and Floating**: Options to position sheets and objects in the dashboard, with tiled option adhering to the grid and floating allowing movement through coordinates; each with its merits and demerits.

- **Layout Pane**:
  - **Controls**: Available at the top for managing title display, tile and floating options through a clickable checkbox.
  - **Sheet Configuration**: Manage sheet size through width, height, and position settings, which operate on a pixel-related coordinate system.
  - **Design Features**:
    - **Borders and Backgrounds**: Offers customization of sheet border color and style, along with background color.
    - **Padding**: Ensures control over the white space surrounding your sheets, avoiding the need for additional blank objects.
  - **Item Hierarchy**: Displays the layered structure of objects in your dashboard, helping in locating what you need easily.

- **Creating a New Dashboard**:
  - **Initiation**: Begin by clicking the square icon with a plus sign at the bottom right side.
  - **Naming**: Rename it as per preference, for instance, "Executive Dashboard."
  - **Positioning**: Drag the dashboard to the preferred side for ease of organization, and customize the display style of sheets between name, filmstrip, and gallery based on your convenience.

The segment prepares you for the hands-on task of starting with your dashboard creation, and insights into how to utilize both tiled and floating will be covered in the subsequent lesson. It is pivotal to acquaint yourself with these functionalities to build a dashboard that is not only efficient but also user-friendly, facilitating a smooth navigation process.

### Tiled vs. Floating Layouts

In this Tableau Desktop online course module, you learned the distinctions between tiled and floating objects, how to utilize them, and the respective advantages they offer in dashboard design. Here's a breakdown:

- **Tiled vs Floating Objects**
  - **Personal preference**: While some hardliners prefer exclusively using one over the other, it often comes down to personal preference.
  - **End-users**: Usually, they can't distinguish between the use of tiled or floating layouts in the final product.
  
- **Tiled Objects**
  - **Grid system**: Objects snap to a grid when dragged, facilitating organization.
  - **Mobile viewing**: Generally preferred for mobile dashboard views.
  - **Utilization**: Initially, best to tile everything as you learn to navigate Tableau.
  
- **Floating Objects**
  - **Pixel-perfect design**: Allows for precise placement on exact pixels, ideal for designers keen on precision.
  - **Tableau Server**: Can enhance rendering performance on Tableau Server as it defines exact dimensions, avoiding resolution discrepancies.
  - **Learning curve**: Might take longer to master compared to tiling objects.

- **Practical Tips**
  - **Container deletion**: You can delete containers to remove legends but retrieve them later.
  - **Sheet replacement**: Facilitates swapping sheets without deleting, aiding in finding the perfect design.
  - **Checking usage**: Right-click on sheets to check which dashboards they are utilized in, helping to foresee the impacts of altering a sheet.

- **Upcoming**
  - **Dashboard sizing**: The next module will guide you on determining the optimal dashboard size according to your requirements.

Remember to try both tiled and floating objects practically in Tableau Desktop to understand their application better and to find which method suits your designing style the most. It encourages finding a comfortable middle ground between tiled and floating objects for efficient and appealing design outcomes.

### Dashboard Sizing

In this part of the Tableau Desktop online course, the focus is on dashboard sizing, which can be categorized into three main options: fixed size, automatic sizing, and range. 

- **Fixed size**:
  - Allows you to define a specific width and length for the dashboard either manually or through pre-designed templates (options include generic desktop webpage, embedded, small blog, etc.).
  - Pros: Faster rendering time as Tableau Server understands the size immediately.
  - Cons: Can be hard to view on devices that don't support the chosen size.
  - Recommended for maintaining the intended analytics without distortions.
- **Automatic sizing**:
  - Adjusts the dashboard to fit the user’s device size.
  - Not recommended due to the potential for the dashboard appearing distorted depending on the end user's screen size.
- **Range**:
  - Allows you to set a minimum and maximum size for both width and height, providing some flexibility in dashboard size while maintaining some control.
  - Can be useful for dashboards viewed on varying device sizes.
- **Pro tip**:
  - Suggested to opt for a fixed size supported with a device designer to preview and optimally design for different devices.
- **Practical application**:
  - The tutorial guides you in selecting and setting up a fixed size of 1200x1200 pixels for an executive dashboard in a Tableau workbook, emphasizing that it will facilitate fitting substantial content effectively.

Remember these key points as you work through dashboard sizing and to explore the device designer feature for more advanced optimization. The next part of the course will delve into dashboard objects.

### Dashboard Objects

In this lesson, we delve deeper into dashboard objects in Tableau Desktop, a pivotal tool in setting up a proficient dashboard. Here’s a breakdown of the crucial elements:

- **Dashboard objects**: These can encompass a variety of functionalities including adding external images and web pages, extensions, and facilitating navigation between dashboards.
- **Containers**: These come in horizontal and vertical layouts and assist in the structured arrangement of objects within defined spaces, enabling easier organization and rapid adjustments for different devices.
- **Text boxes**: Utilized for showcasing flat text or parameters but are limited as they cannot display created fields.
- **Images**: Allows the integration of local images and the setting of target URLs to link to other pages or tools when the image is clicked.
- **Web pages**: They can be embedded in your dashboard and can take parameter selections directly from the URL, providing an extended array of possibilities for dashboard interaction with other tools and web objects.
- **Extensions**: These are third-party applications that enhance your dashboard’s functionality; however, their usefulness is restricted without Tableau Server.
- **Export buttons**: These facilitate easier access to exporting options, permitting end users to export data as images, PDFs, or PowerPoint files, enhancing the user-friendly nature of your dashboard.
- **Navigation buttons**: Streamline the process of toggling between different dashboard pages, offering a seamless, app-like experience.
- **Blanks**: Initially designed to create space between objects, they are now primarily used to cover objects to avoid unnecessary hover-overs and distractions.

In the next step, we will apply what we learned by adding these objects to our Tableau Desktop dashboard, understanding that this practical application aids in grasping the nuanced utility of each object.

### Dashboard Formatting Options

In this segment of the Tableau Desktop online course, the instructor emphasizes the vital role of formatting in creating a dashboard. Here are the primary takeaways:

- **Importance of formatting**:
  - Constitutes about a third of the dashboard creation time.
  - Vital for making the dashboard polished, clean, and user-friendly.
  - A well-formatted dashboard is more likely to be used as it is easier to consume and extract information from.
- **Formatting options in Tableau**:
  - **Workbook level**: Affects the entire workbook; applying changes at this level will overwrite existing settings but individual components can still be altered later.
  - **Worksheet level**: Only impacts the specific worksheet being worked on, not affecting others in the workbook.
  - **Individual elements**: You can specifically format titles, captions, tooltips, legends, fields, and field labels, as well as number and text formats separately.
- **Accessing formatting options**:
  - The quickest way to access the formatting menu is to right-click the item you wish to format and choose the formatting option in the dialog box that appears.
- **Tips for learners**:
  - The right-click shortcut is a helpful tool to quickly access formatting options.
  - While the tutorial will cover a wide range of options in depth, learners do not have to use all of them; it depends on individual preference and the needs of their dashboard.
  - Proper formatting can give one an edge in the competitive field of dashboard development.

The tutorial urges learners to perceive their dashboard as a product that needs to be both functional and aesthetically pleasing to effectively serve its purpose. The following lessons will delve deeply into the various formatting options, starting with workbook level formatting.

### Workbook-Level Formatting

In this Tableau Desktop lesson, we focus on Workbook Level Formatting, a high-level formatting style that is applied to the entire workbook. Here's what was covered:

- **Workbook Level Formatting**: Located in the format menu under the workbook option, this facilitates universal changes to fonts and lines across all sheets in the current workbook.
- **Fonts**:
  - **Workbook level fonts**: Can alter all fonts or specify changes to worksheets, tooltips, and various titles. All elements default to the Tableau font which ensures compatibility, especially when using Tableau Server.
  - **Customizing**: While you can initiate a blanket change initially, individual adjustments can still be made later without being overwritten unless revisited and altered in the workbook menu.
  - **Choice of fonts**: The instructor prefers Century Gothic but advises caution as the selected font must be supported by the Tableau server machine to avoid display issues.
- **Lines**:
  - **Workbook level lines**: Encompasses grid lines, zero lines, trend lines, and more. It doesn't affect grids.
  - **Minimalistic dashboards**: The instructor leans towards minimalistic dashboards with fewer lines for a cleaner appearance.
  - **Modifications**: During the demonstration, grid lines, zero lines, and axis rulers were turned off to achieve the desired look.
- **Practical Application**: Participants were guided to apply workbook level changes, such as altering fonts to Century Gothic and resizing worksheet titles to size 11 for a cleaner and readable appearance.
- **Next Steps**: The subsequent session will explore individual worksheet level formatting for further customization.

Towards the end of the session, attendees were encouraged to personally try modifying different elements as per preference, highlighting the ease and effectiveness of workbook level formatting to achieve a neat and customized dashboard.

### Worksheet-Level Formatting (Part 1)

In the next section of the Tableau Desktop online course, worksheet level formatting was covered, which is a step down from workbook level formatting. Here are the main aspects:

- **Definition and Accessibility**: Worksheet level formatting allows you to modify various elements including fonts, borders, and shading on a single worksheet. It can be accessed from the format menu or by right-clicking on the canvas.
- **Specific Areas to Modify**: This type of formatting lets you control the entire sheet or specific rows and columns separately. Inside these, you find sections such as default, total, and grand total; each housing detailed options for further customizing worksheet, pane, header level, tooltip, and title.
- **Modification Options**:
  - **Font**: Different fonts and sizes can be applied to various areas directly from the font menu.
  - **Alignment**: Adjust vertical and horizontal alignments.
  - **Shading**: Customize color schemes and manage row and column banding.
  - **Borders**: Allows setting borders, including changing color and thickness.
  - **Lines**: Regulate aspects like axis lines, drop lines, and zero lines.
- **Example with Text Table**: The tutorial illustrated the above features using a text table created from sales, profit, and subcategory data, emphasizing the straightforwardness of changing elements like font size and color for different levels including the worksheet, pane, and headers.

**Note**:
- **Practical Use**: Demonstrated the ease of understanding different aspects like pane and header levels through color-coded formatting in the text table.
- **Saved Sheet**: Encouraged saving the created sheet as a reference for future use, highlighting the facility to discern the changes visually.

Remember, while the worksheet level formatting holds numerous options making it a bit overwhelming initially, it offers detailed customization, making it a commonly used feature in formatting tasks. It serves as a prelude to a more in-depth discussion on dashboard formatting to be covered next in the course.

### Worksheet-Level Formatting (Part 2)

In this part of the Tableau Desktop online course, we take a closer look at worksheet level formatting focusing on alignment, shading, borders, and lines, in addition to fonts. Here are the key points covered:

- The session starts with a walkthrough on the **bars sales versus goal tab** of the Tableau dashboard, exploring the formatting options available:
  - **Alignment**: Modifications include left-aligning and bolding headers.
  - **Shading**: Setting the default shading background to "none" to remove the background.
  - **Borders**: Removing all borders including grand totals, row dividers, and column dividers to clean up the view.
  - **Lines**: Removing all axis ticks to simplify the display.

- The course transitions to the **Treemap sales by subcategory sheet**:
  - Here the facilitator showed how to swiftly access the formatting menu through a right-click, and how to adjust header styles directly.
  - The borders for this sheet were all removed to create a cleaner look.

- Moving on to the **bar line monthly sales trend** sheet, the formatting focus remained on removing all borders to enhance the visual appearance.

- Lastly, on the **map sales and profit** sheet, similar formatting steps were applied, notably removing all the borders to tidy up the view.

- The course emphasizes the importance of not getting bogged down in over-detailing every element, and to focus on impactful changes that enhance the user experience.

- It was noted that the next session would delve deeper into number formatting.

It's recommended to practically apply these steps in Tableau Desktop to better grasp the utility of each formatting tool, and to appreciate the transformations they can bring to your dashboard’s aesthetic and readability. It is advised to strike a balance between making necessary changes and avoiding unnecessary complications to save time and effort.

### Number Formatting

In this Tableau Desktop online course session, the focus is on finalizing dashboard formatting with a particular emphasis on number formatting. Below are the key points to note:

- The session started with a focus on number formatting, which is essential before proceeding with dashboard modifications.
- Emphasized the personalization of dashboards, encouraging learners to modify their dashboards as per individual preferences while following along with the tutor.
- **Number Formatting Options in Tableau:**
  - **Axis Tab and Pane Tab:**
    - Axis Tab houses pre-selected and customizable options, including:
      - Automatic (default, no decimals)
      - Number standard (based on locale)
      - Number custom (customizable decimal places, suffixes, etc.)
      - Currency options (standard and custom based on locale)
      - Scientific and percentage options
    - Pane Tab, similar to the Axis tab, with additional features like control over defaults, totals, grand totals, and special values. 
    - Allows for font and alignment modification.
- **Accessing Formatting Menus:**
  - Right-click on the axis for the axis menu.
  - Right-click on a pill within your view to access various formatting options.
- **Pro Tips:**
  - Application of default field properties to maintain consistent formatting across the workbook.
  - Modification of specific measures from the left-hand side to influence workbook level formatting change, impacting the default value whenever that field is used.
- **Practical Application:**
  - The tutorial involves practical application, demonstrating how to implement the discussed formatting options on a Tableau dashboard.

Towards the end, learners are guided to open Tableau Desktop for a hands-on experience to finalize formatting for their workbook, emphasizing it to be a straightforward process due to the learning accrued so far. It marks the preparation stage to transition from the formatting phase completely.

### PRO TIP: Transparent Sheets

In this part of the Tableau Desktop online course, the discussion revolves around utilizing transparent sheets to enhance dashboard aesthetics. Here are the main points:

- **Introduction to Transparent Sheets:**
  - Initially introduced in Tableau version 2018.3.
  - Allows creative layering or stacking of objects and visuals on a dashboard.
  - Useful for layering visualizations over custom images imported into the dashboard.
- **Implementing Transparent Sheets:**
  - Can be achieved by either tiling or floating sheets over one another.
  - To create a transparent background: 
    - Right-click and navigate to "format background."
    - Select "none" in the format shading menu under the sheet default section.
  - Enables viewing of everything behind the top sheet, offering a dynamic visualization approach.
  - Advise against overusing to avoid visual confusion.
- **Example of Transparent Sheet Dashboard:**
  - Presented a woodland-themed dashboard with custom fonts and a PNG image as the background.
  - Layered various sheets with transparent backgrounds over the image, including a map, descriptions, and aggregated data, enhancing the visual appeal.
- **Practical Session:**
  - Encouraged learners to test out the feature in Tableau Desktop by:
    - Selecting a sheet to be floated over the dashboard.
    - Applying transparency to the sheet through the shading menu, demonstrating real-time changes.
    - Highlighted the possibility to design impactful dashboards by effectively utilizing layering with transparent sheets.
  - Emphasized maintaining a balance between design and functionality to prevent a cluttered dashboard and ensure user-friendliness.

Towards the end, it was suggested to explore the technique personally and envision various ways to incorporate it into individual projects. The session ends with a note on the upcoming topic, which is action filters. It hints at a continual process of learning more enhanced features to improve dashboard design in Tableau.

### Action Filters

- **Action Filters in Tableau Desktop**
  - **Introduction to Action Filters**
    - **Definition:** Allows end users to apply dashboard filters by interacting with visual components on the dashboard.
    - **Utility:** Creates intuitive interaction and enhances the diversity of the dashboard functionalities.

  - **Implementing Action Filters**
    - **Adding action filters:** Utilize the "use as filter" button present in any sheet on the dashboard.
    - **Customizing filters:** Via the "edit filter action" menu, one can modify various attributes such as:
      - **Source sheets:** Determines the origin of the action.
      - **Run action on:** Specifies how users trigger the action (hover, select, or menu).
      - **Target sheets:** Identifies which sheets will be impacted by the action.
      - **Clearing the selection:** Dictates what happens after the action is deactivated.
      - **Target filters:** Controls which fields are affected in the target sheets.

  - **Advanced Customizations**
    - **Naming:** Customize filter names to clearly denote their function.
    - **Field Selection:** For improved performance, it is advisable to limit the fields affected by the action to only those necessary.
    - **Testing:** Always test new actions to ensure they function as intended and to prevent errors due to missing fields.

  - **Guidelines for Designing Dashboards**
    - **Z-pattern Design:** Arrange the dashboard so that users interact with it in a 'Z' pattern, enhancing the intuitive nature of the design.
    - **Action Filter Applications:** 
      - **Regional filter:** Restrict the action to relevant sheets to streamline the user experience.
      - **City and State filters:** Configure to impact all sheets except the bar sales vs goal section, enhancing focus on city and state data.
      - **Category and subcategory filters:** Designate specific source and target sheets for these filters to ensure the dashboard remains organized and user-friendly.
   
*Note:* Incorporate the feature of testing different options and always scrutinize the performance to ensure optimal functioning, especially in complex dashboards with large data sets.

### The Device Designer

In the Tableau Desktop module on utilizing the device designer, the key takeaways are:

- **Device Designer**:
  - Facilitates the creation of dashboards optimized for various devices such as desktops, tablets, and phones, without creating separate dashboards for each.
  - Houses a "default dashboard" where all sheets and legends to be used in different views should exist.

- **Views**:
  - **Desktop view**: triggered on devices over 800 pixels.
  - **Tablet view**: applied on devices with 501 to 800 pixels.
  - **Mobile view**: used on devices below 500 pixels.
  - Each view caters to different use-cases and should be designed accordingly.
  - The Tableau server may not properly recognize the device when a dashboard is embedded in other tools, impacting the dashboard's appearance.

- **Creating Different Layouts**:
  - **Phone layout**: automatically generated but can be customized further for optimized viewing.
  - **Tablet layout**: can be customized and previewed for various tablet models before publishing.
  - **Desktop layout**: added through the dashboard menu for customization.
  - It is advised to use a fixed size dashboard with different layouts for flexible viewing across devices.

- **Preview and Customization**:
  - **Device preview option**: enables visualization of the dashboard on different devices before publishing.
  - **Rotation feature**: allows users to see the dashboard in both landscape and portrait modes.
  - **Layout editing**: offers options to adjust size, modify sheets, and optimize layout, facilitating efficient design for smaller screens like phones.

- **Pro tips**:
  - Create separate sheets specifically for phone layout in the default view to ensure impactful visuals given the limited screen size.
  - Consider leveraging the "optimize layout" option to tidy up manually created phone layouts.

Remember that considering how end-users will interact with the dashboard across different devices is essential to ensure effective dashboard design. The session concluded with a hint at exploring "stories" in the upcoming segment, illustrating how they differ from dashboards.

### Creating Stories

- Stories in Tableau Desktop facilitate the creation of visual sequences that build narratives, enhancing the presentation of data by adding context and bringing it to life.
- Stories merge the functionalities of Tableau and PowerPoint, allowing users to embed both dashboards and sheets into a sequential visual narrative, each part referred to as a "story point".
- Features:
  - **Caption customization**: Modify captions with options such as boxes, numbers, dots, and arrows to navigate story points with contextual insights.
  - **Dynamic interaction**: Unlike PowerPoint, stories permit real-time data interaction, answering queries on-the-fly during presentations.
  - **Annotation**: Highlight specific details on the dashboard to emphasize important points in your narrative.
- **Usage in a presentation**:
  - Creating a story helps in drilling down into detailed dashboard views, essential during live presentations to ensure no crucial points are missed.
  - During a presentation, in case of queries, one doesn't need to diverge from the created content as the full data and Tableau functionalities are at disposal.
  - Stories are interactive, enhancing narratives during presentations by allowing data drilling at any point.
- **Creating a story**:
  - The last button on the ribbon labeled "New Story" initiates a new story, where users can drag and adjust the size of the dashboard to fit into the canvas.
  - Users can select a focal point (e.g., New York City) and annotate it to highlight it during the presentation, aiding in the narration.
  - The caption tool helps in underlining the main points during the story narration, for instance, emphasizing high sales in New York state.
  - By saving actions as new captions, one can delineate different stages in the story, facilitating a deeper analysis as the narration progresses.
  - It is possible to freeze specific moments to focus on during the presentation, enhancing the delivery to the end user.

*Note*: The process of creating a story was demonstrated with a practical example, iterating through various functionalities such as creating story points, annotating marks, and highlighting specific data points to build a compelling narrative with data. The next topic in the course will cover best practices in data visualization.

### Data Visualization Best Practices

In the segment discussing the best practices for data visualization while using Tableau, the following key pointers were noted:

- **Understand your audience**: Engage regularly with your audience to gather feedback and avoid creating the dashboard in isolation. Always prioritize the needs of your end-users over your preferences to build a user-friendly dashboard.
  
- **Maintain simplicity**:
  - Resist the temptation to include unnecessary details and features, focusing instead on the clarity of the information presented.
  - While inspiration can be drawn from various high-level works showcased on Tableau Public, it's crucial to remember the distinction between what is suitable for the internet and what meets your end-users' needs.
  - Opt for a design that caters to a broad user base rather than a select group of Tableau experts.
  
- **Avoid continuous redesign**: Although refreshing the design occasionally is advisable, it should be done incrementally to help users adapt gradually and appreciate the dashboard's functionality.
  
- **Stick to basics**:
  - Employ basic visualization forms like bar charts when appropriate but also be open to presenting new concepts.
  - Do not insist on achieving perfection; adhering to the 80/20 rule can help in concentrating on the significant aspects that enhance your dashboard's impact without focusing excessively on minor details.

*Tip*: While it's encouraged not to seek perfection, attention to detail in terms of functionality can make a substantial difference in the overall impact and usefulness of your dashboard.

