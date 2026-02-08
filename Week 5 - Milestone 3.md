# 2.6 Functional Requirements

ConnectHub provide the following core functionalities to ensure newcomers can effectively explore career pathways, discover opportunities, and make informed decisions about their professional growth. These functional requirements define what the system must do to meet user and stakeholder needs.

**2.6.1 User Story Interviews**

**User Interview**

- **Name:** Venky Reddy
- **Age:** 29
- **Occupation:** Civil Engineer (International Experience)
- **Status:** Newcomer to Canada
- **Background:** Holds international degree with 6 years of experience
- **Current Challenge:** Difficulty understanding Canadian certifications and local job expectations

**When you arrived in Canada, what was your biggest challenge in finding a job related to your experience?**

"I didn't know where to start. I kept applying on job boards, but I wasn't sure if my experience was even being considered. I didn't know which certifications I needed or how to build local experience."

**What kind of support would help you most right now?**

"Clear guidance. I want someone or something to tell me what steps I should take - training, volunteering, certifications - instead of just showing job listings."

**Would you like recommendations based on your background and culture?**

"Yes, that would help a lot. It feels more comfortable to attend events or programs where I can relate to others from similar backgrounds."

**Would you create an account to save progress and recommendations?**

"Definitely. I want to track my progress and come back later without starting over every time."

**Stakeholder Interview**

- **Name:** Lisa Martin
- **Role:** Community Employment Coordinator

**How do you see ConnectHub helping newcomers?**

"A centralized platform that combines jobs, training, and community support would reduce confusion and save newcomers months of trial and error."

**What kind of data or reports would be useful for administrators?**

"Insights into user engagement, most searched careers, and which programs are most effective."

### **2.6.2 Core Functionalities**

#### **User Accounts and Authentication**

- Allow users to register, log in, and manage personal profiles securely.
- Store user background information including education, experience, career interests, and preferences.
- Enable users to update profiles and save progress across sessions.

#### **Career Profile and Pathway Recommendations**

- Generate personalized career pathways based on user background and goals.
- Recommend certifications, training programs, and volunteer opportunities aligned with user profiles.
- Highlight steps required to transition into Canadian job markets.

#### **Opportunity Discovery**

- Display job postings, career events, networking sessions, and volunteering opportunities.
- Filter opportunities by industry, location, experience level, and diversity preferences.
- Provide detailed descriptions including eligibility, requirements, and application steps.

#### **Application Management**

- Allow users to apply to opportunities through a unified application portal.
- Track application status and previously applied opportunities.
- Save documents and profile data to reduce repetitive applications.

#### **Community and Networking Support**

- Recommend community organizations, mentorship programs, and networking events.
- Highlight events related to user's background or career interests.
- Allow users to bookmark and revisit events.

#### **User Dashboard**

- Provide a personalized dashboard summarizing saved opportunities, applications, and recommendations.
- Display progress indicators for completed training or certifications.
- Show upcoming events and suggested next steps.

#### **Notifications and Alerts**

- Notify users about new opportunities, events, or updates relevant to their profile.
- Allow users to customize notification preferences (email or in-app).
- Send reminders for upcoming events or incomplete applications.

#### **Administrative Functions**

- Provide an admin panel for managing users, content, and opportunities.
- Monitor system usage, engagement levels, and popular career paths.
- Manage and approve job postings, events, and training listings.

# 2.7 Nonfunctional Requirements

### Usability (API, UI)

- The platform will have a minimalist layout to simplify navigation and reduce cognitive load for newcomers.
- Fewer steps and buttons are required to access recommendations, events, training programs, and profile settings.
- Intuitive workflows ensure users can quickly find relevant opportunities without unnecessary clicks.
- The system will aim to minimize bugs and crashes, providing a smooth and reliable user experience.

### Privacy

- Only necessary personal information will be stored, including name, email, career background, and profile preferences.
- No third-party sharing of personal information will occur without explicit user consent.
- Users will have access to full functional requirements and transparency about what data is collected and how it is used.
- Personal data will only be used to enhance recommendations and experience, never for marketing purposes without consent.

### Security

- Only essential information will be requested; sensitive data such as government IDs or financial details will not be stored.
- All data transfers will be encrypted using HTTPS to ensure secure communication between clients and servers.
- User accounts will be protected with two-factor authentication (2FA) to prevent unauthorized access.
- Regular security audits and code reviews will be performed to maintain robust security standards.

### Performance

- Pages and recommendation dashboards will load efficiently, providing a smooth experience for users.
- API calls for fetching events, training, and career resources will be optimized to return results within a few seconds.
- The system must support up to 10,000 concurrent users without noticeable slowdowns.
- URLs, page structures, and content will be optimized for SEO-friendly indexing, improving discoverability of public resources.

### Maintainability

- The codebase will follow modular and layered design principles to support future feature expansions.
- Documentation and coding standards will be maintained to ensure ease of onboarding new developers.
- APIs, backend services, and frontend components will be loosely coupled, allowing updates or changes without affecting the entire system.
- Continuous integration and automated testing will ensure stable, maintainable releases.
