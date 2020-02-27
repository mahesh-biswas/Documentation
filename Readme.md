# E-Cowork

## Modules

### Layout Designer
#### Description:
> • This module is helpful in creating the floor plan of the co-working space.
> • This plan then will be used for visualization of space in the booking console.

#### Component List:
	[+] Class
		- LayoutDesignerController.cls
		- LayoutController.cls
		- LayoutControllerHandler.cls
		- LayoutControllerHelper.cls
		- Constants.cls
		- Utility.cls
		- UtilityWithoutSharing.cls
		- Wrapper.cls
	[+] Visualforce Components
		+ Pages
			- LayoutPage.page
		+ Component
			- LayoutDesigner.component 
[click to view the relationship diagram](https://eternussolutionscom-my.sharepoint.com/:i:/g/personal/mahesh_biswas_eternussolutions_com/EWNedCfbi1dFvzvAGDTX9yEB8FdHXe2sken4I7T9HbOHLw?e=D815Qm)

### Booking Console
#### Description:
> • This module is used to visualize the co-working space, i.e show the status of any space. for example: if some x space is bookable, if yes then is it occupied within the selected duration.
> • The user can select any space and if wanted then can add facilities to that space.
> • Once finalised then they can see their order summary before final conformation.
> • Once confirmed, the space will be booked for them and the space is marked un-available for others to book.
#### Component List:
	[+] Class
		- LayoutController.cls
		- BookingController.cls
		- BookingControllerHandler.cls
		- Constants.cls
		- Utility.cls
		- UtilityWithoutSharing.cls
		- Wrapper.cls
	[+] Visualforce Components
		[+] Pages
			- BookingPage.page
		[+] Component
			- BookingConsole.component
[click to view the relationship diagram](https://eternussolutionscom-my.sharepoint.com/:i:/g/personal/mahesh_biswas_eternussolutions_com/EdNysA2nLVJBluk9LLrxa9YBVGTmEBLs5nAQxVO49HJ-kA?e=gOgiNL)

### Lead Scoring
#### Description:
> • This module is helpful for the sales person to prioritise the leads.
> • User can configure the **lead scoring rule** as per their requirement.
> • A rule can have multiple fulfilling conditions to succeed reward score point to  the lead.

#### Component List:
	[+] Trigger
		- Criteriatrigger.trigger
		- LeadTrigger.trigger
		- RuleTrigger.trigger
	[+] Class
		- LeadTriggerHandler.cls
		- LeadScoreCalculation.cls
		- RuleTriggerHandler.cls
		- CriteriaTriggerHandler.cls
		- ExpressionEvaluationUtility.cls
		- ValidateLeadFieldName.cls
		- Constants.cls
		- Utility.cls
		- Wrapper.cls
[click to view the relationship diagram](https://eternussolutionscom-my.sharepoint.com/:i:/g/personal/mahesh_biswas_eternussolutions_com/EVLUne1tw0tMiRsdMw33z1gB_fKrObCVmOa897u-fqjBdQ?e=HWyP2c)

### Discounting Rule
#### Description:
> • This module is similar to the **Lead Scoring** module with reference to rule configuration.
> • This module is helpful for the sales person to give discount to any product.
> • User can configure the **discounting rule and condition** as per their requirement.
> • User can give different discount to some product based on the quantity range. i.e for quantity between 10-20 discount of maximum 5% is valid and when quantity is between 20-30 maximum discount allowed can be 10%.
> • This module's requirement is **Quote**. The discounting can be given to **quoteLineItem**.

#### Component List:
	[+] Trigger
		- DiscountConditionTrigger.trigger
		- DiscountTierTrigger.trigger
		- QuoteLineItemTrigger.trigger
	[+] Class
		- DiscountConditionTriggerHandler.cls
		- DiscountTierTriggerHandler.cls
		- DiscountCalculationUtility.cls
		- LeadScoreCalculation.cls
		- ExpressionEvaluationUtility.cls
		- ValidateLeadFieldName.cls
		- Constants.cls
		- Utility.cls
		- Wrapper.cls
[click to view the relationship diagram](https://eternussolutionscom-my.sharepoint.com/:i:/g/personal/mahesh_biswas_eternussolutions_com/EXT_XoCNwKlEoilF4U0OAOkBm04dzwRwdaub-M32k_Jhuw?e=bEWoi1)
