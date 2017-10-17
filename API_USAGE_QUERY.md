We have added a new usage call to our real-time API.

If you call the API with usage = 1 then you get today’s usage and this month’s usage e.g.
 
https://api.emailverifyapi.com/api/a/v1?key=XYZ123&usage=1
 
{
    "apiKey" : "XYZ123",
    "dailyQuota" : "100000",
    "date" : "2017-10-17",
    "dateUsage" : 8353,
    "month" : "2017-10",
    "monthUsage" : 269558
}
 
But with a date from a previous month added to the query then the month stats are for that month e.g.
 
https://api.emailverifyapi.com/api/a/v1?key=XYZ123&usage=1&date=2017-09-14
 
{
    "apiKey" : "XYZ123",
    "dailyQuota" : "100000",
    "date" : "2017-09-14",
    "dateUsage" : 11458,
    "month" : "2017-09",
    "monthUsage" : 467181
}
