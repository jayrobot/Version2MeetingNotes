# HFNY version 2.0 - Design

## Carry-overs
 - "Lock down" version 1.0
 - Git branching and dual master tracks
 - Best Practice Standards
 - Stored procedure streamlining esp. Case Home Page
 - Duplicate removal
 - Review and cleanup
 
## High Importance
- Genericizing
	- Extensibility model 
		- defining what can be extended
		- detailing extension points
	- Data driven where applicable
- Worker associated with logins
- New Landing Pages / Dashboards
	- User / Data Entry
		- Ticklers
		- Recent Searches
		- Most active cases
	- Supervisor
		- Ticklers
		- Outstanding Approvals 
		- Sparklines / Graphs 
	- Program Manager
		- Sparklines / Graphs 
			- Case Load
			- Total Served, Screened, and Visited
			- Capacity
			- Contract Dates
		- Worker List
			- View Dashboard
			- Case Load 
- Mobile - Search cases/addresses. HV Log? 
- Compatibility with Firefox, Chrome, others (see Zoho)

## New / improved features
- Consistent use and look for forms using dataTables (Users / Workers / Maintenance Forms / +++)
- Self service for users 
	- better password reset
	- inform when locked out
- Dirty state - implement detection / handling for forms
- Report Catalog 
	- lazy loading 
	- collapsible sections with tooltips 
	- validation
- New reports 
	- Family Characteristics 
	- PI report 
	- Basic form printouts
	- other
- User interaction 
	- make it easier to spot currently focused control
	- improve tabbing (First to Last back tab)
	- shortcuts and keyboard conveniences
	- Validation - Move to first field with failed validation
- Add alternate mailing address
- Add additional cell phone numbers
- Phone number / address audit history
- Other enhancement requests (see Zoho)
- More appealing layout and graphics (Need better logos for apps and us)

## Other
- Take care of prenatal and postnatal issues when tc dob is entered incorrectly
- Allow changing PC1ID manually, and automate it on name or DOB changes
- Don’t allow cases to be transferred if there are completed discharge intervals of forms in the cases. Options are:
	- make the original site delete discharge forms so the new site can enter new data with no issue 
	- delete (or archive or something) automatically
- Better worker change editor
- Better level editor (clear close button, grid editing, more precise and flexible validations, esp. for transfer cases)
- Levels for transfer cases if baby was born before Case Acceptance date and not entered by previous site. HVLevel form needs to allow users to delete a level entered AFTER the TCID DOB. (HW962)
- Fatherhood advocate and father figure info on Basic Information (HW207)
- From Cheri Elefante 
	- FSW Case List - add FOB or FF's name - promote father involvement.
	- Family Timeline:  Place a check mark next to assessments (PSI, ASQs) that were completed and entered in the system.
- FAQs/Missives/News - searchability, better organization and out of the way of the new landing pages

## Code issues
- Code cleanup - reformat and address consistency of techniques and methodologies
- Code reorganization - split JS / CSS into separate files
- Dependencies 
	- NuGet 
	- npm 
- Build process 
	- gulp 
	- grunt 
	- minifying
- Updates
	- jQuery and plugins 
	- DevExpress 
	- ASP
- JS Framework / Components
	- angular 
	- ember 
	- react 
	- polymer 
	- vue
- Interface
	- bootstrap 
	- humane.js (or humanemsg.jquery.js) notifications
	- Data Layer / ORM: 
		- Entity Framework 
		- data objects 
		- services
	- JS Data
		- Knockout 
		- Backbone 
		- Upshot 
		- KnockBack
- HTML / CSS
	- html5boilerplate 
	- yeoman generators 
	- caniuse 
	- best practices 
- .net framework 5
- release versioning

## Testing
 - Unit
 - Integration
 - Regression
 - Functional
 - Performance
 - Accessibility
 - Usability
 - Acceptance 
 - End-To-End (Running all types of tests) 
 - Continuous Integration (Running tests automatically on save/build/publish)
 - Tools
	 - MS Test
	 - Red Gate SQL Test
	 - xUnit
	 - qUnit
	 - JsUnit
	 - Browserify
	 - WatiN
	 - Mocha
	 - Jasmine
 
## Code notes:
- Home Page - Outstanding Approvals?
- Modal Dialogs

		Do While !having.fun()
			Imbibe()
			Thrash()
			Sleep()
		End While
