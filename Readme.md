# Setup instructions

1-Import the solution

2-Flow:

    a.For the connections it should be under a service
	account.

    b.The service account needs access to the tables
	in the data verse, AI Builder Model

    c.In the flow - > Trigger condition replace`<service-account-guid>`
	with the service accounts guid

Example of trigger condition:

`@not(equals(triggerOutputs()?['body/_modifiedby_value'], '269592a8-5ef6-ef11-9341-7c1e52168ba1'))`
