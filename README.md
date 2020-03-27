<h1>RPA Developer Advanced Certification - Exam #5</h1>

In this exercise, you will create a UiPath automation that performs the steps below. To achieve this, you will use the REFrameWork as the starting template and follow the UiPath development best practices.

Here are the steps performed by the Robot:
<p>1. Log in to https://www.acme-test.com.</p>
<p>2. On the landing page, Dashboard, click on the Work items menu item. Scrape the data in all the pages of the table, page by page, ensuring error handling and recovery.</p>
<p>3. For each page:</p>
<ul><li>Filter the records where Status is 'Open';</li></ul>
<ul><li>Filter the records where Type is 'WI1';</li></ul>
<ul><li>Filter the records where WIID is greater than 200000;</li></ul>
<ul><li>Append the resulting datatable into an Excel worksheet, you shouldn't worry about the headers and format of the output file.</ul></li>

Constraints to follow in the development, using the REFrameWork:<br>
<br>1.TransactionItem datatype should be a String. The process should recover and retry in case of errors in navigation between WorkItems page. One transaction is the action of scraping one web page. By navigating to the next page, the next transaction will execute. (Same as ACME Process 4 Dispatcher from the UiPath Academy). 
<br>2. Create a separate workflow file for the Login to ACME. File input arguments: URL ; Username ; Password. Create a separate workflow file for closing ACME. 
<br>3. Add the ACME_URL and ACME_Credential to the Config file. 
<br>4. Populate InitAllApplications.xaml from the Framework folder with Invoking the Login to ACME and navigation to the Work Items. 
<br>5. Populate CloseAllApplications.xaml from the Framework folder with Invoking the Close ACME. 
<br>6. Populate KillAllProcesses.xaml from the Framework folder with killing the process used. 
<br>7. Populate the Process.xaml file with the following actions: Web scraping, Filtering and Appending to Excel.

<strong>Important Note:</strong> Don't use external file references outside of the project folder (including Orchestrator Assets). Place all the used files within the project folder, zip that folder and upload it to the UiPath Certification Platform.

Zip <strong>ALL</strong> the used workflow files <strong>AND</strong> the output Excel file. Then upload the .zip file to the UiPath Certification Platform.

Good luck!
