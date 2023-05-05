Download Link: https://assignmentchef.com/product/solved-dbms-lab-project-database-development
<br>



<strong><u>Objective:</u></strong>

Enable the student to design and develop a database. In this project, the student are required to show their abilities of:

<ul>

 <li>Analyzing the System Requirement</li>

 <li>Represent the requirement into logical design using Entity Relationship (ER) or/and Enhanced Entity Relationship (EER) model</li>

 <li>Mapping the designed model into relational schemas</li>

 <li>Transform the relational schemas into normalized tables</li>

 <li>Writing SQL statements to creates the tables including all applied integrity constraints</li>

 <li>Writing SQL statements to populate the initial records of each table</li>

 <li>Front End Development of Forms/ Reports</li>

</ul>

<strong><u>Case Brief</u></strong>

<strong>HAMAREY BACHCHEY</strong>

<ol>

 <li><strong> Introduction</strong></li>

</ol>

Hamarey Bachchey is a NGO with the goal to reform education for children. They offer weekly classes for children below the age of 15. They wish to develop a database system.

The NGO is organized in the following ways.

After signing up, each student has to register for a course, and can only be registered to one course at a time. Once the course is completed, the student can register for a new course. After registration, the student is split into different classes based on their age (eg 3-4 years to class 1, 4-6 years to class 2, etc). Each class will be taught the same subjects, in a manner best suited to their age group. Each class can have multiple sections, depending on the need. Classes can also be further separated into groups based on students’ gender. Classes can also be given a custom title.

Each students’ personal information will be saved, including photos which may need to be updated every year. The most crucial information will be that of the parents/guardians. The Email, phone number, address and CNIC of both parents need to be recorded for each student. In the event of any incident where the parents will be unavailable, a guardian also needs to be available, in which case their details and relation to the students also need to be recorded. A history needs to be maintained for whenever base information of students/parents/guardians is changed.

For the earlier classes with very young students, the mother needs to be present with the child. If for whatever reason the mother cannot come, a female guardian must be present instead. In such cases, the NGO needs to be informed ahead of time of the individual accompanying the child, and other such information, including whether the individual is pregnant and/or needs assistance in any way.

The fee each student has to pay is different, depending on their class. If a parent admits more than 3 children, they may be offered a discount. Moreover, if the parents can’t pay for legitimate reasons, they will be offered a discount. There will be no fee for a child of a Hamarey Bachchey staff member. Payment of fee is made before admission to a third-party which provides the parents a challan or voucher number, which the parents then enter during admission process.

<ol start="2">

 <li><strong> The following manual records are kept:</strong></li>

</ol>

The following are samples of forms the NGO currently maintain. These forms need to be developed using web. Data should be enter through these forms. Forms/attributes can be added if required.

The student admission form is filled by every parent/guardian for every child’s admission.

<strong>Form: Student Admission</strong>

<table width="650">

 <tbody>

  <tr>

   <td width="650"><strong>HAMAREY BACHCHEY</strong><strong>STUDENT ADMISSION FORM</strong>

    <table width="71">

     <tbody>

      <tr>

       <td width="71">Photo</td>

      </tr>

     </tbody>

    </table><strong>Students Information:</strong>Name  : Date of Birth   :Gender            :

    <table width="630">

     <tbody>

      <tr>

       <td colspan="2" width="336"><strong>Parents Information:</strong>Mother Name     :</td>

       <td width="144">Father Name</td>

       <td width="150">:</td>

      </tr>

      <tr>

       <td width="144">  Mother Contact</td>

       <td width="192">:</td>

       <td width="144">Father Contact</td>

       <td width="150">:</td>

      </tr>

      <tr>

       <td width="144">  Mother CNIC</td>

       <td width="192">:</td>

       <td width="144">Father CNIC</td>

       <td width="150">:</td>

      </tr>

      <tr>

       <td width="144">  Mother Email</td>

       <td width="192">:</td>

       <td width="144">Father Email</td>

       <td width="150">:</td>

      </tr>

      <tr>

       <td width="144">  Mother Address</td>

       <td width="192">:</td>

       <td width="144">Father Address</td>

       <td width="150">:</td>

      </tr>

      <tr>

       <td colspan="2" width="336"><strong>Guardian Information:</strong>Guardian Name   :   Guardian Contact:   Guardian CNIC     :Guardian Gender :Relation        :</td>

       <td width="144"> </td>

       <td width="150"> </td>

      </tr>

     </tbody>

    </table><strong>For Staff Only</strong>Fee Amount :   Discount :Final Amount    :Fee Fully Paid :           YesNo Challan #       :</td>

  </tr>

 </tbody>

</table>

In the event a guardian must accompany a child for a class, they have to fill the following form ahead of time.

<strong>Form: Student Accompanying Form</strong>

Some forms are used by the admins for internal management, such as assigning/reallocation students to different classes.

<strong>Form: Class Assignment</strong>

<strong>Note:</strong> Other required forms/attributes can be created.

The following is a sample of how the NGO wants their student management GUI to look like: <strong>Students per class (A list of students grouped by classes)</strong>

<table width="650">

 <tbody>

  <tr>

   <td width="650"><strong>HAMAREY BACHCHEY</strong><strong>STUDENTS PER CLASS FORM</strong>

    <table width="286">

     <tbody>

      <tr>

       <td width="79">Name   ▼</td>

       <td width="147"> </td>

       <td width="59">ADD +</td>

      </tr>

     </tbody>

    </table>SEARCH<strong>Class 1A [MQM] (12 total):</strong>

    <table width="630">

     <tbody>

      <tr>

       <td width="96">ID: 0001</td>

       <td width="144">Name: Hammad</td>

       <td width="144">Age(yrs): 3.2</td>

       <td width="246">Gender: M</td>

      </tr>

      <tr>

       <td width="96">ID: 0002</td>

       <td width="144">Name: Haniya</td>

       <td width="144">Age(yrs): 3.6 ...</td>

       <td width="246">Gender: F</td>

      </tr>

      <tr>

       <td width="96">ID: 0011</td>

       <td width="144">Name: Huda</td>

       <td width="144">Age(yrs): 3.5</td>

       <td width="246">Gender: F</td>

      </tr>

      <tr>

       <td width="96">ID: 0012</td>

       <td width="144">Name: Zayneb</td>

       <td width="144">Age(yrs): 3.4</td>

       <td width="246">Gender: F</td>

      </tr>

      <tr>

       <td width="96"><strong>Class 1B [MQ</strong></td>

       <td width="144"><strong>J] (13 total):</strong></td>

       <td width="144"> </td>

       <td width="246"> </td>

      </tr>

      <tr>

       <td width="96">ID: 0101</td>

       <td width="144">Name: Ahmed</td>

       <td width="144">Age(yrs): 3.1</td>

       <td width="246">Gender: M</td>

      </tr>

      <tr>

       <td width="96">ID: 0101</td>

       <td width="144">Name: Fatima</td>

       <td width="144">Age(yrs): 3.3 ...</td>

       <td width="246">Gender: F</td>

      </tr>

      <tr>

       <td width="96">ID: 0112</td>

       <td width="144">Name: Saqib</td>

       <td width="144">Age(yrs): 3.2</td>

       <td width="246">Gender: M</td>

      </tr>

      <tr>

       <td width="96">ID: 0113</td>

       <td width="144">Name: Huda</td>

       <td width="144">Age(yrs): 3.2</td>

       <td width="246">Gender: F</td>

      </tr>

      <tr>

       <td width="96"><strong>Class 2A [RT</strong></td>

       <td width="144"><strong>-girls] (15 total)</strong></td>

       <td width="144"><strong>:</strong></td>

       <td width="246"> </td>

      </tr>

      <tr>

       <td width="96">ID: 0201</td>

       <td width="144">Name: Husna</td>

       <td width="144">Age(yrs): 4.1</td>

       <td width="246">Gender: F</td>

      </tr>

      <tr>

       <td width="96">ID: 0202</td>

       <td width="144">Name: Kanwal</td>

       <td width="144">Age(yrs): 4.5 ...</td>

       <td width="246">Gender: F</td>

      </tr>

      <tr>

       <td width="96">ID: 0214</td>

       <td width="144">Name: Asma</td>

       <td width="144">Age(yrs): 4.4</td>

       <td width="246">Gender: F</td>

      </tr>

      <tr>

       <td width="96">ID: 0215</td>

       <td width="144">Name: Nur</td>

       <td width="144">Age(yrs): 4.7</td>

       <td width="246">Gender: F</td>

      </tr>

      <tr>

       <td width="96"><strong>Class 2B [RT</strong></td>

       <td width="144"><strong>-boys] (9 total):</strong></td>

       <td width="144"> </td>

       <td width="246"> </td>

      </tr>

      <tr>

       <td width="96">ID: 0301</td>

       <td width="144">Name: Hassan</td>

       <td width="144">Age(yrs): 4.2</td>

       <td width="246">Gender: M</td>

      </tr>

      <tr>

       <td width="96">ID: 0302</td>

       <td width="144">Name: Ismael</td>

       <td width="144">Age(yrs): 4.8 ...</td>

       <td width="246">Gender: M</td>

      </tr>

      <tr>

       <td width="96">ID: 0308</td>

       <td width="144">Name: Usman</td>

       <td width="144">Age(yrs): 4.0</td>

       <td width="246">Gender: M</td>

      </tr>

      <tr>

       <td colspan="4" width="630">ID: 0309    Name: Ibrahim     Age(yrs): 4.9     Gender: M</td>

      </tr>

     </tbody>

    </table><strong>.</strong><strong>.</strong></td>

  </tr>

 </tbody>

</table>

<strong>. </strong>

<strong>The following reports / queries are needed:</strong>

<ol>

 <li>A list of all students</li>

 <li>A list of all mothers and their spouses</li>

 <li>A list of all guardians, grouped by relation to students (show students as well)</li>

 <li>A list of parents and their children</li>

 <li>A list of all students with siblings taking classes, grouped by class</li>

 <li>A list of all students who have been assigned to a new class in the given time span (use check for including or ignoring new admissions)</li>

 <li>A list of all new students in given time span grouped by class</li>

 <li>A list of all new parents in given time span (include children info)</li>

 <li>A list of all parents who are early introducers (enroll their children into courses as soon as the children are old enough)</li>

 <li>Class change history of given student</li>

 <li>A report of a list of students grouped by classes along with <strong>add, search, delete, and edit</strong> student features. Search can be performed using student name or id.</li>

 <li>A report of a list of classes with number of students per class and student count per gender. Search can be performed using class name.</li>

 <li>A report of a list of all students who have been dormant for given number of months/years. Search can be performed using months or years.</li>

 <li>A report of all info on a given student (parents, guardians, siblings, class history). Search can be performed using student name or id.</li>

 <li>A report of all info on a given parent (all children, classes of each child, designated guardian). Search can be performed using parent name or id.</li>

</ol>

<strong>Note: [1-10] are stored procedures (only SQL queries required), while [11-15] are reports. The reports should be displayed on front end using web. All GUI reports with lists, should contain search functionality. Also include SQL queries in document which are used for generating reports. </strong>

Document inclusive of following items in appropriate format

<ul>

 <li>ER and/or EER diagram</li>

 <li>Relational schemas/ Mapping</li>

 <li>Description of all tables Datasets</li>

 <li>SQL statements used to create tables.</li>

 <li>SQL statements used to populate tables (insert statements).</li>

 <li>SQL statements as the answer to the needed 15 queries</li>

 <li>Other</li>

</ul>

<strong>Special Instructions:</strong>

<ul>

 <li>Use at least 1 stored procedure (productively)</li>

 <li>Use at least 1 trigger )productively)</li>

</ul>







<strong>Evaluation:</strong>

Each member needs to develop at least one form and one report OR two forms/reports. S/he should be responsible for all of its development activities (Table design, DDL, Queries, PHP, and HTML). During VIVA each member will be evaluated on basis of his/her own work and also general project working (ERD, Table design, Dataset etc.).

The group will be allowed to use different technologies for their projects development, provided they meet the following conditions:

<ul>

 <li>They commit to a set of technologies (after discussing with their instructor) and only work within that set</li>

 <li>No other technologies (other than those committed at the start of the project) will be allowed</li>

 <li>Unless allowed by the instructor, the group may not change their technologies during their project</li>

 <li>You must use a RDBMS</li>

</ul>