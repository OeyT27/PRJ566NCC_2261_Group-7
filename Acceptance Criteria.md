ConnectHub Acceptance Criteria

1. **Identity and Access**

- **Registration and verification**: User must be able to create and verify the account via email; account remains unactive until verified
- **Secure Access:** Users must be able to login to their account or be able to reset password
- **Session Integrity:** System must support persistent login across app restarts but allow for a complete session termination upon manual logout

- **Career Navigation (Profile and Pathway)**

- **Profile Management**: Users can update or save their personal data, which includes professional background data
- **Intelligent Guidance:** The system must generate at least 3 career recommendation that has relation to the users background
- **Visual RoadMap:** Users can view pathway careers that outline the next step and milestones they have achieve and what else to be done

- **Opportunity Discovery**

- **Search & Filtering:** Users can make key word searches or filters with instant results for any positions available or events for specific searches
- **Engagement:** The "Opportunity Detail" view will display all relevant details and users are able to bookmark events

- **Application Management**

- **Submission Workflow:** Users can submit an application which includes the ability to upload a document of their background
- **Status Tracking:** Users can track the status of their application and see real time progress of what employers decide and may also have the option to withdraw a application

- **Community and Networking**

- **Event Discovery:** User can browse for a lists of communities and events to join as well as filter by interest
- **Networking:** System suggests communities that show and organizations that allow the user to market themselves and put their name out

- **Communication**

- **Alert Accuracy:** System allows user to receive notification in order to be aware of any new events, job positions, or application status of a employment position
- **User Control:** The system provides a settings menu that allows the user how they would like to receive their notification.

- **Administrative Control**

- **Content Moderation:** Admin have the power to approve any events, job opportunities, and job applications that are able to be posted on the system
- **Analytics:** The Admin Panel must display-real time usage metrics such as active users, total applications, etc and able to be exported

- **Infrastructure and Security**

- **Backend and API:** All frontend actions must communicate via a documented API with a response of over 95% success under standard locals
- **Cloud and CI/CD:** The system must be fully deployed on AWS, with a CI/CD pipeline that automatically runs unit integration tests before deploying
- **Security:** All data that is being passed through will all be encrypted from personal information to job applications being sent out.
