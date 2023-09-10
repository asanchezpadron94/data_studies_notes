#tableau

Course: https://www.udemy.com/course/tableau-desktop-speed-performance/
This summary was created by GPT4.

## Performance Optimization
### Why is performance so important

In this segment of our Tableau Desktop online course, we will discuss the pivotal role of workbook performance in fostering effective analytics. It revolves around three primary deliverables:

- **Speed to insight:** Acting as a central force in visual analytics, a faster insight generation facilitates swifter business decisions, ultimately enhancing the utility of your dashboard.
   
- **Analytic flow:** Maintaining a smooth analytic flow ensures efficiency, fostering high-quality insights and analyses that are crucial for a business's growth.
   
- **Iterative development:** Enhanced performance not only truncates dashboard development time but also elevates throughput during development cycles, resulting in comprehensive visualizations aligned with business expectations.

Performance speed invariably affects numerous aspects of the analytic domain, necessitating rapid analytics in our daily and professional spheres to keep pace with the fast-evolving business environment.

### Key Performance Questions

These key questions are:

- **Granularity of the needed data:**
    
    - Establish the level of detail essential for addressing the queries of business users, taking into account the dashboard's purpose.
    - Determine whether specific data like monthly sales trends suffices or if detailed data down to the order line level is necessary.
      
- **Data source and its management:**
    
    - Understand the nuances of your data source to explore viable options for dashboard performance optimization.
    - Ascertain whether you are linking to a regulated published source or possess complete control over the pertinent data.
      
- **Data update or refresh frequency:**
    
    - Recognize the significance of data freshness in organizing and storing your data.
    - Evaluate the necessity for real-time data, considering the restrictions and optimization steps involved with live connections, as opposed to the broader array of performance-boosting opportunities offered by data extracts.
      
- **Existing performance expectations:**
    
    - Discern any pre-existing expectations the team may harbor regarding dashboard performance.
    - Establish a common ground on acceptable performance levels to prevent unforeseen challenges during the development phase.

It is paramount to comprehend that "good performance" is a subjective term and varies with the audience; hence, aligning with the team's norms and expectations is crucial in dashboard development.

### Internal vs External factors

**Internal Factors**

Directly within the developer's control, these should be the primary focus for optimization. They include:

- **Data source optimization:** Be it a local or published source, database, or file, developers have the liberty to optimize it through various means such as filtering and aggregation.
- **Workbook alterations:** Developers hold substantial control here, able to modify various elements including visualization, filters, and dashboard size to foster performance improvements.

**External Factors**

While potentially controllable, these generally involve environmental aspects or elements governed by other team or company members, necessitating external assistance for optimization. They encompass:

- **Database structures and permissions:** Often beyond the developer's reach, alterations here demand coordination with database administrators and actions outside the Tableau platform.
- **Tableau server adjustments:** Depending upon the developer’s role and permissions, changes here may be possible but tend to be slower, especially in larger organizations, affecting all users, not just those engaging with your workbook.
- **Network constraints:** Incorporating elements like internet speed and VPN connections, it remains a challenging aspect to control. Developing and testing locally is advised to obtain baseline performance results, despite the acknowledgment that server performance may be slightly reduced.

### VizQL & Query Processing

In this segment of the Tableau Desktop online course, we delve into the workings of Tableau Workbooks and their underlying data processing pathway, which revolves around SQL or a visual query language acting as a catalyst in transforming user data inputs into queries and eventually into visual representations in Tableau. Here, we outline the crucial eight-step pathway:

1. **Request:** Initiated when a user chooses a dashboard or a specific action in a dashboard.
2. **Initial layout:** It is rendered devoid of data at this juncture.
3. **Viz:** Transforms user inputs into a structured query, directing it to the associated data source.
4. **Data retrieval:** The chosen data source, be it local, published, or a live connection, is accessed to extract the necessary data.
5. **Tableau calculations:** Following data retrieval, Tableau undertakes the computation of the necessary calculations.
6. **Layout finalization:** This is defined based on the query outcomes.
7. **Visualization rendering:** Occurs either on the server-side or desktop-side, evolving into the visual representations.
8. **Final rendering:** Exclusive to Tableau Server users, it takes place on the client-side browser; desktop users bypass this phase.

Despite the multitude of steps involved, users generally perceive this as a rapid process, barely noticing the transition from a blank screen to a data-filled visualization, thanks to the efficiency of the pathway.

Key opportunities for optimization prominently lie in enhancing the query calculations, rendering, and layout phases, offering substantial scope for improving workbook data processing paths.

In the upcoming section, we will unravel the concept of performance recordings in Tableau, both on Desktop and Server, providing a deeper understanding of the ways to fine-tune performance. Stay tuned for more insights.

### Performance Recording

In this segment of your Tableau Desktop online course, you are guided on how to utilize the performance recording tools available in Tableau Desktop to monitor object load times and pinpoint areas for potential enhancement both locally and on the Tableau Server. Here's a detailed breakdown:

- **Performance Recording Tools**
  - Exclusive to Tableau Desktop and Server; not available on Tableau Public.
  - Helps in identifying and targeting potential areas for optimization.
  - Can be accessed via a trial or full version downloadable from Tableau’s official website.

- **How to Record Performance on Tableau Desktop**
  1. Navigate to the help menu, then to settings and performance.
  2. Select "Start Performance Recording".
  3. After rendering your dashboard, return to the menu to stop the recording.
  4. A new workbook will open displaying the results.
  5. Keep the recording simple to easily identify areas needing tuning.

- **Recording Performance on Tableau Server**
  - Entail adding a specific URL parameter before the ID section of your dashboard web address.
  - Recording begins immediately, and results can be viewed by clicking the performance icon on your dashboard.

- **Tips for Effective Recording**
  - Start from a blank page for a clean cut of the performance recording, avoiding any unwanted queries or renders.
  - Save the baseline recording for future comparisons.
  - Conduct multiple recordings to obtain a substantial range of performance data.
  
- **Next Steps**
  - Up next, you will learn to interpret the data from your performance recording workbook to understand and analyze the performance baseline established through the recordings.
  - You will further explore how to scrutinize and leverage this data to optimize your Tableau workbooks.

This section essentially equips you with the foundational knowledge and skills to initiate performance recording, setting a baseline to track and improve your dashboard’s performance over time through informed analysis of recording results. Stay tuned for further insights on interpreting the performance recording outcomes.

**Interpreting Performance Results**

In this Tableau Desktop online course section, you are instructed on how to read and interpret the results obtained from performance recordings, which can aid in optimizing your workbook’s efficiency. Here's the detailed summary:

- **Understanding Performance Summaries**
  - It’s necessary to use Tableau Desktop (not Public) for performance recordings.
  - Performance recording workbook appears automatically once recording stops.
  
- **Interpreting Results**
  - **Timeline**
    - Presents events chronologically along with their durations.
    - Use to identify slow worksheets and dashboards for optimization.
  - **Events List**
    - Displays events in descending order based on runtime.
    - Focus on the longest bars and utilize filters to explore specific timelines and queries (green bars represent executing queries).
  - **Query Detail Section**
    - Initially blank; showcases code upon clicking a green bar in the events list.
    - Requires a local source to view SQL queries, while published sources show HTML code.
    - Advised to record performances after substantial dashboard modifications to track improvements.
    
- **Reviewing Initial Baseline Recording**
  - Created in the previous lesson to identify the poorest performances and understand the origins of most time-consuming queries and events.
  - Utilize the slider to filter events based on their time duration.
  
- **Analyzing Timeline and Event Sorted Sections**
  - Events are categorized based on workbook, dashboard, worksheet, and event type.
  - Observing parallel and sequential events helps in a detailed analysis.
  
- **Query Details**
  - To better interpret query texts:
    - Copy data by right-clicking on query text.
    - Paste it in a text editor like Notepad++.
    - Choose SQL in language settings and remove initial quotes for clearer, color-coded SQL like codes, enhancing readability.
  
- **Next Steps**
  - In the following lesson, delve deeper into understanding different performance recording event types and learning how to effectively work with them.

With these insights, you learn to proficiently analyze the performance recording results, guiding you to locate and work on the areas needing improvements for an efficient workbook operation. Stay tuned for learning how to work with different event types in performance recording.

### Event Types

In this segment of the Tableau Desktop online course, various event types in performance recording and how to optimize them for a more efficient workbook are discussed. Here is a concise summary:

- **Examining Performance Recording Event Types**
  - **Objective:** To identify and mitigate issues hampering the workbook’s speed and performance.
  
- **Common Event Types and Optimization Strategies**
  - **Connecting to Data Source**
    - Issue: Long connection runtimes, especially with published sources.
    - Solution: Use extracts, data source filters, and embed data source connections.
  - **Sorting Data**
    - Issue: High mark counts and sorting in visualizations taxing the workbook.
    - Solution: Use data source filters and aggregate extracts on visible dimensions.
  - **Computing Layouts**
    - Issue: Dashboards with numerous sheets and objects with dynamic sizes.
    - Solution: Specify dashboard size and remove unnecessary elements.
  - **Executing Query**
    - Issue: Long-running queries slowing down the workbook.
    - Solution: Specify action filter fields and replace normal filters with parameters.
  - **Blending Data**
    - Issue: Applying blends across data sources in calculations.
    - Solution: Leverage relationships instead of blending data.
  - **Geocoding Events**
    - Issue: Granular geospatial maps putting additional load on the workbook.
    - Solution: Raise the grain of geocoding and focus on a specific region.
  - **Server Rendering**
    - Issue: A downstream impact driven by other events.
    - Solution: Address the root causes impacting server rendering.
  - **Computing Total Events**
    - Issue: Grand totals and subtotals causing slow performance.
    - Solution: Remove or reduce totals and use other types of calculations.

- **Deep Dive into Recording Event Type Results**
  - **Objective:** Analyzing the specific events affecting the workbook’s performance in the baseline performance recording.
  - **Actions Taken:**
    - Identifying the long runtime events and understanding the total runtime.
    - Grouping event types together to pinpoint key areas for optimization.
  - **Note:** Performance recordings will be conducted after each major section of the course to track improvements.

- **Next Steps**
  - **Objective:** Delve deeper into workbook performance factors in the next segment.

By learning to analyze and address the specific event types causing inefficiencies, you are empowered to enhance the workbook's speed and performance, setting a benchmark for future optimizations. Stay tuned for a broader discussion on workbook performance factors.

### Workbook Performance Factors

In the next section of the Tableau Desktop online course, we will delve into workbook performance factors that predominantly influence the efficiency of dashboard performance. The discussion will encompass the following four pivotal aspects:

- **Data design (40% impact):** This fundamental area offers the most substantial scope for improving dashboard functionality. Key elements include the dimension of raw data, data modeling, column and row numbers, source types, and data source filtering.

- **Filtering (25% impact):** Following data integration in the dashboard, filters serve as critical tools for end users and visual design aids. Proper filter application is crucial as it involves data management that can affect dashboard speed and efficiency.

- **Calculations (20% impact):** Although they furnish essential utilities for developers, calculations demand thoughtful construction and deployment to ensure optimal operation.

- **Layout and visuals (15% impact):** While often deprioritized, the strategic organization and visualization of the dashboard considerably influence its performance.

Remember, while we've assigned specific percentages to indicate the relative impact of each factor, all are integral to achieving a high-performance dashboard. A deficiency in any sector can drastically impede performance. Hence, it is imperative to meticulously evaluate every area before launching your dashboard for business utilization.

## Data Design Optimization

### Intro to Data Design

In this segment of the Tableau Desktop online course, we aim to delve deep into the critical aspects of data design and how it impacts workbook performance. Key takeaways will be:

- **Introduction to data modeling options**
  - Relationships
  - Unions
  - Joins 
  - Blending
    
- **Understanding connection types and their optimization techniques**
  - Live vs. extract connections
    
- **Analysis of different data source types and their performance implications**
  - Flat files
  - Databases
  - Published sources


### Data Modeling

In this part of the Tableau Desktop online course, the focus is on the utilization and understanding of different data modeling options for optimizing workbook performance. The main points covered include:

- **Data Modeling Options in Tableau Desktop**
  
  - **Relationships**: 
    - Create contextually appropriate joins using related fields between tables.
    - The default option in Tableau, minimizing risks of errors like mis-aggregation and duplication.
    - Active only at the sheet level, enhancing performance by reducing the complexity of queries.
      
  - **Unions**:
    - Combine two or more tables into one, preferably with the same columns and data types.
    - Generally not taxing on performance but requires monitoring the amount of data integrated.
      
  - **Joins**:
    - Merging multiple tables based on join clauses to create new fixed tables.
    - Can create issues like data duplication and aggregation problems; should be used sparingly.
    - Requires accurate keys between the tables and precise data source filters.
      
  - **Blending**:
    - Involves visualizing separate sources in the same view using blended fields, akin to a left join.
    - Not advisable due to potential performance issues, except for high-level, simple visualizations.
   
- **Hands-on Application**
  
  - **Workbook Setup**:
    - Guided through setting up a workbook in Tableau Desktop and Tableau Public, including addressing potential issues with live connections in Tableau Public.
    - Detailed walk-through of optimizing the data model in a workbook, with a focus on transforming a full outer join into a more efficient relationship.

### Live & Extract Connections

- **Live and Extract Connections**
  - **Availability**
    - Supported by Tableau Desktop and Server.
    - Not available in Tableau Public, which allows only extracts.

  - **Live Connections**
    - Maintain a direct link to the source data.
    - Queries the database or file every time a visualization is altered in the Desktop or Server.

  - **Extract Connections**
    - Data is pulled from the source into Tableau's hyper file format.
    - Supported functionalities:
      - Scheduling on Tableau Server to refresh data without overloading source platforms.
      - Enabling advanced features, including level-of-detail calculations.
      - Offline data access, allowing work on dashboards without a network connection.
      - Handling very large data sets (into billions of records).
      - Faster creation, particularly with the advent of hyper technology.
      - Incremental updates to include only the new data during regular updates.

- **Utilization Guidelines**
  - It's common to use both live and extract connections, depending on the scenario.
  - Extracts are generally preferred for enhancing performance and enabling additional functionalities.
  - When creating relationships or joins, each table must have the same type of connection (either live or extract).
  
- **Connection Tips**
  - Preferably use the native connector while connecting to databases, as it is optimized for specific data sources, improving the performance of both live and extract connections.

### Live Connection Optimization

**Workbook Level Tuning**

- **Leveraging Tableau's Relationship Models**
  - Benefits: query optimization and improved performance for distinct count calculations.
  - Method: Keeping tables separate until activated, different from standard joins.

- **Avoiding Custom SQL**
  - Issues with Custom SQL: generates subqueries leading to complex queries and reduced performance.
  - Alternative: Utilize initial SQL which operates once when the workbook is opened, possibly speeding up performance despite some limitations.

- **Utilizing Multiple Sources**
  - Strategy: Employ multiple smaller sources for easier query handling instead of a single large source.
  - Caution: Avoid excessive data source integration and limit cross-data source filtering to prevent performance issues.

**Database Level Tuning**

- **Indexing**
  - Benefits: Speeds up queries by creating lookups or shortcuts for more frequent dimensions.
  - Focus: Index join dimensions and filter dimensions to enhance efficiency.

- **Data Type Casting**
  - Issues: Repeated casting over numerous rows can slow down performance.
  - Solution: Add new fields with different cast types if original fields cannot be altered.

- **Moving Calculations to the Database**
  - Strategy: Shift intensive row-level calculations like LOD or math calculations to the database to avoid burdening Tableau unnecessarily.

- **Creating New Views**
  - Purpose: To amalgamate desired data into a single view, replacing modeling structures or custom SQL queries.
  - Benefits: Despite the time and resources required, it can substantially improve user experience if well-executed.

### Extract Connection Optimization

- **Initial Benefits**
   - Even a basic data extraction can offer performance benefits.

- **Parallel Queries and Query Fusion**

  - **Parallel Queries**: Introduced in Tableau version nine, enables running multiple queries simultaneously, enhancing speed and processing time.
  - **Query Fusion**: Helps in combining and removing queries to run operations more efficiently. Encouraged by having similar dimensions across different sheets.

- **Reduction of Extract Size**
  
  - **Methods**: 
     - Removing unneeded columns
     - Aggregating data based on visible dimensions
     - Utilizing data source filters to lessen the number of rows
     - Choosing between logical and physical extracts based on specific conditions.

- **Embedding Extracts**
  
  - **Benefits**: 
     - Speeds up queries through the creation of temporary tables 
     - Facilitates quicker data transfers 
       
  - **Caution**: Avoid over-embedding to prevent server issues.

- **Materializing Calculations**
  
  - **Description**: Incorporating pre-calculated developer creations into the extract, needing periodic updates when new calculations are introduced.

- **Incremental Extracts**
  
  - **Benefit**: While not directly improving dashboard performance, it eases the burden on the Tableau server, enhancing the workbook and source operation generally.

**Practical Application**:

The latter part of the session involved a hands-on demonstration in Tableau Desktop where participants learned how to:

- Hide unnecessary fields in the data source.
- Add data source filters, including how to exclude all null values in specific columns.
- Execute aggregate functions based on visible dimensions while being cautious of potential calculation alterations due to the process.
   
The session aimed to equip learners with techniques to fine-tune extract connections for better performance, walking them through features like parallel query logic, query fusion, and various methods to reduce extract size, among other strategies, emphasizing a balanced use of features to optimize performance without overloading the server. It closed with a practical demonstration of applying these techniques in Tableau Desktop.

### Data Source Options

In this section of the Tableau Desktop online course, the discussion revolves around selecting the best data sources and connection types to enhance workbook performance:

- **Data Sources**
  - **Flat files (Excel, CSV, PDF)**
    - **Live Connection**: Near-real-time data but often offers poor to fair performance
    - **Extract**: Superior performance because data is translated into Tableau's hyper format; most suitable in numerous scenarios
  - **Server Connections (MySQL, SQL Server, Snowflake)**
    - **Live Connection**: Allows real-time querying but may face performance issues due to database configurations
    - **Extract**: Generally offers good performance, particularly with well-structured and reasonably sized data; can update up to every 15 minutes
  - **Published Sources**
    - **Use case**: Can be shared across multiple workbooks and dashboards, ensuring data validity and security
    - **Performance**: Requires more data transfer time, which can slow down the loading time (between two to tens of seconds more)
    - **Management**: Balancing between published and embedded sources is critical to avoid performance degradation and data source proliferation

**Note**:
- Before proceeding with another performance recording on the workbook, clear the cache by closing all local workbooks to attain an accurate performance assessment.
- Be prepared to open the workbook on a blank page for the next part of the course.

### Performance Impact - Data Design

In the data design portion of the Tableau Desktop online course, the performance impact of various optimizations was analyzed:

- **Initial Testing** 
  - Initial render time: 30 to 34 seconds

- **Post-optimization**
  - Runtimes for this segment fluctuated between 24 and 48 seconds
  - This illustrates an advancement of approximately 15 to 20%
  - Implying that the primary issues lie less with the data source and data model, and more within other sectors set to be optimized like filtering calculations and visuals

- **Data Design Improvements**
  - Altering Join connections to utilize relationships extracted into a hyper file format
  - Concealing unused columns and applying extract filters to remove records and aggregate visible dimensions improved performance
  
- **Observations**
  - The foremost areas to enhance are the execution and compilation of queries, along with rendering
  - Despite a large number of green bars in the event type ranking, many are non-additive due to the simultaneous running facilitated by query fusion and parallel queries, making the situation better than it seems at a first glance

Take into account that this is a good first step in refining performance, and the focus should now shift to further optimizations in other areas for more improvements.

## Filter Optimization

### Intro to Filter Optimization

In this segment of the Tableau Desktop online course, the focus shifts to optimizing filters to enhance workbook performance. Here is what will be covered:

- **Objective**
  - To delve into filter optimization strategies that involve selecting suitable filter types and applying the right filter options, including utilizing alternatives such as set and parameter actions.

- **Key Takeaways**
  - **Filtering Order of Operations**: Understanding the hierarchy and sequence of applying filters to optimize performance.
  - **Filter Types and Their Performance Impact**: Learning the distinction between various date filters and understanding how they affect performance.
  - **Alternative Approaches**: Investigating alternative tactics such as parameter and set actions to facilitate filter actions more efficiently.

- **Goals**
  - Review Tableau's filtering order of operations in detail.
  - Learn general optimization tips and best practices for particular filter types.
  - Compare different date filters and analyze their performance impacts.
  - Explore the alternative approaches to filter actions.

The section aims to offer a more in-depth understanding of filtering and its impact on performance, setting the stage for a detailed exploration of the filtering order of operations.

### Filtering Order of Operations

In your Tableau workbook, filtering operations occur at different stages and affect performance differently. Understanding the Order of Operations, which governs the sequence of computations, actions, and filter applications, can help optimize performance. Here is a breakdown of the main filter types used in Tableau:

- **Extract Filters**
  - Applicable when using extracts.
  - Used during extract creation or refresh.

- **Data Source Filters**
  - The highest level of filtering.
  - Affect the entire data source, encompassing all worksheets and views.

- **Context Filters**
  - Elevated dimensional filters influencing top-end functions.
  - Initially designed to enhance performance, but results vary and are not a reliable solution for performance improvement.

- **Dimension Filters**
  - Utilize a dimension to limit the data displayed on your dashboard.

- **Measure Filters**
  - Employ measure fields to filter sheets or workbooks.

- **Table Calculation Filters**
  - Leverage table or window calculations in visualizations, operating only within Tableau, not affecting the data source.

Additionally, there are secondary elements, including sets, conditional filters, and level of detail calculations, interspersed between the main filters, playing crucial roles in various processes in Tableau.

Remember to consider the Order of Operations not only for filtering but for all operations to effectively manage performance. Applying extract and data source filters generally positively impacts performance by reducing data at the source, whereas context, dimension, measure, and table calculation filters demand careful and precise application due to their varied impact on performance.

### Filter Optimization Tips

To optimize filter performance in Tableau, consider the following general and type-specific best practices:

**General Best Practices**

- **Limit the number of filters**
   - Reduces complexity in queries pushed back to the data source.
- **Avoid filters with large lists**
   - Substituting with custom value lists or wildcard matches can be more efficient.
- **Avoid LOD expression-based filters**
   - They can be resource-intensive; opt for sets inside calculated fields instead.
- **Minimize user filters**
   - They limit Tableau's caching ability and increase data size; consider aggregating to higher-level dimensions.

**Type-Specific Best Practices**

- **Context Filters**
  - Utilize them only if necessary, for functions like top N features.
- **Dimension Filters**
  - Including the dimension being filtered on in sheets can aid performance.
- **Measure Filters**
  - Range type filters tend to perform better than discrete dropdown lists.
- **Table Calculation Filters**
  - Given their potential negative impact on performance, use other filter types instead.

In the practical session with the "Tableau Desktop Performance Data Design Workbook," several steps were undertaken to enhance the performance:

1. **Saving the Workbook**
   - A new version of the workbook named "Tableau Workbook, Performance Filtering Optimization" was created.
   
2. **Removing Unnecessary Filters**
   - Non-essential filters were identified and removed. For instance, filters with long, discreet list types, such as location, latitude, and longitude, were removed.
   
3. **Pausing Data Source Updates**
   - To speed up the removal process, data source updates were paused temporarily.

4. **Reviewing and Cleaning Dashboard**
   - Each filter was reviewed, and unnecessary ones were deleted to streamline the dashboard according to the defined objective: finding the safest path for a cyclist in NYC.

5. **Global Filters Management**
   - Global filters were efficiently managed by removing them from the main source sheet, thereby reflecting the removal across all related sheets.

6. **Reactivating Data Source Updates**
   - After cleanup, data source updates were reactivated to visualize the improved dashboard performance.

By following these best practices and practical steps, you'll ensure a more efficient and high-performing Tableau dashboard, focused on the essential filters to answer the key question at hand, without sacrificing necessary data.

### Filter Options

- **Filter customization in Tableau Dashboard**:
  
  - **Apply Button**:
    - Prevents the dashboard from blanking out when all selections are deselected.
    - Allows users to make multiple selections before executing a query, enhancing user experience and avoiding continuous reloads with each filter adjustment.
  - **Range Filters**:
    - Faster performance compared to discrete dropdown lists because it avoids querying the entire data to create a unique list; converting fields to a measure can enable this.
  - **Wildcard and Multiple Value Custom Lists**:
    - Offers better performance by allowing users to search and find values themselves without querying the entire dataset.
  - **Using Only Relevant Values cautiously**:
    - Useful but can slow down performance when many filters are applied as it references other filters in the dashboard.

- **Practical Application in Tableau Desktop**:
  
  - **Best Practices**:
    - Customize filters at the dashboard level, not the worksheet, to ensure the changes are applied to the dashboard.
  - **Adding Apply Button**:
    - Facilitates easier interaction for users with the dashboard by holding the actions until selections are made.
  - **Setting up Multiple Value Custom Lists**:
    - Preferable to wildcards as it shows all matched results, allowing users to pick the right option.
    - Wildcards are performant but don’t show the matching results, which can be a drawback.
  - **Avoiding 'Only Relevant Values' for search functionalities**:
    - For search functionalities, using 'all values in database' is recommended as it doesn’t restrict the values displayed, offering more freedom for users.

*Note*: The application part involves working in the Tableau Desktop Performance Filter Optimization Workbook and saving changes to facilitate further deep dives into filtering dates in upcoming lessons. Adjustments were made to enhance the user experience by optimizing filter functionalities, emphasizing the utility of multiple value custom lists and the proper use of 'Only Relevant Values'.

### Date Filtering

- **Date Filters in Tableau**
  
  - **Types and performances**
    
    - **Relative date filters**
      - Mid-performance level.
      - Enhances user experience by allowing dynamic history tracking without data manipulation.
      - Highly customizable for the end-users.
        
    - **Range of date filters**
      - Fastest performance due to continuous date range.
      - Utilizes min and max function.
      - Usability is moderate; controlling specific dates and sliders can be cumbersome.
        
    - **Discrete date filters**
      - Worst performance.
      - Creates distinct lists in dropdowns which affects performance.
      - Preferably avoid using this filter.
        
  - **Performance differentiators**
    - Using **date truncation** is faster compared to date parts for querying date-related data.
    - **Date part functions** are resource-intensive especially with date partitioned databases.
    - Extract data and materialize calculations when using date part functions to avoid recalculation.
  
- **Practical Application**
  - Modified filters in Tableau Desktop Performance Filter Optimization Workbook.
  - Changed year of date filter to a more efficient relative date filter anchored to a specific date.
  - Ensured the filter applied to all necessary worksheets.
  - Improved dashboard by revisiting and amending filter settings, targeting a more streamlined and performant dashboard.

*Note*: The hands-on modification part involves working on Tableau Desktop applying the mentioned strategies to improve dashboard's performance, with a focus on optimizing date filters. The hands-on part details the actions step by step, explaining the changes made in the filter settings to enhance dashboard performance. It also addresses some glitches that might occur and how to resolve them, preparing for the next lesson on filter actions and their impacts on performance.

### Filter Actions

- **Filter Actions in Tableau Desktop**:

  - **Definition and Benefits**:
    - Offer dynamic alternative to static dropdowns using existing dimensions in dashboard sheets.
    - Faster and do not add to rendering or processing load.
  - **Integration and Tuning**:
    - Need to be finely tuned for optimal performance.
    - Offer a variety of options with different functionality-performance trade-offs.

  - **Components and Recommendations**:
    
    - **Source Sheets**:
      - Sheets where action originates; advisable to choose a single source sheet per action.
    - **Run Action On**:
      - Trigger behavior: selecting, selecting via a menu, or hovering (not recommended).
    - **Target Sheets**:
      - Sheets impacted by the action; to maintain efficiency, limit the impacted sheets and follow a logical path (like a Z-pattern).
    - **Clearing Selection**:
      - “Show all values” is default but least performant; consider "keep filtered values" or "exclude all values" for better performance.
    - **Target Filter Section**:
      - Define the fields leveraged in the filter action; recommended to use “selected fields” for better control and performance.

  - **Pro Tips**:
    - Use "exclude all values" for clearing a selection to create a show-hide functionality and improve performance.
    - Customize selected fields through “Add filter” option for finer control.

- **Practical Demonstration in Tableau Desktop**:
  
  - **Setting Up**:
    - In the “Performance Filter Optimization” workbook, clean up existing filter actions before adding new ones.
  - **Editing Existing Actions**:
    - Review each existing filter action, renaming and setting appropriate source and target sheets.
    - Set filter criteria (fields to push) precisely using "selected fields" option to prevent performance issues.
  - **Adding New Action**:
    - Create a "detail table hidden view" sheet for detailed data, which will be hidden initially for performance efficiency.
    - Configure this new sheet to appear only under certain filter conditions, enhancing dashboard efficiency.
    - Use logical names for actions to reflect their functionality clearly.
   
_Note: Tutorial details setting up and optimizing filter actions in a Tableau Desktop dashboard, emphasizing efficient setting up of action triggers, sources, targets, and filter settings for better dashboard performance and user experience._

### Parameter & Set Actions

In this Tableau Desktop online course segment, the topic of enhancing workbook performance using parameter and set actions as filter alternatives was discussed. Below are the main points:

- **Parameter and set actions**: Created from the same menu as filter actions but offer improved efficiency and versatility in affecting calculations, filters, and marks due to their integration into SQL and Tableau's Order of Operations.
  
- **Creation and limitation**:
  - Need to establish based sets and parameters before creating actions.
  - Parameter actions are single-select only, not accepting multiple values.
       
- **Creating and applying a set action**:
  - A set action titled "year set" was developed to apply filters more efficiently.
  - The set action was created using the "year" field and integrated into the dashboard as a floating element, positioned temporarily in the top right corner.
  - The "change set values" option was utilized to establish the set action, defining the "year set" as the source sheet and selecting the relevant data source and set.
  - The set action was then applied as a filter to the map sheet, avoiding application to the "year set" sheet to prevent confusion.
  - The setup enables end users on the main dashboard to swiftly select between two available years in the dataset, offering a faster alternative to traditional filters and dropdowns.

Ensure to save your progress to maintain the new functionalities added to your workbook for user-friendly and efficient operations. This setup aims to enhance the speed and efficiency of selecting different years in the dataset compared to using regular dropdown or filter actions.

### Performance Impact - Filter Optimization

In this section of the Tableau Desktop online course, the focus is on reviewing the progress made in filter optimization and its impact on workbook performance. Here are the main points:

- **Performance Improvement**:
  - Previous testing times: 24-28 seconds
  - Current testing times: 18-20 seconds
  - Result: 6-10 seconds improvement, equating to around 25% enhancement.
  - Expectation: Continued progress in the upcoming sections on calculations and visualizations.
    
- **Strategies Employed**:
  - Removal of unnecessary filters, particularly those with lengthy lists.
  - Transitioning filters to multiple value custom lists.
  - Eradicating relevant value conditions.
  - Streamlining filter actions and utilizing set actions.
    
- **Impact on Event Type Ranking**:
  - Significant reduction in query compiling issues, a primary concern in the raw aggregated data, through filter optimization.
  - Noticeable decline in individual query and rendering times, despite the bars appearing largely unchanged in performance recordings.

This segment highlights the notable advancements achieved in reducing the workbook's response time through effective filter optimization strategies, with a promise of further improvements in subsequent sections tackling calculations and visualizations.

## Calculation Optimization

### Intro to Calculation Optimization

In this segment of the Tableau Desktop online course, the discussion moves on to the optimization techniques for calculations with a focus on enhancing the performance of various components. Here are the primary objectives and topics that will be covered:

- **Reviewing Common Calculation Types**:
  - Row-level functions
  - Aggregators
  - Table calculations
  - Level of Detail (LoD) expressions
    
- **Performance Optimization Tips**:
  - Strategies for optimizing aggregation and table calculations
    
- **Syntax Optimization**:
  - Maximizing efficiency through optimal syntax for conditional or logical calculations
    
- **Utilizing Calculated Groups or Sets**:
  - Leveraging these for live connections to improve performance

The goal is to empower participants with knowledge and tips to optimize calculation processes, contributing to a more efficient use of Tableau Desktop for data analytics.

### Calculation Types

In this portion of your Tableau Desktop online course, you are guided through the various levels where calculations can be applied in Tableau, each varying in functionality and performance. Here is a summary:

- **Row Level Calculations**:
  - Happen at the lowest level in the data source.
  - Generally involve string or mathematical computations.
  - Big opportunities exist for optimization in this area as these calculations can be pushed back to the database, reducing Tableau's processing load.
   
- **Aggregate Calculations**:
  - Roll up to the level of detail of the view and use aggregate functions such as sum, average, etc.
  - The upcoming part of the course will delve deeper into this.

- **Table Calculations**:
  - Materialize after a view has been rendered, posing a challenge for optimization.
  - Examples include rank difference and running total.
  - Optimization strategies for this type will be discussed in future lessons.

- **Level of Detail (LoD) Calculations**:
  - Allow control over the level of detail applied within a calculation, and can either ignore or include additional detail from what is in the view.
  - Potent yet can cause issues if misused.

In the forthcoming section, the focus will be on exploring aggregate calculations in greater depth. The intent is to enhance understanding of the complexity and potential of Tableau's calculation functionalities to foster efficient and effective data analysis.

### Aggregation

In this segment of your Tableau Desktop online course, the focus is on understanding and implementing aggregation in calculations effectively to optimize performance. Here is an insightful summary:

- **Aggregation Types**:
  
  - **Undefined aggregation**:
    - Doesn't specify the type of aggregation used, forcing Tableau to perform logical checks at each row level in your calculation.
    - Can affect performance adversely especially in complex views with many measures.
    - Illustration: sales, quantity, and discount referencing the row level records in a given view without wrapping an aggregation around metrics.
  - **Defined aggregation**:
    - Places the aggregation inside your calculation, simplifying logical checks as they are performed post aggregation.
    - Allows multiple types of aggregations for measures called out inside that calculation.
    - Facilitates logical checks at an aggregated level, thus enhancing efficiency.
    - Pro tip: Utilizing regular aggregation functions like Min and Max can be more efficient than average and attribute functions.

- **Hands-on with Aggregation in Tableau**:
  
  - **Workbook Preparation**:
    - Save the current workbook as a new file named "Calculation Optimization" to track the changes made during this course segment.
  - **Optimizing Existing Multi-Measure Calculation**:
    - Initially, the multi-measure in the data tab lacked defined aggregation, causing logical checks at the row level.
    - Strategy: Define aggregations up front and wrap each field in a sum, ensuring a uniform type of aggregation to avoid errors.
    - Post modification: The field changes to "agg" indicating an internal defined aggregation and requires re-dragging into the view to replace the red pill error.

- **Final Checks**:
  - Ensured that the modified multi-measure field works without errors in different sheets of the dashboard.
  - Important to rectify opaque sheets which indicate errors by locating and replacing the problematic pill.

As you proceed, remember that understanding and implementing aggregation correctly is key to optimizing the performance of your Tableau workbooks. This hands-on approach will help in grasping the nuances of aggregation in Tableau.

### Level of Detail Expressions

In this section of the Tableau Desktop online course, you are guided on how to utilize level of detail (LoD) expressions to control the granularity of your calculations. Here is a summary:

- **Understanding LoD Expressions**:
  - Allow control over the granularity of calculations.
  - Can be an alternative to other calculation types.
  - Essential to understand the data and the grain of the source being utilized in your view.

- **Decision Making for Calculation Types**:
  - **Question 1**: Does the question require ranking, recursion, moving calculations, or inter-row calculations?
    - **Yes**: Use table calculations.
    - **No**: Move to the next question.
  - **Question 2**: Is all the necessary data present in the view for your calculations?
    - **Yes**: You can leverage table calculations.
    - **No**: Proceed to the final question.
  - **Question 3**: Does the granularity of the question match the view's granularity?
    - **Yes**: Opt for basic mathematical or logical calculations, preferably pushing them back to the data source.
    - **No**: LoD calculations would be the better option as they control grain irrespective of the view presented.

- **Utilizing LoD Calculations**:
  - Can replace table and basic calculations when required.
  - Often more efficient with well-designed data sources using logical tables.

- **Performance Evaluation**:
  - **Testing**: The optimal approach is to test various calculation types and assess the performance outcomes.
  - **Variables**: The efficiency of LoD calculations can depend on factors such as:
    - Source type (live or extract connection).
    - Calculation logic being employed.
    - Complexity of the view where the calculation is brought out to.

Remember to take into account the specific circumstances of your data source and the complexity of your view while choosing between LoD and other types of calculations. It encourages a hands-on approach of testing different methods to find the most efficient solution.

### Table Calculations

In this segment of your Tableau Desktop online course, the focus is on optimizing table calculation performance in your workbook, specifically in larger or highly detailed views. Here’s a detailed summary of this part:

- **Table Calculations in Tableau**:
  - Performed at the view level and can slow down workbook performance, especially in detailed or complex views.
  - Table calculations work harder as view complexity increases.

- **Alternatives to Table Calculations**:
  
  - **Data Aggregation**:
    - Conducted inside the data source to remove the need for table calculations.
    - Involves removing unnecessary columns and aggregating visible dimensions.
  - **Database Level Views**:
    - Creating a view or table at the database level can mimic the level of detail required for your calculations, similar to using extracts but at the database level.
    - Not suitable for all scenarios, especially when retaining detailed data is necessary for other dashboard parts.

- **Utilization of Level of Detail (LoD) Expressions**:
  
  - Control the grain at which calculations are processed.
  - Allow users to choose the level a calculation operates at irrespective of the view construction.
  - Require testing and performance analysis to weigh the pros and cons against table calculations.

- **Performance Optimization**:
  - Reduce table calculation complexity before seeking alternatives, generally by simplifying your view and aggregating to higher levels.

- **Practical Application**:
  
  - **Activity in Tableau Desktop**:
    - Analyzing and optimizing table calculations in a Tableau Desktop Performance Calculation Optimization workbook.
    - Involves modifying, replacing, or removing elements to enhance efficiency and suitability for end use.
  - **Steps**:
    - Identifying inefficient table calculations.
    - Replacing an existing table calculation with a more efficient LoD expression.
    - Creating a new calculated field for total persons injured by borough using fixed LoD on borough with a sum aggregation.
    - Reformatting views and removing unnecessary table calculations for efficiency.

The session ends with a return to the 'start here' point, saving the workbook, and prepping for a deeper dive into conditional calculations in the next part. The hands-on approach in Tableau Desktop serves to foster better understanding and efficiency in optimizing workbook performances, emphasizing practical experience over theoretical knowledge.

### Conditional Calculations

In this section of the Tableau Desktop online course, the topic revolves around optimizing conditional calculations to achieve the best performance. Here is a streamlined summary of the essential information:

- **Organization of Conditional Calculations**:
  - Order them based on the most common outcomes first to maximize efficiency.
  - Tableau processes the calculation logic until a match is found — organizing with the highest frequency matches first allows for quicker data processing and eliminates records for subsequent logic parts, returning fewer values.

- **Optimizing Queries for Best Performance**:
  - Start with a null check in your conditional calculation.
  - Order the conditional statements according to the occurrence rate of each dimension option to facilitate optimal query performance.
  - Utilize a separate sheet to lay out the dimensions and get a grasp of the option frequencies, helping to better structure the conditional calculation from the highest to the lowest frequency, pulling out larger data chunks first.

- **Pro Tips for Faster Conditional Calculations**:
  - Using "else if" without a space is quicker than with a space, as it generates less complex logical tests.
  - The "in" function operates faster than several "or" functions in the conditional calculations, promoting quicker execution.

- **Practical Application in Workbook**:
  - Transitioning to hands-on application, you're guided to enter the workbook to refine some existing calculations.

Understanding the fundamental strategies for organizing and optimizing conditional calculations is crucial in leveraging Tableau effectively. The session aims to assist learners in enhancing the speed and efficiency of their Tableau operations through well-structured conditional calculations, with a hands-on approach to deepen understanding and application in real-world scenarios.

### Calculation Groups

This segment of your Tableau Desktop online course deals with enhancing the performance of live connections through different grouping strategies. Here is the summary:

- **Grouping Strategies**:
  
  - **Native Grouping**:
    - Best for well-structured data sources with good relationships and extract connections.
    - Generally offers faster performance compared to other alternatives.

  - **Live Connections**:
    - **Case Statements**:
      - A straightforward alternative to native grouping.
      - Can perform better in some scenarios if appropriately ordered.
    - **Sets**:
      - Ideal for creating conditional groups or addressing special use cases.
      - Allows for faster and more flexible operations in filters, calculations, etc.
      - Generally processed earlier by Tableau, enhancing dashboard performance.

- **Benefits of Using Sets**:
  
  - **Performance**:
    - Executed early in Tableau’s order of operations, aiding quicker data filtering.
    - Foster quicker processing of subsequent calculations and filters.
    - Creates more performant SQL queries compared to other grouping methods.
  - **Functionality**:
    - Facilitates conditional thresholds not available in native grouping.
    - Can embed other conditional logic and reference measure values.

- **Limitations of Sets**:
  - Not suitable for all scenarios due to usability restrictions.
  - Traditional filters might offer more functionalities in certain aspects, though set controls have bridged the gap significantly.

- **Next Steps**:
  - Future discussions will leverage sets to enhance calculated groups further.
  - The upcoming section will address other common issues in calculation optimization.

The section underlines the necessity to test various grouping strategies against each other due to the distinct characteristics of different data sources, workbooks, and use cases. It provides an in-depth understanding of grouping functionalities, highlighting the advantages of utilizing sets for optimized performance, albeit noting their limitations.

### Common Pain Points

In this part of your Tableau Desktop online course, the focus is on averting common pitfalls related to calculation optimization and offering alternatives for a more efficient workflow. Here's the summarized version:

- **Common Pain Points in Calculation Optimization**:
  - **Blended Calculations**:
    - Issue: Requires multiple queries from at least two data sources, affecting performance and limiting query optimization.
    - Solution: Utilize Tableau's logical relationships model for situational source joining, enabling query fusion and parallel processing.

  - **String Manipulation**:
    - Issue: Resource intensive when using functions like left split and regex.
    - Solution: Perform these calculations at the database level, provided you have the necessary business logic.

  - **Parameters in Calculations**:
    - Issue: Cannot be materialized inside calculations, forcing Tableau to calculate them each time the workbook is opened.
    - Solution: Separate calculations to distinguish between materializable and non-materializable components, reducing the load on parameter-free calculations.

  - **External Services**:
    - Issue: Slower response times due to reliance on off-platform technologies.
    - Solution: Leverage Tableau's in-built features, which now incorporate many functionalities previously found in external platforms.

- **Practical Application**:
  - **Task**: To optimize a calculation identifying drug and alcohol-related accidents.
  - **Issue**: The existing calculation uses regular expressions, which is considered overkill.
  - **Solution**:
    - Create a set named "drugs and alcohol" including 'alcohol involvement' and 'drugs illegal' criteria.
    - Apply this set as a filter, eliminating the need for the previous regular expressions and enhancing efficiency.

By focusing on Tableau's advanced features and shifting certain functions back to the database, the session demonstrates how to improve the efficiency of different calculations significantly. It proposes solutions to several common issues, emphasizing a more optimized approach to handling blended calculations, string manipulations, parameters in calculations, and the use of external services. It practically illustrates this by optimizing a calculation in the Tableau workbook, showcasing a more efficient solution using sets over regular expressions.

### Performance Impact - Calculations Optimization

In this segment of your Tableau Desktop online course, you scrutinized the impacts of calculation optimization on performance. Here are the pertinent points:

- **Performance Impact Analysis**:
  - **Prior performance**: The filtering section had runtimes falling in the 18-20 seconds range.
  - **Current performance**: With the calculation optimization measures implemented, the runtimes improved, registering between 14 and 18 seconds - a total enhancement ranging from 2 to 6 seconds.

- **Calculation Optimization Approaches**:
  - Replaced regular expression string calculations.
  - Defined aggregation within calculations.
  - Switched table calculations with Level of Detail (LoD) expressions.
  - Reordered logical formula syntax based on frequency.

- **Analysis of Event Type Ranking**:
  - Observations were made on the raw aggregated form, which showed a reorganization of the top events:
    - A decrease in rendering times.
    - An increase in the executing query events.

This section illustrates that calculation optimization techniques can lead to notable improvements in performance, anticipating potential further enhancements in the forthcoming visuals segment of the course. The improvements are evidenced by a reduction in the runtime in workbook performance tests. The techniques employed in optimizing the calculations, including adopting more efficient strategies for handling expressions and aggregations, had a positive effect, which is reflected in the event type ranking shifts with a decrease in rendering times and a rise in executing query events.

## Layout & Visuals Optimizations

### Intro to Layout & Visual Optimization

In this part of the Tableau Desktop online course, the focus is on optimizing layout and visuals to enhance speed and performance. Here are the objectives and the main elements to be explored:

- **Understanding Performance Impacts**:
  - **Sheet and Mark Counts**: Learn the effects of varying the counts of sheets and marks on the performance.
  - **Pages and Animations**: Delve into how the utilization of pages and animations can affect the workbook’s performance.
  
- **Techniques and Tools**:
  - **Geospatial Mapping**: Understand and apply the techniques for geospatial mapping and layering to potentially enhance performance.
  - **Tooltips**:
    - **Simplification**: Learn how to simplify tooltips to optimize performance.
    - **Efficient Utilization**: Get to know the ways to use tooltips efficiently to aid in optimization.

- **Workbook Configurations**:
  - **Properties and Objects**: Figure out how configuring various workbook properties and objects can have implications on performance.

- **User Experience (UX)**:
  - **Dashboard Layout**: Discover common UX tips to facilitate smooth dashboard layout and navigation.

Through this section, the intention is to help you gain a comprehensive understanding of different facets of layout and visual optimization, equipping you with knowledge on how to leverage various features and settings to improve the speed and overall performance of your Tableau workbooks.

### Mark & Sheet Counts

Pending

### Mapping Options

 In this section, you are advised on how to optimize the use of mapping functionalities in Tableau to enhance performance. Key takeaways include:

- **Map Types**:
  - **Symbol Maps**: Faster as they only produce circles at the central point of the regions depicted.
  - **Filled Maps**: Slower compared to symbol maps as they involve filling entire areas, resulting in more marks.

- **Custom Territories**:
  - **High-Grain Geospatial Data**: Encourages using the highest grain geospatial data that meets your needs to build custom territories to avoid unnecessary processing of lower grain data layers.

- **Layering**:
  - **Dual Axis**: Notes that layering performance threshold is similar to dual axis, and the difference in swapping them is negligible.
  - **Limit Layers**: Advises limiting the number of layers to aid performance.

- **Practical Application**:
  - **Case Example**: In the ongoing workbook, filled maps were chosen over symbol maps despite being generally slower. This was done to remove thousands of marks from symbol maps, moving the detail level up to the zip level, thereby enhancing performance noticeably.

This segment emphasizes being judicious in the use of filled maps, constructing custom territories with appropriate data grain, and being restrained with layering to boost the overall performance while working with maps in Tableau. It underlines that practical performance improvements might sometimes go against general guidelines, illustrated by the choice of filled maps in the workbook.

### Tooltips

In this section, the focal point is optimizing tooltips in Tableau for better performance and user experience, here are the salient points:

- **Tooltips Optimization**:
  - **Simplicity**: Encouraged to keep tooltips straightforward by limiting the number of complex measures and utilizing basic visuals to aid users.
  - **Filter Actions**: Utilize filter actions to refine visualization and tooltip filtering to enhance performance.
  
- **Working with Tableau Desktop**:
  - **Tooltip Cleanup**: Existing tooltips in the workbook were simplified; a vision tooltip was removed for being too complex and hard to render.
  - **Adding Visuals**: A simple visual was added to the map to offer insights into factors contributing to incidents by zip code, using a custom color spectrum in a bar chart and ensuring labels are displayed clearly.
  - **Preview and Adjustment**: The tooltip was previewed and adjusted for width and height to avoid a crowded appearance.
  - **Final Touches**:
    - **Data Filtering**: To enhance readability, a filter was applied to show only records with at least one injury, eliminating irrelevant zero values.
    - **User Experience**: Emphasized keeping tooltips simple and minimalistic to not detract from the main view and to avoid unnecessary rendering or processing time.

This section guides on balancing detail and performance while working with tooltips, emphasizing simplicity and the strategic use of filter actions to maintain a user-friendly experience without compromising on the essential details in Tableau Desktop.

### Pages

In this section, the discussion centers around the cautious and informed use of pages in Tableau to enhance presentation delivery without compromising performance. Here are the key points:

- **Using Pages Effectively**:
  - **Dimension Selection**: When selecting dimensions for the pages shelf, avoid using those with a large number of unique values since they query all data values simultaneously, not individually as each page loads. 
  - **Playback Speed**: Utilize the fastest playback speed to create an illusion of a quicker pace and heightened performance, fostering a perception of a more performant dashboard.

- **Testing Dimensions for Pages Shelf**:
  - **Pro Tip**: Before deciding on a dimension for the pages shelf, test it by placing it on the level of detail of the view to assess the rendering time. The goal is to avoid slow rendering times which occur when executing queries on all possible dimensions from a specific field.
  
- **Case in Point - Our Dashboard**:
  - **Enhancements**: The “injuries by month” sheet previously had the pages feature enabled, which hindered performance significantly. A set action was introduced to replace the year pages, offering a more intuitive and performant solution, thus optimizing the workbook.

The section advises on the prudent use of pages in Tableau, emphasizing the careful selection of dimensions and playback speed to improve performance perception, and recommending testing dimensions in the level of detail view to avoid potential slow-downs. It also illustrates the application of these tips in optimizing a specific dashboard.

### Dashboard Properties

 In this section, the topic of discussion is optimizing dashboard properties in Tableau to ensure efficient caching and rendering of dashboards. Here are the pertinent details:

- **Optimizing Dashboard Properties**:
  - **Device-Specific Views**:
    - **Issue**: Creating different designer profiles for various devices (desktop, mobile, and tablet) causes Tableau to constantly reassess screen size, hindering caching.
    - **Recommendation**: Utilize fixed sizing on Tableau Server (and to a lesser degree on Tableau Desktop) to assist Tableau in rendering dashboards more efficiently without wasting time determining the appropriate dashboard size for varying screen sizes.
  - **Fixed Sizing**:
    - **Advantage**: Helps in specifying the exact dashboard dimensions, thus facilitating quicker rendering.
    - **Planning**: Requires pre-planning and acceptance testing with business users but significantly simplifies the dashboard size and caching process.

This segment provides guidance on improving the Tableau dashboard's efficiency by modifying properties, with a focus on reducing Tableau's workload during the rendering process using fixed sizing, and setting a dashboard size that accommodates the majority of users, setting the ground for further optimization in upcoming lessons.

### Dashboard Objects

In this segment, the discussion revolves around optimizing the dashboard objects in Tableau to enhance performance and improve the visual appeal. Here are the key aspects covered:

- **Dashboard Object Optimization**:
  - **Objective**: To enhance performance by reducing, consolidating, or limiting the dashboard objects like images or text boxes.
  - **Rules**:
    - **Necessity**: Use only necessary objects.
    - **Reduction**: Minimize the size of objects and image files to limit the compute time required for layout and rendering.
    - **Consolidation**: Migrate objects into existing sheets or consolidate them into a single object to reduce overall compute time and impact.
    - **Tip**: Using the floating option for dashboard objects can offer better cache and render efficiency compared to the tiled option.

This section details the procedures to optimize dashboard objects, primarily emphasizing the reduction of unnecessary objects and utilizing the floating option for better efficiency. The process outlined here forms a meticulous guide to adjusting the layout through precise positioning of objects and sheets, enhancing both functionality and aesthetics. It underscores the importance of making calculated decisions in object utilization to facilitate improved performance and user experience. It sets a robust ground for building a streamlined and visually attractive dashboard by utilizing optimized objects and layout configurations.

### User Experience Tips

In this segment, tips are provided to enhance the user experience in dashboard usability and design in Tableau. Here are the main points:

- **Improving User Experience**:
  - **Objective**: Boost perceived performance and overall user satisfaction.
  - **Benefit**: Though it may not significantly increase performance, it can enhance the customer's perception of the dashboard.

- **User Experience Tips**:
  - **Common Reading Patterns**:
    - **Approach**: Use a drill pattern, initiating with high-level dimensional views and then progressing to detailed data.
    - **Layout**: Adhere to a specific pattern that navigates from the top left to the top right, then bottom left, and finally bottom right.
    - **Goal**: Facilitate insightful actions and informed business decisions through structured data presentation.
      
  - **Hiding Filter Menus**:
    - **Placement**: Ensure the filters are well-placed and only visible when required.
    - **Technique**: Utilize containers with buttons to conceal the filter menus, a strategy commonly used in web pages.
      
  - **Sheet Management**:
    - **Hiding and Swapping**: Leverage parameters, filters, and actions to control the visibility of sheets, improving performance and enabling detailed data view options.
    - **Benefit**: Enhances performance by limiting initial rendering while offering depth in data visualization.
      
  - **User-Friendly Navigation**:
    - **Strategy**: Segregate dashboards into various tabs to manage an excess of data views.
    - **Advantage**: Facilitates the grouping of similar sheets and themes, enhancing performance through limited dashboard views.
      
  - **Purposeful Animation**:
    - **Usage**: Incorporate animations sparingly and only when it adds value to the user experience.
    - **Speed**: Favor fast animations to avoid giving the impression of slow performance.

The discussion revolves around user experience optimization in dashboard design, emphasizing the strategic use of layout patterns, effective management of filter menus and sheets, and the judicious use of animations. The aim is to enhance the perception of the dashboard, fostering user satisfaction and facilitating informed business decisions through a streamlined and intuitive navigation structure. The suggestions provided form a holistic approach to optimizing user interaction with the dashboard, promoting a blend of aesthetics and efficiency in design.

### Performances Impact - Layout & Visual Optimization

During the recent evaluation of the workbook, a substantial improvement was observed in the calculation section. Here are the key findings and changes implemented:

- **Performance Metrics**:
  - **Before**: The calculation section's testing time ranged between 14 and 18 seconds.
  - **After**: Performance testing runtimes were notably reduced to a range of 3 to 5 seconds.
  - **Improvement**: This reflects an enhancement in speed varying between 9 to 15 seconds, a significant upgrade in efficiency.

- **Identified Cause of Previous Delays**:
  - **Main Factors**: It was discerned that the prime contributors to the earlier performance lag were the levels of the sheets, marks, and objects utilized in the dashboard.

- **Implemented Enhancements**:
  - **Marks**: The number of marks on all sheets was lessened.
  - **Objects**:
    - **Reduction**: The count of dashboard objects, such as containers and images, was minimized.
    - **Floating**: A strategy of using floating dashboard objects and sheets was adopted for better performance.
  - **Sizing**: The dashboard size was fixed to optimize layout.
  - **Device Designer**: The layouts stemming from the device designer were eliminated.

- **Results on Event Type Ranking**:
  - **Reduction**: There has been a large decrease in various account metrics, markedly in the areas of rendering and query execution.

By addressing the principal factors causing delays previously, notably the sheets, marks, and objects in the dashboard, significant improvements were achieved. The measures involved optimizing visual elements and restructuring the layout, resulting in markedly enhanced performance with faster rendering and query execution. The outcome is a more streamlined and efficient dashboard, evidenced by the substantial reduction in testing runtimes.

## Tableau Server & Online Optimizations

### Intro to Server & Online

In this segment, we delve into performance aspects exclusive to Tableau Server and online, paying particular attention to:

- **Data Sources**:
  - **Embedded vs. Published**: Analyzing and contrasting the performance of these two types of data sources on Tableau Server.
  
- **Caching**:
  - **Introduction**: Familiarizing with caching and cache warming techniques.
  - **Cache Warming**: Learning techniques to preload dashboard content, facilitating quicker access and improved efficiency.

- **Rendering**:
  - **Client vs. Server Side**: Gaining an understanding of the different rendering methods.
  - **Application**: Understanding the appropriate circumstances under which each rendering method should be applied.

The goal is to furnish you with the knowledge and tools to optimize performance leveraging the functionalities and features of Tableau Server and online platforms.

### Embedded vs Published Sources

In this section, we delve into the distinctions between embedded and published data sources and how they influence performance and usability in Tableau:

- **Embedded Data Sources**:
  - **Speed**: Generally operate faster due to materialized calculations and rapid data transfer.
  - **Individualized**: Specifically tailored to individual workbooks, hence minimizing communication time.
  - **Limitation**: Not shareable among various workbooks on the Tableau server, leading potentially to data source proliferation.
  
- **Published Data Sources**:
  - **Shareability**: Can be shared across multiple workbooks on the Tableau server, promoting a unified source of truth and preventing proliferation.
  - **Slow Performance**: Have slower operational speeds due to additional communication time required between the data source and the workbook.
  - **Beneficial in Cases**: If the performance lag is minimal, utilizing a shared data source might be more beneficial, fostering efficiency and consistency.

- **Considerations for Choice**:
  - **Balancing Act**: Requires careful balancing between the swiftness of embedded sources and the consolidated truth offered by published sources.
  - **Holistic Approach**: Consider the broader implications including the importance of the dashboard, the number of users, and potential benefits in the context of the performance difference.
  - **Prudent Decision**: It is pivotal to wisely evaluate the performance disparities before deciding on the route to take to ensure optimal results.

Understanding the nuances of these data sources will guide you in making an informed decision on the best approach for your specific needs in Tableau.

### Dashboard Caching

In this section, we are focusing on the function and optimization of caching in Tableau, mainly concerning Tableau Server:

- **Caching Overview**:
  - **Definition**: Caching is the process of preloading a dashboard view to facilitate faster load times in future accesses.
  - **Platforms**: It is available on both Tableau desktop and server, with a stronger emphasis on server due to the higher user interaction on that platform.

- **Setting Up Caching**:
  - **Administrator Role**: Collaborate with an administrator to activate caching.
  - **Refresh Rate**: Set up caching to refresh less frequently to enhance resource utilization and maintain an active cache for a more extended period for users.

- **Limitations of Caching**:
  - **Dashboard Updates**: It is less effective for dashboards that undergo multiple updates daily.
  - **Individual User Cache**: Clearing the cache on an individual's Tableau desktop doesn't affect the cache status for other users.
  - **Cache Clearing**:
    - **Desktop**: It is essential to clear the cache when doing performance recording; this can be done by closing all local workbooks.
    - **Server**: On the Tableau server, clicking the refresh icon clears the local cache, but not for other users engaging with the dashboard.

### Cache Warming

In this part of the course, we explore the concept of "cache warming" and its applications in Tableau Server:

- **Definition**:
  - **Cache Warming**: It refers to preloading dashboard views on Tableau Server to facilitate quicker access when users eventually view them.

- **Methods**:
  - **Subscriptions**:
    - **Operation**: Set up to run post data update but before dashboard view by end users, it triggers the caching process.
    - **Benefits**: Avoids the necessity for local server admins to make server alterations and imitates a user initializing the cache by viewing the dashboard.
  - **Data Acceleration**:
    - **Tools**: Can be initiated through Python utilities or Tableau's Rest API.
    - **Considerations**: Admins should assess the repercussions carefully as it diverts server resources from regular functions to complete the caching.
    - **Effectiveness**: Though a more detailed approach compared to subscriptions, it is efficient in warming the cache.

- **What's Coming Up**:
  - The subsequent section will evaluate client and server side rendering, probing their distinctions and applicable circumstances.

### Client vs Server - Side Rendering

In this segment, the intricacies of rendering on Tableau Server are discussed, focusing on the two primary rendering methods - server-side and client-side:

- **Rendering Types**:
  - **Server-side Rendering**:
    - **When Used**: For high complexity dashboards, around a complexity score of 120.
    - **How it Works**: The server renders the dashboard and sends it as an image to the client device, which can be a mobile or a desktop.
    - **Pros**: Faster performance for complex views.
    - **Cons**: Offers a less flexible dashboard experience.
      
  - **Client-side Rendering**:
    - **When Used**: For low complexity dashboards, typically with a score of 80 or less.
    - **How it Works**: The dashboard is rendered directly on the client's browser or computer, enabling functionalities like tooltips and highlighting.
    - **Pros**: Retains Tableau functionalities and tools.
    - **Device Thresholds**: Browsers have a default threshold of 100, while mobile devices have a lower threshold of 40, hence using server-side rendering more often.

- **Customization and Testing**:
  - **Admin Controls**: Server admins can adjust the rendering thresholds for different devices.
  - **Testing**: Individuals can test different rendering thresholds using specific URLs that include the render parameter followed by desired threshold values.
  - **Custom URLs**: Users can be provided with custom URLs that specify a rendering method (server or client-side) optimized for their use, enhancing their experience.

- **Implication**:
  - **Awareness**: Understanding the nuances of these rendering methods is pivotal in developing dashboards, helping to align the rendering approach with the dashboard's complexity and the device specifications for optimal performance.

In the upcoming steps of the course, leverage this knowledge to optimize the performance of your dashboards in Tableau Server effectively.

## Wrapping Up

### Key Performance Takeways

![[Screenshot 2023-09-10 at 9.59.54 PM.png]]