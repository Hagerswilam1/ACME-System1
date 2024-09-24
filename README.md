<h1>ACME System1 Automation Library</h1>
<p>This UiPath library automates interactions with the ACME System1 website. It handles various operations such as logging in and out, navigating to work items, extracting and updating work item details, and updating the comment and status of each work item. This library can serve as a reusable component for automating workflows related to the ACME System1 website.</p>

<h2>Features</h2>
<ul>
    <li>Login and logout from the ACME System1 website</li>
    <li>Navigate to the Work Items page</li>
    <li>Extract a list of available work items</li>
    <li>Navigate to individual work item pages</li>
    <li>Extract detailed information from each work item</li>
    <li>Update work item comments and status</li>
</ul>

<details><summary><h2>Prerequisites</h2></summary
                                            
<ul>
    <li>UiPath Studio (latest version)</li>
    <li>A compatible web browser (Chrome)</li>
    <li>UiPath Web Automation packages installed</li>
    <li>Stable internet connection</li>
    <li>Valid credentials for the ACME System1 website</li>
</ul>
    
</details>

<h2>Installation</h2>
<p>Download or clone this Library:</p>
<ul>
    <li><a href="https://github.com/your-repo/ACME-System-1" target="_blank">ACME System 1</a></li>
</ul>
<p>Open UiPath Studio and load the library into your project.</p>

<h2>Usage</h2>
<h3>Library</h3>
<ol>
    <li><strong>Import the Library:</strong> After cloning or downloading, import the library into your UiPath project.</li>
    <li><strong>Setup Credentials:</strong> Ensure that your ACME System1 login credentials are stored securely, either using UiPath Orchestrator Assets or Windows Credential Manager.</li>
    <li><strong>Use Activities:</strong> Use the following sequence of activities to automate ACME System1 operations:
        <ul>
            <li><strong>Login:</strong> Automates logging into the ACME System1 website.</li>
            <li><strong>Navigate to Work Items:</strong> Directs the browser to the Work Items page.</li>
            <li><strong>Extract Work Items:</strong> Scrapes data about all work items from the page.</li>
            <li><strong>Navigate to Details Page:</strong> For each work item, this navigates to its detail page.</li>
            <li><strong>Extract Data from Details Page:</strong> Captures information such as Client ID, Account Number, Account Amount.</li>
            <li><strong>Click Update Work Item Button:</strong> Clicks on the Update Work Item Button to open the update page.</li>
            <li><strong>Update Work Item:</strong> Automates navigating to the update page, where it changes the comment and status fields for each work item.</li>
            <li><strong>Logout:</strong> Logs out from the system.</li>
        </ul>
    </li>
</ol>

<h2>Example Workflow</h2>
<ol>
    <li><strong>Login:</strong> Pass the username and password as input arguments or store them securely using Orchestrator Assets or Credential Manager.</li>
    <li><strong>Navigate and Extract:</strong> After logging in, navigate to the Work Items page and extract the available work items.</li>
    <li><strong>Iterate through Work Items:</strong> For each work item:
        <ul>
            <li>Navigate to the work item detail page.</li>
            <li>Extract details such as Client ID, Account Number, and Account Amount.</li>
            <li>Navigate to the update page and update the status and comment fields.</li>
        </ul>
    </li>
    <li><strong>Logout:</strong> Once all work items are processed, log out from the ACME System1 website.</li>
</ol>

<h2>Customization</h2>
<ul>
    <li><strong>Browser Type:</strong> The library is set to use Chrome by default.</li>
    <li><strong>Selector Updates:</strong> Depending on any UI changes to the ACME System1 website, the Library will adjust the selectors for navigating or extracting work item details.</li>
</ul>

<h2>Error Handling</h2>
<p>Proper exception handling is built into the activities to ensure that the process continues even if a particular work item cannot be processed. If the login fails, the process will retry a set number of times before exiting.</p>

<h2>Contributions</h2>
<p>Feel free to submit issues or pull requests to enhance the library.</p>
