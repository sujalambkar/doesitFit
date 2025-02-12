# DoesitFit
Integrateable tool to check feasibility of clothing size. 

1. Overview

Use Case Name: Apparel Size Feasibility Checker
Description: A tool that assesses whether a selected apparel size is feasible for an individual based on body measurements, size charts, and fit preferences.
Primary Actor: End Users (Customers, Retailers, Fashion Brands)
Secondary Actors: E-commerce Platforms, AI/ML Algorithms, Customer Support Teams

2. Objectives

    Reduce size-related returns and exchanges in online and offline apparel shopping.
    Provide accurate size recommendations based on individual body measurements.
    Improve customer satisfaction and brand trust through precise sizing guidance.
    Optimize inventory management by predicting popular sizes accurately.

3. Stakeholders
Stakeholder	Role	Interest
Customers	End-users using the tool to check size feasibility	Wants accurate size recommendations to avoid wrong purchases
Retailers & Brands	Sellers integrating the tool into their platforms	Reduce return rates and enhance customer experience
E-commerce Platforms	Online stores integrating the tool	Optimize order fulfillment and reduce logistics costs
Developers	Tech team implementing the tool	Ensuring accurate calculations and seamless user experience
4. Preconditions

    The user provides body measurements manually or via body scanning (camera-based).
    The tool has access to brand-specific size charts.
    The user selects a specific apparel type (shirt, jeans, dress, etc.).

5. Postconditions

    The system provides a size feasibility result:
        ✅ Perfect Fit
        ⚠️ Possible Fit with Adjustments
        ❌ Not Recommended
    Suggestions for alternative sizes or tailored options.

6. Main Flow (Happy Path)
Step	Description
1	User selects apparel type (e.g., T-shirt, jeans, dress).
2	User inputs body measurements manually or via scanning.
3	System retrieves relevant brand-specific size charts.
4	System compares user data with size chart metrics.
5	System displays feasibility results (Perfect Fit / Possible Fit / Not Recommended).
6	If size is not feasible, system suggests alternatives.
7	User confirms selection or modifies choices.
7. Alternate Flows
Scenario	Alternate Flow
User does not know exact measurements	Tool provides a guided self-measurement process.
Apparel brand is missing from the database	System estimates size based on standard sizing data.
User gets a “Not Recommended” result	Suggests closest fit or custom-tailoring options.
8. Error Handling
Error	Handling Mechanism
Incomplete measurements	Prompt user to provide missing details.
System unable to match size	Offer generic size recommendations based on best fit.
Measurement errors	Allow user to re-enter or adjust measurements.
9. Assumptions & Constraints

    Accuracy depends on correct input of user body measurements.
    Different brands may have inconsistent sizing charts.
    AI-based scanning (if used) should have high precision to ensure reliable recommendations.

10. Functional Requirements
Requirement ID	Description	Priority
FR-01	Allow users to input body measurements manually.	High
FR-02	Integrate AI-based body scanning (optional).	Medium
FR-03	Retrieve and store brand-specific size charts.	High
FR-04	Compare user measurements with size charts.	High
FR-05	Display feasibility results with recommendations.	High
11. Non-Functional Requirements
Requirement ID	Description	Priority
NFR-01	Response time should be under 3 seconds.	High
NFR-02	Should support mobile and desktop platforms.	High
NFR-03	Secure storage of user measurement data.	High
NFR-04	Scalable to accommodate different brands & apparel types.	Medium
12. Potential Enhancements (Future Scope)

    Integration with AR/VR for virtual try-ons
    AI-based predictive sizing based on past purchases
    Custom-tailored size recommendations for niche apparel

Conclusion

This Apparel Size Feasibility Checker enhances the shopping experience by reducing size-related issues and improving fit accuracy. It benefits both customers and retailers by lowering return rates, optimizing inventory, and boosting confidence in online and offline apparel purchases. 🚀
