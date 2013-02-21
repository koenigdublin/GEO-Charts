GEO-Charts
==========


C# ncloc 27414
js ncloc 13521

70 controls
duplication 2.2%


Status with Applications not using the UI Core Framework (Pre UI FW):
  Each Developer writes own pages, layouts, controls, etc.
  Each Screen has lots of duplicate code (within the page, and across pages).
	High Development, Testing and Maintenance Cost due to the lack of consistency of implementation.
	High Cost on rework for DDA, Style guide (Phoenix), cross browser support.
	Huge and inconsistent HTML and Java script Code affecting performance. 
	Performance tuning needs to be replicated across every page of the application.


Exists (as of CD BE 1.3a)
	Model-View-Controller (MVC3), Metadata configs for generating views.
	*Consistent and performing controls and layouts for all supported browsers (application team doesn’t need to code HTML/CSS).
	Public API’s for ASP.NET and JavaScript UIFW features, with IntelliSense auto completion to aid developers.
	Common features, e.g. Print (UIFW service exists). 
	Portal integration for checking authentication,  preferences,  and entitlements.
	Client and server side validation (API exists) and logging.
	Client and server side Unit Tests (with high coverage).
	Localisation API, facilitates early detections of missing strings.
	Security built in - XSS prevention (client, server), XSRF prevention (prevents cloning of pages), and VA compliance.
	Iterative process, “Definition of Done” in place – all tasks 100% completed before a User Story is set to Completed.
	Automated continuous builds and deployments, with automated functional and regression tests (per build).
	Reference Implementation/Demo for the UIFW features, with Performance  testing capabilities.
	Training video’s, wiki page, discussion board.

In Progress
	White Label / Service Provider support for – labels, controls, layouts, UX branding, look and feel, integration.
	Mobile controls and layouts (PoC completed).
	*Charting capabilities (PoC completed, Scalable Vector Graphics (SVG)-based charting  being looked at next to allow for development of custom charts).
	Tablet support (generation of Native Hybrid Apps based on HTML5 base) – initial analysis in progress.
	Accessibility support for controls and layouts.
	Hello World package to allow application developers to get up to speed quickly (goal is within a few hours).
	Product Backlog, Governance.

To be prioritised
	Database-driven Metadata configs (currently compile time configs).
	Link UI Core Framework wiki with Global UX Practice website.
	Branding, look and feel changes that may result from consolidation across the three channels by the Global UX Practice (if so, will need updated UX implementation in UIFW).
	Approval of UIFW Vision and Charter.

UI FW scope:
	Provide reusable components for application teams
	Ensure HTML, styles and cross-browser compatibility
	Introduce configurability of UI including dependency injection
	Ensure high application performance
	Improve code manageability
	Provide guidance for application development process

Model Metadata
	UI configuration implemented by Model, Model Metadata and View
	Model Metadata and View are configured using “fluent” approach
	Fluent approach based on C# code so it can be unit tested
	Model metadata configuration is based on standard API of ASP.NET MVC


----------
TABLET
----------

The current platform of CitiDirect (CitiDirect, CitiDirect BE Portal, CitiDirect BE Mobile) is very strong in handling complex Treasury needs using a flexible entitlement engine to perform transactions, generate reports and other day-to-day activities of the cash management. It is a truly global consolidated system that is handling various different business rules to meet the demands of multi-billion corporations down to the local SME. In doing so, the system has focused on the core needs to add and enhance very rich features and functionalities of all products including payment, receivable, liquidity & investment, trade and even SFS. 
While the system is very strong and powerful, an opportunity exists to simplify the interface for senior level authorizers who are looking for a convenient and fast way to perform specific tasks such as authorizing single and multi-payments and file & batch approvals.
The core CitiDirect BE Tablet audience is for these senior managers of institutional clients. There are many examples and public data confirming the growing usage of Tablet (specifically iPad) and it’s not just a trend in developed countries but even in emerging countries as well. We see the growing number of professionals carry Tablet device either for business or personal usage and their daily consumption of contents and activity on tablet is increasing. So having a dedicated solution on this unique device with a bigger panel than mobile device is a logical choice for CTS to take next step and developing new solution that will bridge the gap. Knowing their needs is important so that we build the right solution. We can summarize the core need to be holistic Cash Management or Working Capital Management. Across products, across currencies, across regions and countries, these organizations operate their business in cash and that’s where the core need exists. 
While the core target market is senior managers, we recognize that the tablet device growth and usage will extend and penetrate over time to other levels of management and client users.  The initial application and structure should allow for extensibility to other market segments.



-----


The current platform of CitiDirect (CitiDirect, CitiDirect BE Portal, CitiDirect BE Mobile) is very strong in handling complex Treasury needs using a flexible entitlement engine to perform transactions, generate reports and other day-to-day activities of the cash management. It is a truly global consolidated system that is handling various different business rules to meet the demands of multi-billion corporations down to the local SME. In doing so, the system has focused on the core needs to add and enhance very rich features and functionalities of all products including payment, receivable, liquidity & investment, trade and even SFS. While the system is very strong and powerful, an opportunity exists to simplify the interface for senior level authorizers who are looking for a convenient and fast way to perform specific tasks such as authorizing single and multi-payments and file & batch approvals.

CitiDirect BE Mobile is a channel solution to focus on the specific needs of authorizers. Instead of replicating CitiDirect, it optimizes the experience by simpler navigation, intuitive UI, speedy page loading, and some new and unique features in mobile like Filtering. This process innovation and user-experience allowed the authorizers to be remote and has paid off. By focusing on this particular authorizer user segment and their specific needs, we have learned several things about the solution of mobile and tendency of our users. 


1.	When the solution is convenient even with a security concern of mobile, there are a group of users who quickly adapt and drive the volume. 

2.	When the solution is simple, intuitive yet consistent with CitiDirect presenting existing data and functionalities to a new device, a user takes minimum effort to learn even in a new look & feel.

3.	When the solution is focused in 20% of the top features and functionalities, you can maximize the benefits from the rapid commercialization.


Despite the success of our various electronic platforms the user base is primarily at the level of the Assistant Treasurer and below. While our relationship managers interface with the CFO/T/AT’s, their digital experience with Citi is minimal. These senior officers of the institutions have several common behaviours.

1.	They make treasury related financial decisions.
2.	They do not access CitiDirect normally. 
3.	They are focused on understanding the larger financial picture
4.	They are looking for opportunities to improve efficiency of working capital management
5.	They direct the treasury team to perform daily and ad-hoc analysis.
6.	If they are authorizers, they are more concerned with the balance of the accounts and liquidity position than other treasury professionals.
7.	They lead the treasury staff meetings
8.	They need to periodically report the current financial situation of the firm
9.	They are frequently out of their office either in meetings or travelling

They key observation is #2 where these seniors do not access CitiDirect. Many of them still do not use CitiDirect BE Mobile because it is focused on payment authorization. These platforms don’t have the features that are needed by these seniors including reporting, risk management, work flow view etc. Therefore, between CitiDirect and CitiDirect BE Mobile, we do not have an electronic relationship with these types of users. Not having any digital interface with these professionals is a gap that we must overcome with new solution in the new device, tablet.

The core CitiDirect BE Tablet audience is for these senior managers of institutional clients. There are many examples and public data confirming the growing usage of Tablet (specifically iPad) and it’s not just a trend in developed countries but even in emerging countries as well. We see the growing number of professionals carry Tablet device either for business or personal usage and their daily consumption of contents and activity on tablet is increasing. So having a dedicated solution on this unique device with a bigger panel than mobile device is a logical choice for CTS to take next step and developing new solution that will bridge the gap. Knowing their needs is important so that we build the right solution. We can summarize the core need to be holistic Cash Management or Working Capital Management. Across products, across currencies, across regions and countries, these organizations operate their business in cash and that’s where the core need exists. 

While the core target market is senior managers, we recognize that the tablet device growth and usage will extend and penetrate over time to other levels of management and client users.  The initial application and structure should allow for extensibility to other market segments.

 
