# Errors

Emploai uses conventional HTTP response codes to indicate the success or failure of an API request. In general: Codes in the <code>2xx</code> range indicate success. Codes in the <code>4xx</code> range indicate an error that failed given the information provided (e.g., a required parameter was omitted, a charge failed, etc.). Codes in the <code>5xx</code> range indicate an error with Emploai's servers (these are rare).

Some <code>4xx</code> errors that could be handled programmatically (e.g., a user is deleted ) include an error code that briefly explains the error reported.


Error Code | Meaning
---------- | -------
200 | Everything worked as expected.
400 | Bad Request -- The request was unacceptable, often due to missing a required parameter.
401 | Unauthorized -- No valid API key provided.
402 | Request Failed -- The parameters were valid but the request failed.
404 | Not Found -- The requested resource doesn't exist.
409 | Not Acceptable -- The request conflicts with another request (perhaps due to using the same idempotent key).
429 | Too Many Requests -- Too many requests hit the API too quickly. We recommend an exponential backoff of your requests.
500 | Internal Server Error -- We had a problem with our server. Try again later.
503 | Service Unavailable -- We're temporarily offline for maintenance. Please try again later.
