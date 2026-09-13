# Topic 1 Conforming Alternate Version and Non-Interference

## Introduction
### Learning Objective
At the end of this Topic you will be able to:
1.	Identify if alternate versions of content exist.
2.	Test if the alternate version passes all applicable Test Conditions in this test process.
3.	Verify if the accessible version is up to date with the same information, language, and functionality.  
4.	Verify if the mechanism to reach the accessible equivalent version passes all applicable tests.
5.	Determine if non-conforming versions of content meet requirements for non-interference.

### Overview
The purpose of this topic is to test the conformance requirements for conforming alternate versions and non-interference. Alternate versions of content may be provided if one of those versions is fully conforming to all test requirements. Conforming alternate versions are acceptable methods to provide the same information and functionality in an accessible manner when other non-conforming versions of that content exist. Providing a conforming alternate version is not a requirement but is sometimes needed so that there is a way for all users to access the content.

When a website provides alternate versions of content to meet accessibility requirements, you will evaluate whether the alternate version provided is fully accessible and equivalent to the original content. In addition, you will evaluate whether each version meets WCAG requirements for accessing the alternate content.
To be considered a conforming alternate version, the following must be determined:
-	Is it fully accessible?
-	Does it have equivalent information and functionality?
-	Is the mechanism to reach it accessible?

If a conforming alternate version is identified, this version replaces the non-conforming version in testing. The non-conforming version is not included in the test report and only the conforming alternate version is tested.

When a conforming alternate version is found, the non-conforming versions only must be tested for 1.D Non-Interference. This ensures that the non-conforming content does not interfere with a user’s ability to access its content.

Although the alternate version must pass all tests in the Trusted Tester test process (covered in Topics 2- 19) to be considered a Conforming Alternate Version, testers should continue testing even if a failure is found. While this deviates from WCAG’s Understanding Conformance article, this will allow all failures to be reported in the same report for eventual remediation. In this case, the test report should indicate that the nonconforming version is still limited to only the non-interference tests.

In this topic the “identified version” refers to the version that has been identified by the developer as the conforming alternate version. This is because you are going to verify if it passes all applicable tests and qualifies to be called a “conforming alternate version.”

*Topic 1 Conforming Alternate Version and Non-Interference* is taught as the last topic in the course because of the complexity and the need to understand all the other topics. This topic is the first test in the Trusted Tester process because it is essential for defining the scope of testing.
There are four test IDs in this topic:
-	1.A Accessible Alternate Version — alt-version-conformant
-	1.B Equivalent Alternative — alt-version-equivalent
-	1.C Conformant Mechanism — alt-version-access
-	1.D Non-Interference — non-interference

## 1.A Accessible Alternate Version

**Test Requirement**

The purpose of this test is to determine if an alternate version of the content passes all applicable Test Conditions. It is not a requirement to provide alternate versions of the same content. However, if only one version of the content exists and it does not conform to the Section 508 requirements, and that version will not be remediated, then conforming alternate versions are necessary. This allows developers to provide the same information and functionality in an accessible manner when non-conforming versions of that content exist.

An alternate version of content must pass all applicable Test Conditions to be considered a “conforming alternate version” as defined by WCAG. The results from this test are used to determine if WCAG's Conforming Alternate Version requirements are met.

Alternate versions could be identified and presented in a number of ways, such as:
-	an accessibility mode provided on a web page
-	a link pointing to an accessible alternate
-	allowing users to customize preferences on the web page.

**Methods**
-	Manual inspection
-	Methods used in applicable Test Conditions.

**Tools**

-	All tools in applicable Test Conditions.

Test ID	Test Name	Test Condition
1.A	alt-version-conformant	The identified version passes all applicable Test Conditions in this test process.

|  Test ID  | Test Name              | Test Condition    |
| --------- | ---------------------- |  -------------    |
| 1.A       | alt-version-conformant | The identified version passes all applicable Test Conditions in this test process.   |


**Identifying Content**

Alternate versions may be provided for a part of the page, entire pages, or an entire site. Some indications that alternate versions may be present include:
-	Instructions that describe how to enable accessibility
-	Content identified as the accessible version
-	Multiple methods provided to complete a task, such as a calendar widget and a text field to enter a date. Content could be a part of a web page. It does not need to be an entire web page.
-	A link or a version for assistive technology, such as screen reader versions
-	User preferences or settings to enable accessibility
-	User controls to modify colors and text appearance.

If found, check if any of these have been identified as a conforming alternate version.

Users must be made aware if a conforming alternate version is provided, so that they have the option of using that version rather than a non-conforming version. As such, conforming alternate versions must be identified for users. For example, if content or functionality is provided in multiple ways on the same page at the same time, one version must be identified as the accessible version.

Conforming alternate versions can be identified by various means, such as:
-	Instructions that describe how to enable accessibility
-	Content identified as the accessible version
-	A link or a version for assistive technology, such as screen reader versions.

Where user settings or preferences are provided for accessibility, they can be considered as indirect identification of conforming alternate versions, for example:
-	User preferences or settings to enable accessibility
-	User controls to modify colors and text appearance.

These lists are examples only and not meant to be exhaustive.

The alternate version does not need to reside within the scope of conformance or on the same website if it is as freely available as the non-conforming version. For example, the alternate version may be located on a different domain from the site you are testing. However, for this test process, the scope of testing is limited to web-based alternatives that are available in a browser on a desktop computer. Alternate versions do not include mobile applications that can only be accessed on a mobile device.

### Does Not Apply

This Test Condition **DOES NOT APPLY (DNA)** if:
-	there is only one version of content, or
-	if no versions are identified as the conforming alternate version/accessible version.

If there is more than one version and none are identified as the conforming alternate version or accessible version, assume there is no conforming alternate version and that these Conforming Alternate Version tests **DO NOT APPLY**. Perform tests 2-20 on all versions.

Depending on the scope of all the versions, for example if they are entire websites, you may want to check with the developer if any of those versions should have been identified as the conforming alternate version. If so, they should remediate this issue, and you can test the version they have identified as the conforming alternate version.

#### How to Test 1.A Accessible Alternate Version

**From the TT Process:**
1.	Enable accessibility settings (if necessary), select, and/or navigate to the version of content identified as the accessible alternate version.
2.	Following this test process, test the identified version of the content for all applicable Test Conditions. Record the result for the appropriate Test ID.
    a.	If no failures are found, this may be a conforming alternate version.
    b.	If a failure is found, the identified version is not a conforming alternate version.

Only content that is available in more than one version is evaluated in this test. Test the identified version against all applicable test conditions. For example, suppose there is a video with no captions. If a different file of the same video with captions is provided and identified as the conforming alternate version (or accessible version), your scope of testing for accessibility is the video file with captions. The video without captions only needs to be tested for 1.D Non-Interference.

If an accessibility setting is enabled and applies to the entire web page or site, the entire page or site content is the alternate version of content. Thus, the entire page or site should be fully accessible and meet ALL test process requirements. Any failures of the content would mean it is not an accessible alternate version.

As another example, suppose user controls for color contrast adjustment are provided on a web page, and are identified as provided for accessibility. To test, you would enable these color contrast settings. The scope of your testing would be the contrast adjustment feature and ALL the content affected by those settings.

#### Evaluating Content
**From the TT Process:**

If the following is TRUE, then the content PASSES; if the following is FALSE, then this Test Condition FAILS:
1.	The identified version of content passes all applicable Test Conditions in this test process.

#### Does Not Apply Examples

##### Example 1
You are testing a single web page that has a feedback form for your shopping experience. There is only one version of the content.
The content **DOES NOT APPLY** for 1.A Accessible Alternate Version because there is only one version of content. You also mark tests 1.B Equivalent Alternative through 1.D Non-Interference as DNA as well.

##### Example 2
You are testing a web page with a date input field. Users can use a calendar widget to select a date or enter the date manually in a text field. Neither is identified as the accessible or conforming alternate version.

Since there is no version of the content identified as the accessible or conforming alternate version, this test **DOES NOT APPLY** (DNA). Both versions of the date field remain in scope of testing; you should test both versions for other applicable tests. You also mark tests 1.B Equivalent Alternative through 1.D Non-Interference as DNA as well.

#### Passing Examples
##### Example 1
A web page offers median housing prices information in a table. The text before the table identifies it as the accessible version of this information.
 
There is also via a “View line graph” link that opens a graph showing the same information.

**Test for Topic 1.A Accessible Alternate Version**
**From the TT Process:**
1.	Enable accessibility settings (if necessary), select, and/or navigate to the version of content identified as the accessible alternate version.

You find that there are no accessibly settings for the site. The table is identified as the accessible alternate version.

**From the TT Process:**

2.	Following this test process, test the identified version of the content for all applicable Test Conditions. Record the result for the appropriate Test ID.

  a.	If no failures are found, this may be a conforming alternate version.

  b.	If a failure is found, the identified version is not a conforming alternate version.

Since the table is identified as the accessible version, the graph is out of testing scope and is only tested for 1.D Non-Interference. You start testing the table for every applicable Test Condition, such as 14 Tables. You find that it PASSES all applicable Test Conditions.

**Evaluate for Topic 1.A Accessible Alternate Version**

**From the TT Process:**

If the following is TRUE, then the content PASSES; if the following is FALSE, then this Test Condition FAILS:

1.	The identified version of content passes all applicable Test Conditions in this test process.
The content PASSES 1.A Accessible Alternate Version because ALL applicable results are TRUE.

##### Example 2
A web page has drag-and-drop controls to answer a quiz. There is a link to “Enable accessibility mode.”
 
Test for Topic 1.A Accessible Alternate Version
**From the TT Process:**
2.	Enable accessibility settings (if necessary), select, and/or navigate to the version of content identified as the accessible alternate version.
The site provides an option to “Enable Accessibility Mode.” You select this option, which redisplays the page with the same quiz question but a different set of controls which are keyboard accessible.
**From the TT Process:**
3.	Following this test process, test the identified version of the content for all applicable Test Conditions. Record the result for the appropriate Test ID.
a.	If no failures are found, this may be a conforming alternate version.
b.	If a failure is found, the identified version is not a conforming alternate version.
Since this is the version is identified for accessibility, you start testing it for every applicable Test Condition. You determine that the identified version passes every applicable Test Condition.
Evaluate for Topic 1.A Accessible Alternate Version
**From the TT Process:**
If the following is TRUE, then the content PASSES; if the following is FALSE, then this Test Condition **DOES NOT APPLY** (DNA):
1.	There is an accessible alternate version of content that passes all applicable Test Conditions in this test process.
The content PASSES for 1.A Accessible Alternate Version because ALL applicable results are TRUE.

#### Failing Examples
##### Example 1
A web page offers user controls to modify the color contrast. It provides four custom color palettes and a default option. You identify the option to change colors as a method to provide an accessible version of the content.
 
**Test for Topic 1.A Accessible Alternate Version**

**From the TT Process:**

1.	Enable accessibility settings (if necessary), select, and/or navigate to the version of content identified as the accessible alternate version.
You identify that the accessible version is provided through the user controls for changing the color settings. Since the entire page is modified by this accessibility setting, the entire page is within the scope of testing. You enable the “yellow on black” color option. Selecting colors changes all text color and the background color of the page to yellow text against a black background.

**From the TT Process:**

 a.	Following this test process, test the identified version of the content for all applicable Test Conditions. Record the result for the appropriate Test ID.

If no failures are found, this may be a conforming alternate version.

If a failure is found, the identified version is not a conforming alternate version.

The settings provide some accessible high contrast options. However, you determine that the page fails some other applicable Test Conditions, such as 11.A Language of Page.

**Evaluate for Topic 1.A Accessible Alternate Version**

**From the TT Process:**

If the following is TRUE, then the content PASSES; if the following is FALSE, then this Test Condition FAILS:

1.	The identified version of content passes all applicable Test Conditions in this test process.
The identified version FAILS 1.A Accessible Alternate Version because it failed one or more applicable test conditions.

#### Summary for Test ID 1.A 
| Test ID     | Test Name    | Test Condition |
| ------------- | ------------- | ------------- |
| 1.A	 | alt-version-conformant | The identified version passes all applicable Test Conditions in this test process.|

Test ID *1.A (alt-version-conformant)* requires that any versions of content identified as accessible alternatives PASSES all applicable Test Conditions. Remember that while alternate versions may be identified directly, they may also be identified indirectly, such as by providing user settings for accessibility.


## 1.B Equivalent Alternative
**Test Requirement**

The purpose of this test is to verify that the identified version from 1.A Accessible Alternate Version provides the same information and functionality as the non-conforming version.  The identified version needs to have content in the same human language and provide up-to-date information. This ensures that the identified version provides equivalent information and content. The results from this test are used to determine if WCAG’s Conforming Alternate Version requirements are met.

**Methods**
-	Manual inspection.

**Tools**
-	None.

|  Test ID  | Test Name              | Test Condition    |
| --------- | ---------------------- |  -------------    |
| 1.B       | alt-version-equivalent | The identified version is up to date with the same information and functionality.  |


**Identifying Content**

Continue testing the identified version from 1.A Accessible Alternate Version.

### Does Not Apply

This Test Condition **DOES NOT APPLY** (DNA) if Test ID 1.A Accessible Alternate Version was DNA.

#### How to Test 1.B Equivalent Alternative

**From the TT Process:**
1.	Continue from Test 1.A Accessible Alternate Version.
2.	Review the content of the non-conforming version.
3.	Verify that the identified version has the same information, functionality, and language as the non-conforming version.
The accessible version does not need to match the non-conforming version page for page. One version may consist of fewer pages than the other. However, they both need to be equally up to date in information and functionality to be considered equivalent.
Verify that the information in each version uses the same human language.


#### Evaluating Content
If the following is TRUE, then the content PASSES; if the following is FALSE, then this Test Condition FAILS:

1.	The identified version provides all the same information and functionality in the same human language as the non-conforming content.

The accessible version that passes this 1.B Equivalent Alternative test will be referred to as the “accessible equivalent version” in subsequent tests.

#### Does Not Apply Examples
##### Example 1
You are testing a web page that generates reports. As there is no alternate version identified for the web page or any of its content, you mark Test ID 1.A Accessible Alternate Version as **DOES NOT APPLY** (DNA).

The content **DOES NOT APPLY** (DNA) for 1.B Equivalent Alternative because there was only one version of the content and therefore Test ID 1.A Accessible Alternate Version was marked as **DOES NOT APPLY** (DNA).


#### Passing Examples
##### Example 1
A web page offers information on median house prices in two ways. The information is available through a table and an image of a graph, showing the same information on the same page. Text on the page identifies the table as the accessible alternate version.
 
**Test for Topic 1.B Equivalent Alternative**
**From the TT Process:**
1.	Continue from Test 1.A Accessible Alternate Version.

The table is identified as the accessible alternate version.
**From the TT Process:**
2.	Review the content of the non-conforming version.

You review the content of the non-conforming graph.
 
**From the TT Process:**
3.	Verify that the identified version has the same information, functionality, and language as the non-conforming version.

You compare the table with the non-conforming graph and see that they present equivalent information and functionality in the same human language.
 
**Evaluate for Topic 1.B Equivalent Alternative**

**From the TT Process:**

If the following is TRUE, then the content PASSES. If the following is FALSE, then this Test Condition FAILS:

1.	The identified version provides all the same information and functionality in the same human language as the non-conforming content.
TRUE: The identified version, the table, provides ALL the same information and functionality in the same human language as the non-conforming content.
The content PASSES 1.B Equivalent Alternative because the test result is TRUE.

##### Example 2

A web page offers user controls to modify the color contrast by providing four custom color palettes and a default option. A user can select any color combination to view the web page. You identify the option to change colors as a method to provide a version for accessibility purposes.
 
**Test for Topic 1.B Equivalent Alternative**

**From the TT Process:**
1.	Continue from Test 1.A Accessible Alternate Version.

When you select a color contrast setting, the setting affects all the text on the current page.

**From the TT Process:**
2.	Review the content of the non-conforming version:
 
**From the TT Process:**
3.	Verify that the identified version has the same information, functionality, and language as the non-conforming version.

You review the yellow-on-black version and notice it is the same as the default version except for the change in color.
 
**Evaluate for Topic 1.B Equivalent Alternative**

**From the TT Process:**

If the following is TRUE, then the content PASSES. If the following is FALSE, then this Test Condition FAILS:
1.	The identified version provides all the same information and functionality in the same human language as the non-conforming content.

TRUE: The content in the accessible version provides the same information and functionality in the same language as the non-conforming content.

The content PASSES 1.B Equivalent Alternative because the test results are TRUE.

#### Failing Examples
##### Example 1
A meeting scheduling website offers two ways to input a date. You can either type the date in the Date text field or use a date picker control. There is a link before the date field labeled “Accessibility info.”

Since multiple methods are provided to input the date, you check if either method is identified as the accessible version. Clicking on the “Accessibility info” link opens a page that says that text fields are the accessible version of the date fields.

**Test for Topic 1.B Equivalent Alternative**

**From the TT Process:**
1.	Continue from Test 1.A Accessible Alternate Version.

The date text field was identified as the accessible version of the non-conformant date picker.

**From the TT Process:**

2.	Review the content of the non-conforming version.
**From the TT Process:**

4.	Verify that the identified version has the same information, functionality, and language as the non-conforming version.

You review the content on the non-conforming date picker and compare it to the identified version, and see they are both in the same human language. However, the text field does not offer the same information when inserting a date. The date picker offers the ability to identify what day of the week you are trying to select. This information can be very beneficial. For example, when scheduling a meeting, it can help ensure it is not inappropriately scheduled for a weekend. Also, selecting a date from the date picker automatically enters a date in the expected date format. However, the text field does not provide information on the expected date format.

**Evaluate for Topic 1.B Equivalent Alternative**

**From the TT Process:**

If the following is TRUE, then the content PASSES. If the following is FALSE, then this Test Condition FAILS:
1.	The identified version provides all the same information and functionality in the same human language as the non-conforming content.

FALSE: The text field does not provide the same information as the date picker.
The content FAILS for 1.B Equivalent Alternative because the result is FALSE.

##### Example 2
You are testing a website that allows users to enable an accessibility mode that applies to the entire web page.

**Test for Topic 1.B Equivalent Alternative**

**From the TT Process:**
1.	 Continue from Test 1.A. Accessible Alternate Version.

**From the TT Process:**
2.	 Review the content of the non-conforming version.

**From the TT Process:**
3.	Verify that the identified version has the same information, functionality, and language as the non-conforming version.

With accessibility mode enabled, you review the content and notice that the accessible version is not all in English. It appears that two sentences are now in French, with no English translation.

**Evaluate for Topic 1.B Equivalent Alternative**
**From the TT Process:**

If the following is TRUE, then the content PASSES. If the following is FALSE, then this Test Condition FAILS:
1.	The identified version provides all the same information and functionality in the same human language as the non-conforming content.

FALSE: The identified version does not provide the same information in the same human language. There are two sections in French only, with no English translation.
The content FAILS for 1.B Equivalent Alternative because the result is FALSE.

##### Example 3
A web page offers median house price information in a table. There is also a link that, when selected, shows a graphic of the same information.
 
**Test for Topic 1.B Equivalent Alternative**
**From the TT Process:**
1.	Continue from Test 1.A Accessible Alternate Version.
**From the TT Process:**
2.	Review the content of the non-conforming version.
You select the link to view the line graph and review the content of the non-conforming version.
 
**From the TT Process:**
3.	Verify that the identified version has the same information, functionality, and language as the non-conforming version.
The data table only includes the data points from the graph. It is missing a statement about the trend of decreasing housing prices between 2014 and 2018 that was highlighted on the bar graph.
**From the TT Process:**
If the following is TRUE, then the content PASSES. If the following is FALSE, then this Test Condition FAILS:
1.	The identified version provides all the same information and functionality in the same human language as the non-conforming content.
FALSE: The data table is missing specific information about the trend of decreasing housing prices between 2014 and 2018 that was highlighted on the bar graph.
The content FAILS for 1.B Equivalent Alternative because the result is FALSE.

#### Summary for Test ID 1.B
| Test ID     | Test Name    | Test Condition |
| ------------- | ------------- | ------------- |
| 1.B	 | alt-version-equivalent | The identified version is up to date with the same information and functionality.|

Test ID 1.B (alt-version-equivalent) requires that the identified version has the same information, functionality, and language as the non-conforming version. However, they do not have to match page for page.

 
## 1.C Conformant Mechanism
**Test Requirement**

In this test and the next, you will determine how the identified version is accessed by the user.
This Test ID covers how to test the mechanism the user takes to access the accessible equivalent version. The mechanism must conform to all applicable Test Conditions. The results from this test are used to determine if WCAG’s Conforming Alternate Version requirements are met.

**Methods**
-	Manual inspection.

**Tools**
-	Tools used in applicable Test Conditions.

| Test ID     | Test Name    | Test Condition |
| ------------- | ------------- | ------------- |
| 1.C	 | alt-version-access | The mechanism to reach the identified version is accessible.|


**Identifying Content**

Identify the mechanism used to access the identified version. Various mechanisms may be used to reach the identified version, such as:
-	A link to the identified version or a version for assistive technology (e.g., screen reader version)
-	User preferences or settings to enable accessibility for a page or the entire site
-	User controls to modify colors and text appearance of the page or entire site
-	Navigating to the identified accessible version of content on a page
-	A button, link, or hotkey combination
-	Providing the accessible equivalent version on the same page as the non-conforming version
-	Text before a link to the accessible version stating that the link leads to the accessible version.
-	Hiding non-conforming content from assistive technologies (AT) or excluding it from keyboard focus, so that users with disabilities only access the accessible version.

A mechanism is widely defined as a process or technique for achieving a result. It may be explicitly provided in the content, or it may be provided by the platform or user agents, including AT. For example:
-	A keyboard-only user would rely on the operating system and browser’s functionality to navigate using the keyboard, such as the Tab or Arrow keys.
-	A screen reader user would likely rely on additional features provided by their screen reader to navigate the content of a web page, such as custom shortcut keys.

### Does Not Apply
This Test Condition **DOES NOT APPLY** (DNA) if Test ID 1.A Accessible Alternate Version was DNA.

### How to Test 1.C Conformant Mechanism
**From the TT Process:**
1.	Perform Tests 2 through 20 for the mechanism used to reach the identified version.

### Evaluating Content
**From the TT Process:**

If the following is TRUE, then the content PASSES; if the following is FALSE, then this Test Condition FAILS:
1.	The mechanism used to reach the accessible equivalent version passes all applicable Test Conditions.

#### Does Not Apply Examples
##### Example 1
You are testing a single web page of a feedback form for a recent shopping experience. There is only one version of the content.
The content **DOES NOT APPLY** (DNA) for 1.A Accessible Alternate Version since there is only one version of the content. As such, 1.C Conformant Mechanism does not apply.


#### Passing Examples
##### Example 1
A web page offers information on median house prices in two ways. The information is available through a table and an image of a graph, showing the same information on the same page side by side. The page identifies the table as the accessible alternate version.
 
You first identify how the accessible equivalent version is accessed. You determine that the mechanism used is to present both versions side by side on the same page.
**Test for Topic 1.C Conformant Mechanism**

**From the TT Process:**
1.	Perform Tests 2 through 20 for the mechanism used to reach the identified version.

Both versions of the content are presented on the same page, side by side. No special interactions are needed to access the identified version. As such, the only applicable mechanisms to access the content are techniques to navigate the web page, such as a keyboard or pointing device. Therefore, no additional Test Conditions apply.

**Evaluate for Topic 1.C Conformant Mechanism** 

**From the TT Process:**

If the following is TRUE, then the content PASSES; if the following is FALSE, then this Test Condition FAILS:
1.	The mechanism used to reach the accessible equivalent version passes all applicable Test Conditions.

TRUE: There are no other Test Conditions that apply since the mechanism does not require any additional user interaction.
The content PASSES 1.C Conformant Mechanism because the results are TRUE.

##### Example 2
A web page offers user controls to modify the color contrast by providing four custom color palettes and a default option. A user can select any color combination to view the web page. You identify the option to change colors as the mechanism to provide a version for accessibility purposes.
 
**Test for Topic 1.C Conformant Mechanism**
**From the TT Process:**
1.	Perform Tests 2 through 20 for the mechanism used to reach the identified version.

You return to the default page setting, which contains non-conforming content and the mechanism, the user controls for changing the text colors. You test the mechanism for all applicable tests. The mechanism passes all applicable Test Conditions.

**Evaluate for Topic 1.C Conformant Mechanism**

**From the TT Process:**
If the following is TRUE, then the content PASSES; if the following is FALSE, then this Test Condition FAILS:
1.	The mechanism used to reach the accessible equivalent version passes all applicable Test Conditions.
TRUE: The mechanism PASSES all applicable Test Conditions.
The content PASSES 1.C Conformant Mechanism because the results are TRUE.

#### Failing Examples
Example 1
A web page provides a line graph of house pricing information. Below the graph is a link that reads “View accessible version,” which leads to an accessible equivalent version. The link is not keyboard accessible.
 
**From the TT Process:**
1.	Perform Tests 2 through 20 for the mechanism used to reach the identified version.
You find that the link is not keyboard accessible.
**From the TT Process:**
If the following is TRUE, then the content PASSES; if the following is FALSE, then this Test Condition FAILS:
1.	The mechanism used to reach the accessible equivalent version passes all applicable Test Conditions.
FALSE: The mechanism fails the test for keyboard accessibility.
The content FAILS 1.C Conformant Mechanism because the result is FALSE.

Summary for Test ID 1.C
Test ID	Test Name	Test Condition
1.C	alt-version-access	The mechanism to reach the identified version is accessible.
Test ID 1.C (alt-version-access) requires that the mechanism to access the identified version PASSES all applicable Test Conditions. The mechanism can include links, buttons, user preferences, instructions, and other methods.

 
1.D Non-Interference
Test Requirement
The purpose of this test is to verify that the non-conforming content from the preceding tests does not interfere or block the user’s ability to interact with the conforming content. By performing five specific tests on the non-conforming content, you will verify that the web page:
-	Allows users to pause, stop, or control volume of audio content that plays automatically, AND
-	Allows users to pause, stop, or hide moving, blinking, or scrolling content, AND
-	Allows users to stop, pause, hide, or control the frequency of any automatically updating content, AND
-	Has no flashing content present, AND
-	Has no keyboard trap.
Non-interference requirements apply to ALL content on a web page. This includes non-conforming content that has a conforming alternate version, because a failure could interfere with further use of the page. While a conforming alternate version of content might have been confirmed under Tests 1.A through 1.C, a content owner CANNOT make a claim of conformance to the Section 508 standards if ANY version of content fails Test 1.D Non-interference. This includes content that is not otherwise relied upon to meet conformance.
The results from this test are used to determine if WCAG Conformance Requirement 5 is met.
Methods
-	Methods used in applicable Test Conditions.
Tools
-	Tools used in applicable Test Conditions.
Test ID	Test Name	Test Condition
1.D	non-interference	Content in the non-conforming version(s) meets Conformance Requirement 5.
Identifying Content
The non-conforming version(s) of the content. Exclude the version identified as the accessible version.
Does Not Apply
This Test Condition **DOES NOT APPLY** (DNA) if Test ID 1.A Accessible Alternate Version was DNA.
How to Test 1.D Non-Interference
**From the TT Process:**
1.	If necessary and/or applicable, disable accessibility features within site setting or preferences.
2.	Perform ONLY the following tests on the non-conforming version(s) of the content:
a.	Test ID 2.A Audio Control
b.	Test ID 2.B Blinking, Moving, and Scrolling
c.	Test ID 2.C Auto-Updating
d.	Test ID 3.A Flashing
e.	Test ID 4.C Keyboard Trap.
3.	Enter test results for the appropriate Test IDs listed above.
4.	Do not perform any further testing on the non-conforming version(s) of the content.
Evaluating Content
**From the TT Process:**
If the following is TRUE, then the content PASSES. If the following is FALSE, then this Test Condition FAILS:
1.	The results for each of the following tests are PASS or **DOES NOT APPLY** for all non-conforming version(s) of the content.
a.	Test ID 2.A Audio Control
b.	Test ID 2.B Blinking, Moving, and Scrolling
c.	Test ID 2.C Auto-Updating
d.	Test ID 3.A Flashing – Must be **DOES NOT APPLY**
e.	Test ID 4.C Keyboard Trap
The results for all these five tests must be either **DOES NOT APPLY** or PASS. If any of these five tests FAIL, then the result of this test is FAILS.
3.A Flashing must have a test result of **DOES NOT APPLY** in order to meet 1.D Non-interference. A test result of NOT TESTED does not meet the 1.D Test Condition. See Test ID 3.A Flashing for further details.
After performing this test on the non-conforming version of content that has a conforming alternate version, you can omit the non-conforming content from further testing.

Does Not Apply Examples
Example 1
You are testing a single web page of a feedback form for a recent shopping experience. There is only one version of the content. Since there is only one version of content, this example was marked **DOES NOT APPLY** for 1.A Accessible Alternate Version. As such, it is also DNA for 1.D Non-Interference.

Passing Examples
Example 1
You are testing a new version of the web page and determine that the developer has offered median house content in more than one way. It is available through an accessible table and an image of a graph, showing the same information on the same page side by side.
You already tested this page for 1.A Accessible Alternate Version through 1.C Conformant Mechanism and determined that it passed all applicable test conditions.
 
Test for Topic 1.D Non-Interference
**From the TT Process:**
1.	If necessary and/or applicable, disable accessibility features within site settings or preferences.
There are no accessibility features provided.
**From the TT Process:**
2.	Perform ONLY the following tests on the non-conforming version(s) of the content:
a.	Test ID 2.A Audio Control
b.	Test ID 2.B Blinking, Moving, and Scrolling
c.	Test ID 2.C Auto-Updating
d.	Test ID 3.A Flashing
e.	Test ID 4.C Keyboard Trap
You determine that the non-conforming content is the graph. You did not find any audio, auto-playing, auto-updating, or flashing content, so these tests do not apply. There are no keyboard traps.
Evaluate for Topic 1.D Non-Interference
**From the TT Process:**
If the following is TRUE, then the content PASSES. If the following is FALSE, then this Test Condition FAILS:
1.	The results for each of the following tests are PASS or **DOES NOT APPLY** for all non-conforming version(s) of the content.
a.	Test ID 2.A Audio Control.
DNA: There is no auto-playing audio content.
**From the TT Process:**
b.	Test ID 2.B Blinking, Moving, and Scrolling
DNA: There is no moving, blinking, or scrolling content.
**From the TT Process:**
c.	Test ID 2.C Auto-Updating
DNA: There is no auto-updating content.
**From the TT Process:**
d.	Test ID 3.A Flashing
DNA: There is no flashing content.
**From the TT Process:**
e.	Test ID 4.C Keyboard Trap
PASS: You do not find a keyboard trap.
The results for each of the five applicable Test Conditions are PASS or DNA. There is no other non-conforming version of this content. The content PASSES 1.D Non-Interference because the result is TRUE.
After performing this test on this non-conforming version of the content, you omit testing of this non-conforming content from the rest of your testing.
Example 2
A web page offers user controls to modify the color contrast by providing four custom color palettes and a default option. A user can select any color combination to view the web page. You identify the option to change colors as the mechanism to provide a version for accessibility purposes.
You already determined that this page passed for 1.A Accessible Alternate Version through 1.C Conformant Mechanism.
 
Test for Topic 1.D Non-Interference
**From the TT Process:**
You already determined that this page passed for 1.A Accessible Alternate Version through 1.C Conformant Mechanism.
1.	If necessary and/or applicable, disable accessibility features within site settings or preferences.
You disable the any contrast options by selecting “Reset to default.”
**From the TT Process:**
2.	Perform ONLY the following tests on the non-conforming version(s) of the content:
a.	Test ID 2.A Audio Control
b.	Test ID 2.B Blinking, Moving, and Scrolling
c.	Test ID 2.C Auto-Updating
d.	Test ID 3.A Flashing
e.	Test ID 4.C Keyboard Trap
You determine that the non-conforming content is the web page with the color options disabled. You did not find any audio, auto-playing, auto-updating, or flashing content, so these tests do not apply. There are no keyboard traps.
Evaluate for Topic 1.D Non-Interference
**From the TT Process:**
If the following is TRUE, then the content PASSES. If the following is FALSE, then this Test Condition FAILS:
1.	The results for each of the following tests are PASS or **DOES NOT APPLY** for all non-conforming version(s) of the content.

a.	Test ID 2.A Audio Control.
DNA: There is no auto-playing audio content.
**From the TT Process:**
b.	Test ID 2.B Blinking, Moving, and Scrolling
DNA: There is no moving, blinking, or scrolling content.
**From the TT Process:**
c.	Test ID 2.C Auto-Updating
DNA: There is no auto-updating content.
**From the TT Process:**
d.	Test ID 3.A Flashing
DNA: There is no flashing content.
**From the TT Process:**
e.	Test ID 4.C Keyboard Trap
PASS: You do not find a keyboard trap.
The results for each of the five applicable Test Conditions are PASS or DNA. There is no other non-conforming version of this content. The content PASSES 1.D Non-Interference because the result is TRUE.
After performing this test on this non-conforming version of the content, you omit testing of this non-conforming content from the rest of your testing.

Failing Examples
Example 1
You are testing a web page that has accessibility mode enabled by default, but users can also choose to toggle the accessibility mode off or on.
 
Test for Topic 1.D Non-Interference
**From the TT Process:**
1.	If necessary and/or applicable, disable accessibility features within site settings or preferences.
You disable accessibility mode. You determine the non-conforming content is the entire web page with accessibility mode disabled.
**From the TT Process:**
2.	Perform ONLY the following tests on the non-conforming version(s) of the content:
a.	Test ID 2.A Audio Control
b.	Test ID 2.B Blinking, Moving, and Scrolling
c.	Test ID 2.C Auto-Updating
d.	Test ID 3.A Flashing
e.	Test ID 4.C Keyboard Trap
You check for any instances where any of the tests above produces a result of FAIL or NOT TESTED (for Test ID 3.A Flashing).
You notice that there is continually flashing content at the top of each page. The flashing is at different rates and does not stop. Because of this, people with attention deficit disorder may become distracted, and those with photosensitive seizure disorders may have seizures. You mark 3.A Flashing as NOT TESTED.
Evaluate for Topic 1.D Non-Interference
**From the TT Process:**
If the following is TRUE, then the content PASSES. If the following is FALSE, then this Test Condition FAILS:
1.	The results for each of the following tests are PASS or **DOES NOT APPLY** for all non-conforming version(s) of the content.
a.	Test ID 2.A Audio Control
b.	Test ID 2.B Blinking, Moving, and Scrolling
c.	Test ID 2.C Auto-Updating
d.	Test ID 3.A Flashing
e.	Test ID 4.C Keyboard Trap
FALSE: Since there is flashing content on the web page, you mark 3.A Flashing as NOT TESTED.
Since 3.A Flashing is not PASS or DNA, the test condition is FALSE and FAILS. You also mark 3.A Flashing as NOT TESTED.
The content FAILS 1.D Non-Interference because the test result is FALSE.
Example 2
A web page has an alternate conforming version which has passed all applicable tests. The non-conforming content is found towards the bottom half of the page.
Test for Topic 1.D Non-Interference
**From the TT Process:**
1.	The non-conforming content that has a conforming alternate version must be tested prior to omitting the content from the rest of testing.
You locate the non-conforming content at the bottom half of the web page.
**From the TT Process:**
2.	If necessary and/or applicable, disable accessibility features within site settings or preferences.
There are no accessibility settings to disable.
**From the TT Process:**
3.	Perform ONLY the following tests on the non-conforming version(s) of the content:
a.	Test ID 2.A Audio Control
b.	Test ID 2.B Blinking, Moving, and Scrolling
c.	Test ID 2.C Auto-Updating
d.	Test ID 3.A Flashing
e.	Test ID 4.C Keyboard Trap
When testing the non-conforming version for 4.C Keyboard Trap, the keyboard focus gets stuck in a loop. As this creates a keyboard trap, it FAILS Test ID 4.C Keyboard Trap.
Evaluate for Topic 1.D Non-Interference
**From the TT Process:**
If the following is TRUE, then the content PASSES. If the following is FALSE, then this Test Condition FAILS:
1.	The results for each of the following tests are PASS or **DOES NOT APPLY** for all non-conforming version(s) of the content.
a.	Test ID 2.A Audio Control
b.	Test ID 2.B Blinking, Moving, and Scrolling
c.	Test ID 2.C Auto-Updating
d.	Test ID 3.A Flashing
e.	Test ID 4.C Keyboard Traps
FALSE:  Since Test ID 4.C Keyboard Trap FAILS, the test condition is FALSE and the test FAILS.
You also record this failure under Test ID 4.C Keyboard Trap.
The content FAILS 1.D Non-Interference because the test result is FALSE.

Summary for Test ID 1.D
Test ID	Test Name	Test Condition
1.D	non-interference	Content in the non-conforming version(s) meets Conformance Requirement 5.
Test ID 1.D (non-interference) requires that the non-conforming versions of content do not have elements that could interfere with a user’s ability to access the accessible versions. This includes auto-playing content that cannot be controlled, flashing content, and keyboard traps.

Topic Summary
Test ID 1.A (alt-version-conformant) requires that any versions of content identified as accessible alternatives PASSES all applicable Test Conditions. Remember that while alternate versions may be identified directly, they may also be identified indirectly, such as by providing user settings for accessibility.
Test ID 1.B (alt-version-equivalent) requires that the identified version has the same information, functionality, and language as the non-conforming version.
Test ID 1.C (alt-version-access) requires that the mechanism to access the identified version PASSES all applicable Test Conditions. The mechanism can include links, buttons, user preferences, instructions, and other methods.
Test ID 1.D (non-interference) requires that the non-conforming versions of content do not have elements that could interfere with a user’s ability to access the accessible versions. This includes auto-playing content that cannot be controlled, flashing content, and keyboard traps.
