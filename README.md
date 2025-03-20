# fed-layoffs
Tracking the layoffs of federal employees since 2025-01-20

This was supposed to be an exercise in scraping information from court documents, but that didn't work out so instead I've assembled a hand-curated CSV of federal employees who were terminated and reinstated subsequent to a court-ordered temporary restraining order. Currently includes counts of probationary employees only. 

## Context
On January 20, 2025, many executive branch agencies received a guidance memorandum from the Office of Personnel Management (OPM) which stated that “agencies should identify all employees on probationary periods” and “should promptly determine whether those employees should be retained at the agency.” This is a count, by agency, of the number of such employees terminated. 

A temporary restraining order (TRO) was issued on March 13, 2025, requiring the agencies to reinstate all Affected Probationary Employees, as defined in paragraph 10(c) of the TRO, who were terminated on or after January 20, 2025. 

## Data
- agency: U.S. government agency
- action_date (in yyyy-mm-dd format): the date an action was taken. When dates are expressed as a range (e.g., "between February 13, 2025, and February 24, 2025" the end date is used. 
- action: e.g., terminated, rehired, reinstated
- status: whether the reinstated employees are on administrative leave or fully reinstated
- employees: number of employees affected by the action
- employee_type: whether employees were probationary, career, etc. 
- case_number: court case number
- case_date: the date the court document was filed
- court: which court the document was filed in
- district: the court district the document was filed in
- notes: a text field describing anything unusual about the information provided
- source: a link to a source URL
