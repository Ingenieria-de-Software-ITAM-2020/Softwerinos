**IEEE Test Plan Outline ![](Plan%20de%20Calidad.001.png)**

Foundation Course in Software Testing 

TEST PLAN OUTLINE (IEEE 829 FORMAT) 

1) Test Plan Identifier 
1) References 
1) Introduction 
1) Test Items 
1) Software Risk Issues 
1) Features to be Tested 
1) Features not to be Tested 
1) Approach  
1) Item Pass/Fail Criteria 
1) Suspension Criteria and Resumption Requirements 
1) Test Deliverables 
1) Remaining Test Tasks 
1) Environmental Needs 
1) Staffing and Training Needs 
1) Responsibilities 
1) Schedule 
1) Planning Risks and Contingencies 
1) Approvals 
1) Glossary ![](Plan%20de%20Calidad.002.png)

IEEE TEST PLAN TEMPLATE 

Está bueno el template

**1  TEST PLAN IDENTIFIER** 

Some type of unique company generated number to identify this test plan, its level and the level of software that it is related to.  Preferably the test plan level will be the same as the related software level.  The number may also identify whether the test plan is a Master plan, a Level plan, an integration plan or whichever plan level it represents. This is to assist in coordinating software and testware versions within configuration management. 

Keep in mind that test plans are like other software documentation, they are dynamic in nature and must be kept up to date.  Therefore, they will have revision numbers. 

You may want to include author and contact information including the revision history information as part of either the identifier section of as part of the introduction. 

**2  REFERENCES** 

List all documents that support this test plan.  Refer to the actual version/release number of the document as stored in the configuration management system. Do not duplicate the text from other documents as this will reduce the viability of this document and increase the maintenance effort. Documents that can be referenced include: 

Project Plan 

Requirements specifications 

High Level design document 

Detail design document 

Development and Test process standards Methodology guidelines and examples Corporate standards and guidelines 

**3  INTRODUCTION** 

State the purpose of the Plan, possibly identifying the level of the plan (master etc.). This is essentially the executive summary part of the plan. 

You may want to include any references to other plans, documents or items that contain information relevant to this project/process.  If preferable, you can create a references section to contain all reference documents. 

Identify the Scope of the plan in relation to the Software Project plan that it relates to. Other items may include, resource and budget constraints, scope of the testing effort, how testing relates to other evaluation activities (Analysis & Reviews), and possible the process to be used for change control and communication and coordination of key activities. 

As this is the “Executive Summary” keep information brief and to the point. 

**4  TEST ITEMS (FUNCTIONS)** 

These are things you intend to test within the scope of this test plan.  Essentially, something you will test, a list of what is to be tested. This can be developed from the software application inventories as well as other sources of documentation and information. ![](Plan%20de%20Calidad.002.png)

This can be controlled and defined by your local Configuration Management (CM) process if you have one.  This information includes version numbers, configuration requirements where needed, (especially if multiple versions of the product are supported).  It may also include key delivery schedule issues for critical elements. 

Remember, what you are testing is what you intend to deliver to the Client. 

This section can be oriented to the level of the test plan.  For higher levels it may be by application or functional area, for lower levels it may be by program, unit, module or build. 

**5  SOFTWARE RISK ISSUES** 

Identify what software is to be tested and what the critical areas are, such as: 

1. Delivery of a third party product. 
1. New version of interfacing software 
1. Ability to use and understand a new package/tool, etc. 
1. Extremely complex functions  
1. Modifications to components with a past history of failure 
1. Poorly documented modules or change requests 

There are some inherent software risks such as complexity; these need to be identified.   

1. Safety 
1. Multiple interfaces 
1. Impacts on Client 
1. Government regulations and rules 

Another key area of risk is a misunderstanding of the original requirements. This can occur at the management, user and developer levels. Be aware of vague or unclear requirements and requirements that cannot be tested. 

The past history of defects (bugs) discovered during Unit testing will help identify potential areas within the software that are risky.  If the unit testing discovered a large number of defects or a tendency towards defects in a particular area of the software, this is an indication of potential future problems.  It is the nature of defects to cluster and clump together.  If it was defect ridden earlier, it will most likely continue to be defect prone. 

One good approach to define where the risks are is to have several brainstorming sessions. 

Start with ideas, such as, what worries me about this project/application. 

**6  FEATURES TO BE TESTED** 

This is a listing of what is to be tested from the **USERS** viewpoint of what the system does.  This is not a technical description of the software, but a USERS view of the functions. 

Set the level of risk for each feature.  Use a simple rating scale such as (H, M, L): High, Medium and Low. These types of levels are understandable to a User.  You should be prepared to discuss why a particular level was chosen. 

It should be noted that Section 4 and Section 6 are very similar. The only true difference is the point of view.  Section 4 is a technical type description including version numbers and other technical information and Section 6 is from the User’s viewpoint.  Users do not understand ![](Plan%20de%20Calidad.002.png) technical software terminology; they understand functions and processes as they relate to their jobs.

**7  FEATURES NOT TO BE TESTED** 

This is a listing of what is NOT to be tested from both the Users viewpoint of what the system does and a configuration management/version control view.  This is not a technical description of the software, but a USERS view of the functions. 

Identify WHY the feature is not to be tested, there can be any number of reasons. 

Not to be included in this release of the Software. 

Low risk, has been used before and is considered stable. 

Will be released but not tested or documented as a functional part of the release of this version of the software. 

Sections 6 and 7 are directly related to Sections 5 and 17.  What will and will not be tested are directly affected by the **levels of acceptable risk** within the project, and what does not get tested affects the **level of risk** of the project.  

**8  APPROACH (STRATEGY)** 

This is your overall test strategy for this test plan; it should be appropriate to the level of the plan (master, acceptance, etc.) and should be in agreement with all higher and lower levels of plans.  Overall rules and processes should be identified. 

Are any special tools to be used and what are they? 

Will the tool require special training? 

What metrics will be collected? 

Which level is each metric to be collected at? 

How is Configuration Management to be handled? 

How many different configurations will be tested? 

Hardware 

Software 

Combinations of HW, SW and other vendor packages 

What levels of regression testing will be done and how much at each test level? Will regression testing be based on severity of defects detected? 

How will elements in the requirements and design that do not make sense or are untestable be processed? 

If this is a master test plan the overall project testing approach and coverage requirements must also be identified. 

Specify if there are special requirements for the testing. 

Only the full component will be tested. 

A specified segment of grouping of features/components must be tested together. Other information that may be useful in setting the approach are: 

MTBF, Mean Time Between Failures - if this is a valid measurement for the test involved and if the data is available. 

SRE, Software Reliability Engineering - if this methodology is in use and if the information is available. ![](Plan%20de%20Calidad.002.png)

How will meetings and other organizational processes be handled? 

**9  ITEM PASS/FAIL CRITERIA** 

What are the Completion criteria for this plan?  This is a critical aspect of any test plan and should be appropriate to the level of the plan. 

At the Unit test level this could be items such as: 

All test cases completed. 

A specified percentage of cases completed with a percentage containing some number of minor defects. 

Code coverage tool indicates all code covered. 

At the Master test plan level this could be items such as: 

All lower level plans completed. 

A specified number of plans completed without errors and a percentage with minor defects. 

This could be an individual test case level criterion or a unit level plan or it can be general functional requirements for higher level plans. 

What is the number and severity of defects located? 

Is it possible to compare this to the total number of defects?  This may be impossible, as some defects are never detected. 

A defect is something that **may** cause a failure, and may be acceptable to leave in the application. 

A failure is the result of a defect as seen by the User, the system crashes, etc. 

**10  SUSPENSION CRITERIA AND RESUMPTION REQUIREMENTS** 

Know when to pause in a series of tests. 

If the number or type of defects reaches a point where the follow on testing has no value, it makes no sense to continue the test; you are just wasting resources. 

Specify what constitutes stoppage for a test or series of tests and what is the acceptable level of defects that will allow the testing to proceed past the defects. 

Testing after a truly fatal error will generate conditions that may be identified as defects but are in fact ghost errors caused by the earlier defects that were ignored. 

**11  TEST DELIVERABLES** 

What is to be delivered as part of this plan? 

Test plan document. 

Test cases. 

Test design specifications. 

Tools and their outputs. 

Simulators. 

Static and dynamic generators. 

Error logs and execution logs. Problem reports and corrective actions. 

One thing that is not a test deliverable is the software itself that is listed under test items and is delivered by development. ![](Plan%20de%20Calidad.002.png)

**12  REMAINING TEST TASKS** 

If this is a multi-phase process or if the application is to be released in increments there may be parts of the application that this plan does not address.  These areas need to be identified to avoid any confusion should defects be reported back on those future functions.  This will also allow the users and testers to avoid incomplete functions and prevent waste of resources chasing non-defects. 

If the project is being developed as a multi-party process, this plan may only cover a portion of the total functions/features. This status needs to be identified so that those other areas have plans developed for them and to avoid wasting resources tracking defects that do not relate to this plan. 

When a third party is developing the software, this section may contain descriptions of those test tasks belonging to both the internal groups and the external groups. 

**13  ENVIRONMENTAL NEEDS** 

Are there any special requirements for this test plan, such as: 

Special hardware such as simulators, static generators etc. 

How will test data be provided.  Are there special collection requirements or specific ranges of data that must be provided? 

How much testing will be done on each component of a multi-part feature? Special power requirements. 

Specific versions of other supporting software. 

Restricted use of the system during testing. 

**14  STAFFING AND TRAINING NEEDS** 

Training on the application/system. 

Training for any test tools to be used. 

Section 4 and Section 15 also affect this section.  What is to be tested and who is responsible for the testing and training. 

**15  RESPONSIBILITIES** 

Who is in charge? 

This issue includes all areas of the plan.  Here are some examples: 

Setting risks. 

Selecting features to be tested and not tested. 

Setting overall strategy for this level of plan. Ensuring all required elements are in place for testing. 

Providing for resolution of scheduling conflicts, especially, if testing is done on the production system. 

Who provides the required training? 

Who makes the critical go/no go decisions for items not covered in the test plans?![](Plan%20de%20Calidad.002.png)

**16  SCHEDULE** 

Should be based on realistic and validated estimates.  If the estimates for the development of the application are inaccurate, the entire project plan will slip and the testing is part of the overall project plan. 

As we all know, the first area of a project plan to get cut when it comes to crunch time at the end of a project is the testing.  It usually comes down to the decision, ‘Let’s put something out even if it does not really work all that well’. And, as we all know, this is usually the worst possible decision. 

How slippage in the schedule will to be handled should also be addressed here. 

If the users know in advance that a slippage in the development will cause a slippage in the test and the overall delivery of the system, they just may be a little more tolerant, if they know it’s in their interest to get a better tested application. 

By spelling out the effects here you have a chance to discuss them in advance of their actual occurrence. You may even get the users to agree to a few defects in advance, if the schedule slips. 

At this point, all relevant milestones should be identified with their relationship to the development process identified.  This will also help in identifying and tracking potential slippage in the schedule caused by the test process. 

It is always best to tie all test dates directly to their related development activity dates.  This prevents the test team from being perceived as the cause of a delay.  For example, if system testing is to begin after delivery of the final build, then system testing begins the day after delivery.  If the delivery is late, system testing starts from the day of delivery, not on a specific date.  This is called dependent or relative dating. 

**17  PLANNING RISKS AND CONTINGENCIES** 

What are the overall risks to the project with an emphasis on the testing process? 

Lack of personnel resources when testing is to begin. 

Lack of availability of required hardware, software, data or tools. Late delivery of the software, hardware or tools. 

Delays in training on the application and/or tools. 

Changes to the original requirements or designs. 

Specify what will be done for various events, for example: 

Requirements definition will be complete by January 1, 19XX, and, if the requirements change after that date, the following actions will be taken. 

The test schedule and development schedule will move out an appropriate number of days.  This rarely occurs, as most projects tend to have fixed delivery dates. 

The number of test performed will be reduced. 

The number of acceptable defects will be increased. 

These two items could lower the overall quality of the delivered product. Resources will be added to the test team. 

The test team will work overtime. 

This could affect team morale. 

The scope of the plan may be changed. 

There may be some optimization of resources.  This should be avoided, if possible, for obvious reasons. ![](Plan%20de%20Calidad.002.png)

You could just QUIT.  A rather extreme option to say the least. 

Management is usually reluctant to accept scenarios such as the one above even though they have seen it happen in the past. 

The important thing to remember is that, if you do nothing at all, the usual result is that testing is cut back or omitted completely, neither of which should be an acceptable option. 

**18  APPROVALS** 

Who can approve the process as complete and allow the project to proceed to the next level (depending on the level of the plan)? 

At the master test plan level, this may be all involved parties. 

When determining the approval process, keep in mind who the audience is.  

The audience for a unit test level plan is different than that of an integration, system or master level plan. 

The levels and type of knowledge at the various levels will be different as well. Programmers are very technical but may not have a clear understanding of the overall 

business process driving the project. 

Users may have varying levels of business acumen and very little technical skills. Always be wary of users who claim high levels of technical skills and programmers that 

claim to fully understand the business process.  These types of individuals can cause more harm than good if they do not have the skills they believe they possess. 

**19  GLOSSARY** 

Used to define terms and acronyms used in the document, and testing in general, to eliminate confusion and promote consistent communications. ![](Plan%20de%20Calidad.002.png)

**SAMPLE MASTER TEST PLAN** 

**1  TEST PLAN IDENTIFIER  RS-MTP01.3 2  REFERENCES** 

None Identified. 

**3  INTRODUCTION** 

This is the Master Test Plan for the Reassigned Sales Re-write project. This plan will address only those items and elements that are related to the Reassigned Sales process, both directly and indirectly affected elements will be addressed. The primary focus of this plan is to ensure that the new Reassigned Sales application provides the same level of information and detail as the current system while allowing for improvements and increases in data acquisition and level of details available 

(granularity).

The project will have three levels of testing, Unit, System/Integration and Acceptance. The details for each level are addressed in the approach section and will be further defined in the level specific plans. 

The estimated time line for this project is very aggressive (six (6) months), as such, any delays in the development process or in the installation and verification of the third party software could have significant effects on the test plan. The acceptance testing is expected to take one (1) month from the date of application delivery from system test and is to be done in parallel with the current application process. 

**4  TEST ITEMS** 

The following is a list, by version and release, of the items to be tested:

1. EXTOL EDI package, Version **3.0** 

If a new release is available prior to roll-out it will not be used until after installation. It will be a separate upgrade/update project. 

2. DNS PC EDI transaction package, Version **2.2** 

If a new release is available prior to roll-out it will not be used until after installation. It will be a separate upgrade/update project. 

3. Custom PC EDI transaction package (two distributors only). 
3. New reassigned sales software, initial version to be Version **1.0** 

A detailed listing of programs, databases, screens and reports will be provided in the system and detailed design documents. 

5. Order Entry EDI interface software, Current version at time of pilot. Currently, version **4.1.** 
5. Reassigned Sales System requirements document, SST\_RQMT.WPD version **4.1** 
5. Reassigned Sales System Design Document, SST\_SYSD.WPD version **3.02** 
5. Reassigned Sales Detail Design Document, SST\_DTLD.WPD version **3.04** ![](Plan%20de%20Calidad.002.png)

**5  SOFTWARE RISK ISSUES** 

There are several parts of the project that are not within the control of the Reassigned Sales application but have direct impacts on the process and must be checked as well. 

1. The local AS/400 based vendor supplied EDI software package. This package will be providing all the reformatting support from the ANSI X12 EDI formats to the internal AS/400 data base file formats. 
1. The PC based software package installed at each distributor's location (both custom written and vendor supplied) will be providing the formatting of the distributors data into the correct EDI X12 formats.  
1. Backup and Recovery of the EDI transmission files, local databases and restart of the translation process, must be carefully checked. 
1. The ability to restart the application in the middle of the process is a critical factor to application reliability. This is especially true in the case of the transmission files as once the data is pulled from the mail box it is no longer available there and must be protected locally. 
1. Database security and access must be defined and verified, especially for files shared between the Order Entry application and the Reassigned Sales process. All basic security will be provided through the AS/400 systems native security process. 

**6  FEATURES TO BE TESTED** 

The following is a list of the areas to be focused on during testing of the application. 

1. New EDI data acquisition process. 
1. Redesigned On-line screens. 
1. Redesigned/Converted reports. 
1. New Automated Archive process. 
1. Interface to the Order Entry system and data bases. 
1. Computation of Sales Activity by region for commissions 

**7  FEATURES NOT TO BE TESTED** 

The following is a list of the areas that will not be specifically addressed.  All testing in these areas will be indirect as a result of other testing efforts. 

1. Non-EDI Order Entry processes. 

Only the EDI interface of the Order Entry application will be verified. Changes to the EDI interface to support Reassigned Sales are not anticipated to have an impact on the Order Processing application. Order Entry is a separate application sharing the data interface only, orders will continue to process in the same manner. 

2. Network Security and dial-in access. 

Changes to include EDI transactions for reassigned sales will have no impact on the security aspects of the network or the EXTOL/EDI interface. 

3. Operational aspects of the EDI process.

Changes to include EDI transactions for reassigned sales will have no impact on the operational aspects of the EXTOL/EDI interface. ![](Plan%20de%20Calidad.002.png)

4. PC based spreadsheet analysis applications using Reassigned Sales data. 

These applications are completely under the control of the customer and are outside the scope of this project. The necessary data base format information will be provided to the customers to allow them to extract data. Testing of their applications is the responsibility of the application maintainer/developer. 

5. Business Analysis functions using Reassigned Sales data. 

These applications are completely under the control of the management support team and are outside the scope of this project. The necessary data base format information will be provided to the support team to allow them to extract data. Testing of their applications is the responsibility of the application maintainer/developer. 

6. Marketing/Forecasting processes using Reassigned Sales data. 

These applications are completely under the control of marketing and are outside the scope of this project. The necessary data base format information will be provided to marketing to allow them to extract data. Testing of their applications is the responsibility of the application maintainer/developer. 

**8  APPROACH** 

1. **Testing Levels** 

The testing for the Reassigned Sales project will consist of Unit, System/Integration (combined) and Acceptance test levels. It is hoped that there will be at least one full time independent test person for system/integration testing. However, with the budget constraints and time line established; most testing will be done by the test manager with the development teams participation. 

UNIT Testing will be done by the developer and will be approved by the development team leader. Proof of unit testing (test case list, sample output, data printouts, defect information)  must be provided by the programmer to the team leader before unit testing will be accepted and passed on to the test person. All unit test information will also be provided to the test person. 

SYSTEM/INTEGRATION Testing will be performed by the test manager and development team leader with assistance from the individual developers as required.  No specific test tools are available for this project. Programs will enter into System/Integration test after all critical defects have been corrected. A program may have up to two Major defects as long as they do not impede testing of the program (I.E. there is a work around for the error). 

ACCEPTANCE Testing will be performed by the actual end users with the assistance of the test manager and development team leader. The acceptance test will be done in parallel with the existing manual ZIP/FAX process for a period of one month after completion of the System/Integration test process.  

Programs will enter into Acceptance test after all critical and major defects have been corrected. A program may have one major defect as long as it does not impede testing of the program (I.E. there is a work around for the error). Prior to final completion of acceptance testing all open critical and major defects MUST be corrected and verified by the Customer test representative. 

A limited number of distributors will participate in the initial acceptance test process. Once acceptance test is complete, distributors will be added as their ability to generate the required EDI data is verified and checked against their FAX/ZIP data. As such, some distributors will be in actual production and some in parallel testing at the same time. This will require careful ![](Plan%20de%20Calidad.002.png) coordination of the control tables for the production system to avoid posting test data into the system. 

2. **Configuration Management/Change Control** 

Movement of programs from the development portion of the  ‘RED’ system to the test portion of the ‘RED’ system will be controlled through the existing Configuration Management application process, ‘EXTRACT’. This will ensure that programs under development and those in full test will have the same version controls and tracking of changes. The same extract process will be used to migrate the programs from the Development/Test ‘RED’ system to the production ‘BLUE’ system once all testing has been completed according to published plans and guidelines. 

All Unit and initial system testing will be performed on the Development AS/400 ‘RED’ system. Once the system has reached a reasonable level of stability, no critical or major defects outstanding, initial pilot testing will be done on the production AS/400 ‘BLUE’ system. All testing done on the ‘BLUE’ system will be done in a parallel mode will all controls set to prevent actual updating of the production files. 

This will allow some early testing of the numbers received through the old ZIP/FAX process and the higher level of detail received through the new EDI process. This will also help identify potential problems with the comparison of the two sets of numbers. 

All changes, enhancements and other modification requests to the system will be handled through the published change control procedures. Any modifications to the standard procedures are identified in the project plan change control section. 

3. **Test Tools** 

The only test tools to be used are the standard AS/400 provided utilities and commands.  

1. The Program Development Manager (PDM) will be used as the source version configuration management tool in conjunction with the in-house check-in/check-out control utility. The check-in/out utility is part of each developers standard AS/400 access menu. 
1. The initial prototypes for the new screens will be developed using the AS/400 Screen Design Aid (SDA). The initial layout and general content of the screens will be shown to the sales administration staff prior to proceeding with testing and development of the screens. 
1. All editing, compiling and debugging will be done using the Source Entry Utility (SEU). 
1. Data acquisition will be from actual production files where available using the AS/400 data base copy command CPYF and it's various functions. Additional data will be created and modified as needed using the Data File Utility (DFU). No changes will ever be made to actual production files under any circumstances. 
1. Initial data for EDI testing will be done using one or two beta sites and replicating the data at the mailbox location or locally in the control files, to create high volume data and to simulate multiple distributors sending in data. 
4. **Meetings** 

The test team will meet once every two weeks to evaluate progress to date and to identify error trends and problems as early as possible. The test team leader will meet with development and the project manager once every two weeks as well. These two meetings will be scheduled on different weeks. Additional meetings can be called as required for emergency situations. ![](Plan%20de%20Calidad.002.png)

5. **Measures and Metrics** 

The following information will be collected by the Development team during the Unit testing process. This information will be provided to the test team at program turnover as well as be provided to the project team on a biweekly basis. 

1. Defects by module and severity. 
1. Defect Origin (Requirement, Design, Code) 
1. Time spent on defect resolution by defect, for Critical & Major only.  All Minor defects can be totaled together. 

The following information will be collected by the test team during all testing phases. This information will be provided on a biweekly basis to the test manager and to the project team.  

1. Defects by module and severity. 
1. Defect Origin (Requirement, Design, Code) 
1. Time spent on defect investigation by defect, for Critical & Major only.  All Minor defects can be totaled together. 
1. Number of times a program submitted to test team as ready for test. 
1. Defects located at higher levels that should have been caught at lower levels of testing. 

**9  ITEM PASS/FAIL CRITERIA** 

The test process will be completed once the initial set of distributors have successfully sent in reassigned sales data for a period of one month and the new EDI data balances with the old ZIP/FAX data received in parallel. When the sales administration staff is 

satisfied that the data is correct the initial set of distributors will be set to active and all parallel stopped for those accounts. 

At this point the next set of distributors will begin the parallel process, if not already doing so. Only the initial set of distributors must pass the data comparison test to complete the testing, at that point the application is considered live. All additional activations will be on an as ready basis.  When a distributor is ready, and their data is verified, they will then also be activated. ![](Plan%20de%20Calidad.002.png)

**10  SUSPENSION CRITERIA AND RESUMPTION REQUIREMENTS** 

1. No Distributors are ready for testing at pilot initiation. 

The pilot project will be delayed until at least three Distributors are ready to initiate the pilot process. No additional elements will be added to the Reassigned Sales project during this delay.  

2. Unavailability of two EDI mail boxes. 

In the event two production lines and mail box facilities cannot be obtained the current single production line and mail box will continue to be used until a second line becomes available. This will necessitate careful coordination between the Order Entry department and the Reassigned Sales group. 

3. Distributor PC EDI software delays. 

In the event of a delay in the delivery or availability of the PC software package, the only major delay will be in pilot testing. Unit, Integration and Systems testing can continue using limited data until such time as the PC software is ready.  

This will also add time to the lower levels of testing as full complete testing cannot be done without reasonable amounts of data. The data can only be derived from actual transmissions from the PC software package. 

**11  TEST DELIVERABLES** 

Acceptance test plan System/Integration test plan 

Unit test plans/turnover documentation Screen prototypes 

Report mock-ups 

Defect/Incident  reports and summaries Test logs and turnover reports 

**12  REMAINING TEST TASKS ![](Plan%20de%20Calidad.002.png)**



|<p>TASK </p><p>Create Acceptance Test Plan </p><p>Create System/Integration Test Plan Define Unit Test rules and Procedures Define Turnover procedures for each level Verify prototypes of Screens </p><p>Verify prototypes of Reports </p>|<p>Assigned To </p><p>TM, PM, Client TM, PM, Dev.  TM, PM, Dev. TM, Dev </p><p>Dev, Client, TM Dev, Client, TM </p>|Status |
| - | - | - |
**13  ENVIRONMENTAL NEEDS** 

The following elements are required to support the overall testing effort at all levels within the reassigned sales project: 

1. Access to both the development and production AS/400 systems.  For development, data acquisition and testing. 
1. A communications line to the EDI mailbox facility. This will have to be a shared line with the Order Entry process as only one mailbox is in use. There will have to be a coordinated effort to determine how often to poll the mailbox as the order entry process requires that data be accessed every hour and the sales process really only needs to be pulled once a day. 
1. An installed and functional copy of the AS/400 based EDI vendor package. 
1. At least one distributor with an installed copy of the PC based EDI vendor package for sales data. 
1. Access to the master control tables (data bases) for controlling the production/testing environment on both production and development systems. 
1. Access to the nightly backup/recovery process. 

**14  STAFFING AND TRAINING NEEDS** 

It is preferred that there will be at least one (1) full time tester assigned to the project for the system/integration and acceptance testing phases of the project. This will require assignment of a person part time at the beginning of the project to participate in reviews etc... and approximately four months into the project they would be assigned full time. If a separate test person is not available the project manager/test 

manager will assume this role.

In order to provide complete and proper testing the following areas need to be addressed in terms of training. 

1. The developers and tester(s) will need to be trained on the basic operations of the EDI interface. Prior to final acceptance of the project the operations staff will also require complete training on the EDI communications process. 
1. The sales administration staff will require training on the new screens and reports. 
1. At least one developer and operations staff member needs to be trained on the installation and control of the PC based distributors EDI package. The distributors personnel will also have to be trained on the PC based package and its operational characteristics. ![](Plan%20de%20Calidad.002.png)

**15  RESPONSIBILITIES** 



|<p>Acceptance test Documentation & Execution System/Integration test Documentation & Exec. Unit test documentation & execution </p><p>System Design Reviews </p><p>Detail Design Reviews </p><p>Test procedures and rules </p><p>Screen & Report prototype reviews </p><p>Change Control and regression testing </p>|<p>TM </p><p>X X X X X X </p><p>X </p>|<p>PM X </p><p>X X X </p><p>X </p>|<p>Dev Team</p><p>X X X </p><p>X X X X </p>|<p>Test Team </p><p>X X X X X X X X </p>|<p>Client X </p><p>X </p><p>X X </p>|
| :- | - | :-: | - | :- | :-: |
The development team leader will be responsible for the verification and acceptance of all unit test plans and documentation. 

The project manager/test manager is responsible for all test plans and documentation.  

The entire project team will participate in the review of the system and detail designs as well as review of any change requests that are generated by the user or as a result of defects discovered during development and testing. The sales administration staff is also required to participate in the initial high-level system review. 

The sales administration staff will provide a person, as required, throughout the project to verify test results and answer questions as they arise. This person will also be responsible for participating in the execution of the acceptance test plan. 

**16  SCHEDULE** 

Time has been allocated within the project plan for the following testing activities. The specific dates and times for each activity are defined in the project plan time line. The persons required for each process are detailed in the project time line and plan as well. Coordination of the personnel required for each task, test team, development team, management and customer will be handled by the project manager in conjunction with the development and test team leaders. 

1. Review of Requirements document by test team personnel (with other team members) and initial creation of Inventory classes, sub-classes and objectives. 
1. Development of Master test plan by test manager and test with time allocated for at least two reviews of the plan. 
1. Review of the System design document by test team personnel. This will provide the team with a clearer understanding of the application structure and will further define the Inventory classes, sub-classes and objectives. ![](Plan%20de%20Calidad.002.png)
4. Development of System/Integration and Acceptance test plans by test manager and other essential personnel with time allocated for at least two reviews of the plans. 
5. Review of the Detail design document(s) by test team personnel as required. This will provide the team with a clearer understanding of the individual program structure and will further define the Inventory classes, sub-classes and objectives. 
5. Unit test time within the development process.  
5. Time allocated for both System/Integration and Acceptance test processes. 

**17  PLANNING RISKS AND CONTINGENCIES** 

A.  Limited Reassigned Sales staff. 

The Reassigned Sales administration staff currently has two positions unfilled. As a result of this staff shortage there may be delays in getting staff to review appropriate documents and to participate in the Acceptance test process. Should client staff become a problem, the appropriate dates for reviews and acceptance testing will slip accordingly. No attempt will be made to bypass any part of the review and testing processes.

However, if acceptable to the Reassigned Sales staff administrator, a member if the test team my be available to act as the client’s representative for part of the Acceptance test itself. The reviews of the screens and reports must have Client participation and approval. 

**18  APPROVALS ![](Plan%20de%20Calidad.002.png)**



|<p>Project Sponsor - Steve Sponsor </p><p>Development Management - Ron Manager EDI Project Manager - Peggy Project </p><p>RS Test Manager - Dale Tester </p><p>RS Development Team Manager - Dale Tester Reassigned Sales - Cathy Sales </p><p>Order Entry EDI Team Manager - Julie Order </p>||
| - | :- |

Prepared by Systeme Evolutif Limited  Page PAGE23 
