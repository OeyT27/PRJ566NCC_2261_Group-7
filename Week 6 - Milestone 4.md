# Section 3

3.1 Data Flow Diagrams

3.3.1 DFD Level 0 (CD)  
  
3.3.2 DFD Level 1

# 3.2 User Stories and related Use Case Scenarios

## **User Story 1: Account Registration and Profile Creation**

**User Story:**  
As a newcomer job seeker, I want to create an account and complete my profile so that I can receive personalized career recommendations and apply for opportunities.

### **Use Case Name: Register Account and Create Profile**

**Use Case Name:** Register Account and Create Profile  
**Related Use Case:** Login  
**Actors:** Newcomer Job Seeker, ConnectHub System  
**Description:** User registers a new account and creates a career profile to access ConnectHub services.  
**Preconditions:**

- User has internet access
- User is not already registered

**Postconditions:**

- User account is successfully created
- User profile is stored and available for future sessions

**Main Flow:**

|     |     |
| --- | --- |
| **Actor** | **System** |
| Opens ConnectHub website using browser | Loads homepage and displays Sign Up and Login options |
| Selects "Sign Up" option | Displays user registration form |
| Enters required information (name, email, password) | Validates entered information |
| Submits registration form | Creates new user account in database<br><br>Displays confirmation message |
| Proceeds to profile setup page | Displays profile creation form |
| Enters education, experience, career interests, and preferences | Validates profile information |
| Submits profile form | Saves profile data in system database<br><br>Displays confirmation and redirects user to dashboard |

## **User Story 2: View Personalized Career Pathway**

**User Story:**  
As a newcomer job seeker, I want to view personalized career recommendations so that I know what steps to take for my career in Canada.

### **Use Case Name: View Career Recommendations**

**Use Case Name:** View Career Recommendations  
**Related Use Case:** Profile Management  
**Actors:** Newcomer Job Seeker, ConnectHub System  
**Description:** System generates and displays personalized career pathway recommendations.

**Preconditions:**

- User is logged into system
- User profile exists

**Postconditions:**

- Career recommendations are displayed
- User can view recommended certifications and training

### **Main Flow:**

|     |     |
| --- | --- |
| **Actor** | **System** |
| Logs into ConnectHub system | Authenticates user credentials |
|     | Displays personalized dashboard |
| Selects "Career Pathway" section | Retrieves user profile data |
| Requests career recommendations | Processes user profile data |
|     | Generates career pathway recommendations |
|     | Displays recommended certifications, training, and volunteer opportunities |
| Reviews recommendations | Allows user to explore detailed information |
| Selects recommendation | Displays additional details |

## **User Story 3: Search and Filter Opportunities**

**User Story:**  
As a newcomer job seeker, I want to search and filter opportunities so that I can find relevant jobs, training, or volunteer programs.

### **Use Case Name: Search Opportunities**

**Use Case Name:** Search Opportunities  
**Related Use Case:** Apply for Opportunity  
**Actors:** Newcomer Job Seeker, ConnectHub System  
**Description:** User searches and filters opportunities based on preferences.

**Preconditions:**

- Opportunities exist in system

**Postconditions:**

- Filtered opportunities are displayed
- User can view opportunity details

### **Main Flow:**

|     |     |
| --- | --- |
| **Actor** | **System** |
| Navigates to Opportunities section | Displays all available opportunities |
| Applies filters (location, industry, experience level) | Processes filter criteria |
|     | Retrieves matching opportunities |
|     | Displays filtered opportunities list |
| Selects specific opportunity | Retrieves opportunity details |
|     | Displays full opportunity information |
| Reviews opportunity | Provides Apply and Bookmark options |

## **User Story 4: Apply for Opportunity**

**User Story:**  
As a newcomer job seeker, I want to apply for opportunities so that I can submit my application easily.

### **Use Case Name: Apply for Opportunity**

**Use Case Name:** Apply for Opportunity  
**Related Use Case:** Search Opportunities  
**Actors:** Newcomer Job Seeker, ConnectHub System, Employer  
**Description:** User submits an application for selected opportunity.

**Preconditions:**

- User is logged in
- Opportunity exists

**Postconditions:**

- Application is submitted
- Application is stored in system

### **Main Flow:**

|     |     |
| --- | --- |
| **Actor** | **System** |
| Selects opportunity | Displays opportunity details |
| Clicks Apply button | Displays application form |
| Reviews auto-filled profile data | Retrieves profile information |
| Uploads required documents | Validates uploaded files |
| Submits application | Saves application data in database |
|     | Sends application confirmation message |
|     | Updates application status in user dashboard |

## **User Story 5: Bookmark Opportunities and Receive Notifications**

**User Story:**  
As a newcomer job seeker, I want to bookmark opportunities and receive notifications so that I do not miss important opportunities.

### **Use Case Name: Bookmark Opportunity**

**Use Case Name:** Bookmark Opportunity  
**Related Use Case:** Search Opportunities  
**Actors:** Newcomer Job Seeker, ConnectHub System  
**Description:** User bookmarks opportunity and receives updates.

**Preconditions:**

- User is logged in

**Postconditions:**

- Opportunity is saved in dashboard
- Notifications are enabled

### **Main Flow:**

|     |     |
| --- | --- |
| **Actor** | **System** |
| Views opportunity details | Displays opportunity information |
| Clicks Bookmark button | Saves opportunity in user profile |
|     | Confirms bookmark action |
| Navigates to dashboard | Displays bookmarked opportunities |
|     | Monitors updates for bookmarked opportunities |
|     | Sends notifications when updates occur |

# 3.3 Activity Diagrams3.4 Business Rules

|     |     |     |     |     |
| --- | --- | --- | --- | --- |
| **Business Rule #** | **Description** | **Activity Diagram** | **Related UCS** | **UI  <br>Mock-up** |
| BR1 | Users must register with a unique email address, duplicate emails are not allowed | AD1 | UC1 | UI 2.7.2 |
| BR2 | Users must complete required profile fields (education, experience, target field, location) before receiving career pathway recommendations | AD2 | UC2 | UI 2.7.3 |
| BR3 | Certification/training steps must appear before job application steps when they are marked as prerequisites | AD3 | UC3 | UI 2.7.4 |
| BR4 | A user may save opportunities; duplicates are not allowed in the saved list | AD3 | UC3 | UI 2.7.4 |
| BR5 | An application submission must include all required fields (resume or profile, contact info, and any employer required questions) | AD5 | UC4 | UI 2.7.6 |
| BR6 | Users must not submit more than one application to the same opportunity unless the employer explicitly allows re-application | AD6 | UC5 | UI 2.7.6 |
| BR7 | The system must send reminders for saved events before the event date, unless reminders are disabled | AD7 | UC6 | UI 2.7.7 |
| BR8 | Users must verify their email before submitting any application through the portal | AD8 | UC7 | UI 2.7.8 |
| BR9 | Passwords must meet minimum strength rules and must not match common weak passwords | AD8 | UC7 | UI 2.7.8 |
| BR10 | User sessions must automatically expire after a period of inactivity to reduce unauthorized access risk | AD8 | UC7 | UI 2.7.8 |
| BR11 | Employer or training-provider accounts must be approved by an admin before posting opportunities | AD8 | UC7 | UI 2.7.8 |
| BR12 | The system must flag listings with similar titles, dates, and descriptions to prevent duplicates and spam | AD8 | UC7 | UI 2.7.8 |
| BR13 |     | AD9 | UC8 | UI 2.7.9 |
| BR14 |     | AD9 | UC8 | UI 2.7.9 |
| BR15 |     | AD9 | UC8 | UI 2.7.9 |
| BR16 |     | AD9 | UC8 | UI 2.7.9 |
| BR17 |     | AD10 | AD9 | UI 2.7.9 |
| BR18 |     | AD10 | AD9 | UI 2.7.9 |
| BR19 |     | AD10 | AD9 | UI 2.7.9 |
| BR20 |     | AD11 | UC10 | UI 2.7.10 |
| BR21 |     | AD11 | UC10 | UI 2.7.11 |
| BR22 |     | AD11 | UC10 | UI 2.7.11 |
| BR23 |     | AD12 | UC11 | UI 2.7.10 |
| BR24 |     | AD13 | UC12 | UI 2.7.12 |
