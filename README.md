Download Link: https://assignmentchef.com/product/solved-java-swed-bank-java-assignment
<br>
You are assigned to create a micro-service for a small company, that would give an overview of acquired shares. It should be possible to report purchased share volumes and retrieve the already inserted information by employees. The application initially will have only RESTful API with JSON payloads in response but won’t be limited only to this interface in the future. The data should be stored in embedded database, but it should be possible to swap current data storage to something else (MsSQL, Oracle DB etc.).

<strong>Stock registration should accept:</strong>

<ul>

 <li>share data (Company name, share name, share ISIN code, country, field of economic activity)</li>

 <li>price per share in EUR (Ex. 10.10)</li>

 <li>volume acquired in number (Ex. 12)</li>

 <li>date (ISO format)</li>

 <li>employee ID (Ex. 12345)</li>

</ul>

It should be possible to register one single record or bulk consumption (multiple records in one file, for example multipart/form-data).

Data validation should be performed before persisting and corresponding error message should be returned in case of invalid input.

<strong>Share purchase data retrieval should provide (as a separate endpoint):</strong>

<ul>

 <li>total spent amount of money grouped by month</li>

 <li>list share acquiring records for specified month (each row should contain: Company name, share name, share ISIN code, country, field of economic activity, volume, date, price, total price, employee</li>

</ul>

<ol>

 <li>ID)</li>

</ol>

<ul>

 <li>statistics for each month, list share acquiring records grouped by share id (each row should contain: Company name, share name, share ISIN code, country, field of economic activity, average price, total volume, total price)</li>

</ul>

Every request can be made either for all employees or for the specific employee (identified by id).

<strong>Expected result:</strong>

<ul>

 <li>RESTful API with JSON payloads in response</li>

 <li>Language: Java 11 +</li>

 <li>Any framework (preferably Spring boot). But keep in mind that usage of framework should be reasonable, and architecture of application should allow to switch frameworks.</li>

 <li>Code should be covered by automatic tests</li>

</ul>

· Object-oriented design principles