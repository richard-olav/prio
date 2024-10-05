# A plan for how to implement web-native publications on PRIO.org

Below is a plan on how to implement web-native publications on PRIO.org. This plan tries to follow a clear design methodology, ensuring that both the user experience and technical implementation are thoroughly considered and optimized. 

Keep in mind that the technologies mentioned are only meant as suggestions to illustrate the technology stack. The choice of technology can be limited by already existing technology and in the initial phase the needs can change. 

I would like to clarify that in the specific task I think it is important to present sketches, mockups or prototypes as soon as possible to ensure that technical and non-technical stakeholders have roughly the same perception of what is to be produced/developed. 

---

## High-Level Summary: Web-Native Publications on PRIO.org

#### Purpose
The goal of transitioning PRIO’s research publications from PDF format to web-native format is to enhance accessibility, usability, and audience reach. Web-native publications offer a more dynamic and responsive experience, making it easier for users to interact with multimedia elements like images, graphs, and maps.

#### Scope
The project involves several key steps:
1. **Define**: Understand the needs and goals of transitioning to web-native publications.
2. **Research**: Gather insights from internal and external users to identify pain points and opportunities.
3. **Analysis & Planning**: Develop user personas, user stories, wireframes, and choose the appropriate technology stack.
4. **Design**: Focus on user experience (UX) and user interface (UI) design to ensure a seamless and accessible experience.
5. **Prototyping**: Create interactive prototypes to demonstrate key user flows and gather feedback.
6. **Testing**: Conduct usability testing to refine the design based on user feedback.
7. **Launch**: Develop the final application, perform final tests, and launch the web-native publications.
8. **Iteration**: Continuously monitor and improve the design based on real-world user interaction and feedback.

#### Impact
- **Increased Visibility**: Web-native publications are easier to discover and access, increasing the visibility of PRIO’s research.
- **Improved User Experience**: Users will find it easier to navigate and interact with publications, especially on mobile devices.
- **Enhanced Engagement**: Interactive elements like graphs and maps will make the content more engaging and informative.
- **Accessibility**: Compliance with web accessibility guidelines ensures that all users, including those with disabilities, can access the content.
- **Resource for Media**: The ability to link datasets and interactive plots within articles will be valuable for media professionals looking to recreate visuals for news articles.

By transitioning to web-native publications, PRIO aims to provide a more engaging and accessible platform for its research, benefiting researchers, policy-makers, and the general public.

---

## A more detailed "technical" section

### **Step 1: Define**
**Goal:**  
Transitioning/complementing the already existing PRIO’s PDF research publications archive and archive the publications into web-native format (using HTML, CSS and JavaScript) to enhance accessibility, usability, and audience reach.
**Why:**  
PDFs can be difficult to navigate, especially on mobile devices. PDFs also limit engagement and interactivity. Web-native publications will provide a more dynamic, responsive experience, improving interaction with multimedia elements like images, graphs, diagrams, plots and maps.  
**Who:**  
Primary users include researchers, policy-makers, and general audiences who need easy access to PRIO's research.

**How**
Internal stakeholder meeting or as a first step of a Design Sprint (https://designsprintkit.withgoogle.com/methodology/overview)

**Business Problems Solved:**  
- Increase visibility and discoverability of research.
- Improve user experience and engagement with PRIO’s content.
- Make sure PRIO will continue to stand out as a leading Peace Research Institute make it a go to resource for undertanding complex subjects

**Outcome of Stakeholder Meetings:**  
Set of requirements and a low-fi concept or sketches detailing content flow and layout considerations for the web.

---

### **Step 2: Research**
**Research Focus:**
- **Internal Users:** PRIO researchers, communication staff.
- **External Users:** Government bodies, academics, general public.
- **Methods:**  
  - **Customer Journey Mapping:** Map how users currently access and use PRIO’s PDFs to identify pain points.  
  - **Competitor Analysis:** Review how similar institutions handle web-native research publications.  
  - **Usability Testing:** Conduct tests to understand how users interact with PDF vs. web-native publications.
  
This could be conducted either as a part of a Design Sprint or as an internal process between various actors at PRIO.

---

### **Step 3: Analysis & Planning**
**Key Deliverables:**
- **User Personas:** Profile typical users (e.g., researchers, policy makers) to focus design decisions on their needs.
- **User Stories:** Define how different users will engage with the site (e.g., "As a researcher, I want to quickly find relevant publications", "When I find a publication I want a quick summary to understand if the publication is relevant for my needs").
- **Wireframes:** Create high-level wireframes to visualize the layout and content flow. 
- **Technology Stack:** Consider technologies (e.g. D3.js, Leaflet for graphs, Python Flask, Vue.js etc.) to implement web-native publications. Consider using Scrollama.js, d3.js and html/css for storytelling components or summaries for articles. Leaflet or mapbox for interactive maps. Python could be considered in cases where there is a need for some back-end processing before serving interactive content to the front-end. For this task I would also consider creating interactive examples and libraries for plotting using e.g. Jupyter Notebooks which can be used by researchers at an early stage when they create a publication, for the purpose of creating interactive plot maps etc. that follows the design guidelines. This will make it easier to transfer the content from articles to the web when publishing articles in the web-native format.
  
**Roadmap & Milestones:**
The project should contain a clear roadmap or milestones. Below is a fictional roadmap, and this will depend on the scope of the project and if it is a longer internal project/process between various actors at PRIO or a design sprint.
- Prototype ready by month 2.
- Usability tests by month 3.
- Final launch by month 5.

---

### **Step 4: Design**
**Focus on User Experience (UX):**  
- **Information Architecture:** The organization of the publication archive seems to have a good structure linking topics, projcets and relevant news, but beyond the current organization having web-native publications will enable the possibility to link other relevant articles witin the article itself but also datasets used in a publication (e.g. via https://github.com/prio-data) or databases, apis etc. This will also be usefull resources for the media, wanting to recreate some of the interactive plots for news articles etc.
- **Navigation:** Simple navigation to access full publications, figures, and multimedia elements.
- **Layout:** Responsive design for mobile, tablet, and desktop.
  
**UI Design Considerations:**  
- **Accessibility:** Ensure compliance with WCAG (Web Content Accessibility Guidelines).  
- **Microcopy:** Clear, concise labeling for buttons, links, and tooltips.
- **Visuals:** Use clean, modern color schemes and typography to enhance readability.

This could be conducted either as a part of a Design Sprint or as an internal process between various actors at PRIO.

---

### **Step 5: Prototyping**
**Prototyping Tools:**  
- Use tools like Figma to create interactive, clickable prototypes.  
- **Prototype Components:**  
  - Interactive graphs and maps.
  - E.g. interactive map, placing the articles to the various geographical ares they are related to
  - Fully responsive layouts for each publication type (policy briefs, research papers).
  
**Goals:**  
- Demonstrate key user flows.
- Enable usability testing with realistic interactions.

This could be conducted either as a part of a Design Sprint or as an internal process between various actors at PRIO.

---

### **Step 6: Testing**
**Usability Testing:**  
- Gather feedback from real users (both internal and external) on the prototype.
- Focus on ease of navigation, clarity of content, and interaction with multimedia elements.
  
**Revisions:**  
- Identify areas of friction in the user flow (e.g., complex navigation or unclear visuals).
- Implement changes to refine the design before final development.

This could be conducted either as a part of a Design Sprint or as an internal process between various actors at PRIO.

---

### **Step 7: Launch**
**Development of prototype to fully functional application:**  
- Use the prototype and feedback from user-testing, complete the application with detailed style guides and interaction specification.
- Make sure we have a plan for how the workflow will be for publication of articles to the new platform.
  
**Go-Live:**  
- Perform final tests on staging environments to ensure smooth functionality across devices.
- Launch the web-native publications and announce via PRIO’s channels.
- Follow up an monitor using SEO (e.g. Google Analytics or Matomo)

Usually this will take form as a real application, with full or nearly full functionality. I perfer launching new features and applications as beta version or as a closed version for limited users in order to make sure the application is working on a larger scale.

---

### **Step 8: Iteration**
**Post-Launch:**  
- Monitor user engagement via SEO analytics and user feedback.
- Consider implementing A/B testing to identify optimal design changes.
- Continue to iterate on design, improving usability based on real-world user interaction.

**Long-Term Goal:**
Constantly refine the design and internal library for plotting, maps and interactive components to ensure a seamless, enjoyable user experience and sustained visibility of PRIO’s research content.

In the last phase I would iterate and gather feedback as well as launch a plan for operation, maintanance and further improvement.

I would also make sure that there is a dedicated product owner/stakeholder both at the technical level but also on the user side (researcher, department head etc.) to make sure the application is maintained.
