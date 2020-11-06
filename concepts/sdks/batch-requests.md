---
title: 使用 Microsoft Graph Sdk 进行批处理请求
description: 提供有关使用 Microsoft Graph Sdk 创建一批 API 请求的说明。
localization_priority: Normal
author: DarrelMiller
ms.openlocfilehash: 721adb1631037055a2d2498d321bb06e68b6c257
ms.sourcegitcommit: 22d99624036ceaeb1b612538d5196faaa743881f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/06/2020
ms.locfileid: "48932421"
---
# <a name="use-the-microsoft-graph-sdks-to-batch-requests"></a>使用 Microsoft Graph Sdk 进行批处理请求

[批处理](../json-batching.md) 是将多个请求合并为一个 HTTP 请求的一种方法。 请求将组合到单个 JSON 有效负载中，该负载通过 POST 发送到 `\$batch` 终结点。 Microsoft Graph Sdk 具有一组类，可简化批处理负载的创建和分析批处理响应负载的方式。

> [!IMPORTANT]
> 有关 Microsoft Graph 中 JSON 批处理的当前限制，请参阅 [已知问题](../known-issues.md#json-batching)。

## <a name="create-a-batch-request"></a>创建批处理请求

Microsoft Graph Sdk 提供了三个类来处理批处理请求和响应。

- **BatchRequestStep** -表示单个请求 (例如 `GET /me` 批次中) 。 它允许为请求分配一个唯一的标识符，并指定请求之间的依赖关系。
- **BatchRequestContent** -简化了批处理请求负载的创建。 它包含多个 **BatchRequestStep** 对象。
- **BatchResponseContent** -简化了对来自批处理请求的响应的分析。 它提供了获取所有响应、按 ID 获取特定响应以及获取属性（如果存在）的功能 `@odata.nextLink` 。

## <a name="simple-batching-example"></a>简单的批处理示例

此示例演示如何在不相互依赖的批处理中发送多个请求。 这些请求可以按任何顺序由服务运行。 此示例获取用户并获取当前日期的用户日历视图。

### <a name="c"></a>[C#](#tab/csharp)

```csharp
// Use the request builder to generate a regular
// request to /me
var userRequest = graphClient.Me.Request();

var today = DateTime.Now.Date;
var start = today.ToString("yyyy-MM-ddTHH:mm:ssK");
var end = today.AddDays(1).ToString("yyyy-MM-ddTHH:mm:ssK");

var queryOptions = new List<QueryOption>
{
    new QueryOption("startDateTime", start),
    new QueryOption("endDateTime", end)
};

// Use the request builder to generate a regular
// request to /me/calendarview?startDateTime="start"&endDateTime="end"
var eventsRequest = graphClient.Me.CalendarView.Request(queryOptions);

// Build the batch
var batchRequestContent = new BatchRequestContent();

// Using AddBatchRequestStep adds each request as a step
// with no specified order of execution
var userRequestId = batchRequestContent.AddBatchRequestStep(userRequest);
var eventsRequestId = batchRequestContent.AddBatchRequestStep(eventsRequest);

var returnedResponse = await graphClient.Batch.Request().PostAsync(batchRequestContent);

// De-serialize response based on known return type
try
{
    var user = await returnedResponse
        .GetResponseByIdAsync<User>(userRequestId);
    Console.WriteLine($"Hello {user.DisplayName}!");
}
catch (ServiceException ex)
{
    Console.WriteLine($"Get user failed: {ex.Error.Message}");
}

// For collections, must use the *CollectionResponse class to deserialize
// The .Value property will contain the *CollectionPage type that the Graph client
// returns from GetAsync().
try
{
    var events = await returnedResponse
        .GetResponseByIdAsync<UserCalendarViewCollectionResponse>(eventsRequestId);
    Console.WriteLine($"You have {events.Value.CurrentPage.Count} events on your calendar today.");
}
catch (ServiceException ex)
{
    Console.WriteLine($"Get calendar view failed: {ex.Error.Message}");
}
```

### <a name="typescript"></a>[TypeScript](#tab/typescript)

```typescript
// Create a batch request step to GET /me
let userRequestStep: MicrosoftGraph.BatchRequestStep = {
  id: "1",
  request: new Request("/me", {
    method: "GET"
  })
}

let today = moment({hour: 0, minute: 0, seconds: 0});
let start = today.format();
let end = today.add(1, "day").format();

// Create a batch request step to GET
// /me/calendarview?startDateTime="start"&endDateTime="end"
let calendarViewRequestStep: MicrosoftGraph.BatchRequestStep = {
  id: "2",
  request: new Request(`/me/calendarview?startDateTime=${start}&endDateTime=${end}`, {
    method: "GET"
  })
}

// Create the batch request content with the steps created
// above
let batchRequestContent = new MicrosoftGraph.BatchRequestContent([
  userRequestStep,
  calendarViewRequestStep
]);

let content = await batchRequestContent.getContent();

// POST the batch request content to the /$batch endpoint
let batchResponse = await client
  .api('/$batch')
  .post(content);

// Create a BatchResponseContent object to parse the response
let batchResponseContent = new MicrosoftGraph.BatchResponseContent(batchResponse);

// Get the user response using the id assigned to the request
let userResponse = batchResponseContent.getResponseById("1");

// For a single entity, the JSON payload can be deserialized
// into the expected type
// Types supplied by @microsoft/microsoft-graph-types
if (userResponse.ok) {
  let user: User = await userResponse.json();
  console.log(`Hello ${user.displayName}!`);
} else {
  console.log(`Get user failed with status ${userResponse.status}`);
}

// Get the calendar view response by id
let calendarResponse = batchResponseContent.getResponseById("2");

// For a collection of entities, the "value" property of
// the JSON payload can be deserialized into an array of
// the expected type
if (calendarResponse.ok) {
  let rawResponse = await calendarResponse.json();
  let events: [Event] = rawResponse.value;
  console.log(`You have ${events.length} events on your calendar today.`);
} else {
  console.log(`Get calendar view failed with status ${calendarResponse.status}`);
}
```

### <a name="java"></a>[Java](#tab/java)

```java
// Create the batch request content with the steps
final MSBatchRequestContent batchRequestContent = new MSBatchRequestContent();

// Use the Graph client to generate the request for GET /me
final String meGetId = batchRequestContent
                        .addBatchRequestStep(graphClient
                                              .me()
                                              .buildRequest()
                                              .withHttpMethod(HttpMethod.GET)
                                              .getHttpRequest());

final ZoneOffset localTimeZone = OffsetDateTime.now().getOffset();
final OffsetDateTime today = OffsetDateTime.of(LocalDate.now(), LocalTime.MIDNIGHT, localTimeZone);
final OffsetDateTime tomorrow = today.plusDays(1);

// Use the Graph client to generate the request URL for
// GET /me/calendarview?startDateTime="start"&endDateTime="end"
final List<Option> calendarViewOptions = Arrays.asList(new QueryOption("startDateTime", today.toString()),
                                                      new QueryOption("endDateTime", tomorrow.toString()));
final String calendarViewRequestStepId = batchRequestContent
                                        .addBatchRequestStep(graphClient
                                          .me()
                                          .calendarView()
                                          .buildRequest(calendarViewOptions)
                                          .withHttpMethod(HttpMethod.GET)
                                          .getHttpRequest());

final ICoreAuthenticationProvider auth =
    (ICoreAuthenticationProvider)graphClient.getAuthenticationProvider();
final OkHttpClient client = HttpClients.createDefault(auth);

// Send the batch request content to the /$batch endpoint
final String batchContent = batchRequestContent.getBatchRequestContent();
final Request batchRequest = new Request.Builder()
    .url("https://graph.microsoft.com/v1.0/$batch")
    .post(RequestBody.create(MediaType.parse("application/json"), batchContent))
    .build();

final Response batchResponse = client.newCall(batchRequest).execute();

final ISerializer graphSerializer = graphClient.getSerializer();

// Create an MSBatchResponseContent object to parse the response
final MSBatchResponseContent batchResponseContent = new MSBatchResponseContent(batchResponse);
// Get the user response using the id assigned to the request
final Response userResponse = batchResponseContent.getResponseById(meGetId);

// For a single entity, the JSON payload can be deserialized
// into the expected type
if (userResponse.isSuccessful()) {
    final User user = graphSerializer.deserializeObject(userResponse.body().string(), User.class);
    System.out.println(String.format("Hello %s!", user.displayName));
} else {
    GraphErrorResponse error = graphSerializer
        .deserializeObject(userResponse.body().string(), GraphErrorResponse.class);
    System.out.println(
        String.format("Error getting user: %s - %s", error.error.code, error.error.message));
}

// Get the calendar view response by id
final Response calendarViewResponse = batchResponseContent.getResponseById(calendarViewRequestStepId);

// For a collection of entities, the JSON payload can be deserialized
// into a *CollectionResponse object. The collection can then be
// accessed via the value property
if (calendarViewResponse.isSuccessful()) {
    final EventCollectionResponse events = graphSerializer
        .deserializeObject(calendarViewResponse.body().string(), EventCollectionResponse.class);
    System.out.println(
        String.format("You have %d events on your calendar today", events.value.size()));
} else {
    GraphErrorResponse error = graphSerializer
        .deserializeObject(calendarViewResponse.body().string(), GraphErrorResponse.class);
    System.out.println(
        String.format("Error getting calendar view: %s - %s", error.error.code, error.error.message));
}
```

---

## <a name="batches-with-dependent-requests"></a>使用从属请求的批处理

此示例演示如何在相互依赖的批次中发送多个请求。 这些请求将按依赖项指定的顺序由服务运行。 本示例在当前日期向用户的日历中添加一个具有开始时间的事件，并获取当前日期的用户日历视图。 若要确保返回的日历审阅包含创建的新事件，则对日历视图的请求配置为依赖于添加新事件的请求。 这将确保先执行添加事件请求。

> [!NOTE]
> 如果添加事件请求失败，获取日历视图请求将失败，并出现 `424 Failed Dependency` 错误。

<!-- markdownlint-disable MD024 -->
### <a name="c"></a>[C#](#tab/csharp)

```csharp
var today = DateTime.Now.Date;

var newEvent = new Event
{
    Subject = "File end-of-day report",
    Start = new DateTimeTimeZone
    {
        // 5:00 PM
        DateTime = today.AddHours(17).ToString("yyyy-MM-ddTHH:mm:ss"),
        TimeZone = TimeZoneInfo.Local.StandardName
    },
    End = new DateTimeTimeZone
    {
        // 5:30 PM
        DateTime = today.AddHours(17).AddMinutes(30).ToString("yyyy-MM-ddTHH:mm:ss"),
        TimeZone = TimeZoneInfo.Local.StandardName
    }
};

// POST requests are handled a bit differently
// The SDK request builders generate GET requests, so
// you must get the HttpRequestMessage and convert to a POST
var jsonEvent = graphClient.HttpProvider.Serializer.SerializeAsJsonContent(newEvent);

var addEventRequest = graphClient.Me.Events.Request().GetHttpRequestMessage();
addEventRequest.Method = HttpMethod.Post;
addEventRequest.Content = jsonEvent;

var start = today.ToString("yyyy-MM-ddTHH:mm:ssK");
var end = today.AddDays(1).ToString("yyyy-MM-ddTHH:mm:ssK");

var queryOptions = new List<QueryOption>
{
    new QueryOption("startDateTime", start),
    new QueryOption("endDateTime", end)
};

// Use the request builder to generate a regular
// request to /me/calendarview?startDateTime="start"&endDateTime="end"
var calendarViewRequest = graphClient.Me.CalendarView.Request(queryOptions);

// Build the batch
var batchRequestContent = new BatchRequestContent();

// Force the requests to execute in order, so that the request for
// today's events will include the new event created.

// First request, no dependency
var addEventRequestId = batchRequestContent.AddBatchRequestStep(addEventRequest);

// Second request, depends on addEventRequestId
var eventsRequestId = Guid.NewGuid().ToString();
batchRequestContent.AddBatchRequestStep(new BatchRequestStep(
    eventsRequestId,
    calendarViewRequest.GetHttpRequestMessage(),
    new List<string> { addEventRequestId }
));

var returnedResponse = await graphClient.Batch.Request().PostAsync(batchRequestContent);

// De-serialize response based on known return type
try
{
    var createdEvent = await returnedResponse
        .GetResponseByIdAsync<Event>(addEventRequestId);
    Console.WriteLine($"New event created with ID: {createdEvent.Id}");
}
catch (ServiceException ex)
{
    Console.WriteLine($"Add event failed: {ex.Error.Message}");
}

// For collections, must use the *CollectionResponse class to deserialize
// The .Value property will contain the *CollectionPage type that the Graph client
// returns from GetAsync().
try
{
    var events = await returnedResponse
        .GetResponseByIdAsync<UserCalendarViewCollectionResponse>(eventsRequestId);
    Console.WriteLine($"You have {events.Value.CurrentPage.Count} events on your calendar today.");
}
catch (ServiceException ex)
{
    Console.WriteLine($"Get calendar view failed: {ex.Error.Message}");
}
```

### <a name="typescript"></a>[TypeScript](#tab/typescript)

```typescript
// 5:00 PM
let eventStart = moment({hour: 17, minute: 0, seconds: 0});

// Create a batch request step to add an event
let newEvent: Event = {
  subject: "File end-of-day report",
  start: {
    dateTime: eventStart
      .format("YYYY-MM-DDTHH:mm:ss"),
    timeZone: moment.tz.guess()
  },
  end: {
    // 5:30 PM
    dateTime: eventStart.add(30, "minutes")
      .format("YYYY-MM-DDTHH:mm:ss"),
    timeZone: moment.tz.guess()
  }
}
console.log(JSON.stringify(newEvent));

let addEventRequestStep: MicrosoftGraph.BatchRequestStep = {
  id: "1",
  request: new Request("/me/events", {
    method: "POST",
    body: JSON.stringify(newEvent),
    headers: {
      "Content-Type": "application/json"
    }
  })
}

let today = moment({hour: 0, minute: 0, seconds: 0});
let start = today.format();
let end = today.add(1, "day").format();
console.log(`/me/calendarview?startDateTime=${start}&endDateTime=${end}`);

// Create a batch request step to GET
// /me/calendarview?startDateTime="start"&endDateTime="end"
let calendarViewRequestStep: MicrosoftGraph.BatchRequestStep = {
  id: "2",
  // This step will happen after step 1
  dependsOn: [ "1" ],
  request: new Request(`/me/calendarview?startDateTime=${start}&endDateTime=${end}`, {
    method: "GET"
  })
}

// Create the batch request content with the steps created
// above
let batchRequestContent = new MicrosoftGraph.BatchRequestContent([
  addEventRequestStep,
  calendarViewRequestStep
]);

let content = await batchRequestContent.getContent();

// POST the batch request content to the /$batch endpoint
let batchResponse = await client
  .api('/$batch')
  .post(content);

// Create a BatchResponseContent object to parse the response
let batchResponseContent = new MicrosoftGraph.BatchResponseContent(batchResponse);

// Get the create event response by id
let newEventResponse = batchResponseContent.getResponseById("1");
if (newEventResponse.ok) {
  let event: Event = await newEventResponse.json();
  console.log(`New event created with ID: ${event.id}`);
} else {
  console.log(`Create event failed with status ${newEventResponse.status}`);
}

// Get the calendar view response by id
let calendarResponse = batchResponseContent.getResponseById("2");

if (calendarResponse.ok)
{
  // For a collection of entities, the "value" property of
  // the JSON payload can be deserialized into an array of
  // the expected type
  let rawResponse = await calendarResponse.json();
  let events: [Event] = rawResponse.value;
  console.log(`You have ${events.length} events on your calendar today.`);
} else {
  console.log(`Get calendar view failed with status ${calendarResponse.status}`);
}
```

### <a name="java"></a>[Java](#tab/java)

```java
// Create the batch request content with the steps
final MSBatchRequestContent batchRequestContent = new MSBatchRequestContent(batchSteps);

final ZoneOffset localTimeZone = OffsetDateTime.now().getOffset();
final OffsetDateTime today = OffsetDateTime.of(LocalDate.now(), LocalTime.MIDNIGHT, localTimeZone);
final OffsetDateTime tomorrow = today.plusDays(1);

// Use the Graph client to generate the request URL for POST /me/events
final Event newEvent = new Event();
newEvent.subject = "File end-of-day report";
newEvent.start = new DateTimeTimeZone();
// 5:00 PM
newEvent.start.dateTime = today.plusHours(17)
    .format(DateTimeFormatter.ISO_LOCAL_DATE_TIME);
newEvent.start.timeZone = ZoneOffset.systemDefault().getId();
newEvent.end = new DateTimeTimeZone();
// 5:30 PM
newEvent.end.dateTime = today.plusHours(17).plusMinutes(30)
    .format(DateTimeFormatter.ISO_LOCAL_DATE_TIME);
newEvent.end.timeZone = ZoneOffset.systemDefault().getId();

final String addEventRequestId = batchRequestContent
                                .addBatchRequestStep(graphClient
                                                .me()
                                                .events()
                                                .buildRequest()
                                                .withHttpMethod(HttpMethod.POST)
                                                .getHttpRequest(newEvent));

// Use the Graph client to generate the request URL for
// GET /me/calendarview?startDateTime="start"&endDateTime="end"
final List<Option> calendarViewOptions = Arrays.asList(new QueryOption("startDateTime", today.toString()),
                                                      new QueryOption("endDateTime", tomorrow.toString()));
final String calendarViewRequestStepId = batchRequestContent
                                        .addBatchRequestStep(graphClient
                                          .me()
                                          .calendarView()
                                          .buildRequest(calendarViewOptions)
                                          .withHttpMethod(HttpMethod.GET)
                                          .getHttpRequest(),
                                          addEventRequestId);

final ICoreAuthenticationProvider auth =
    (ICoreAuthenticationProvider)graphClient.getAuthenticationProvider();
final OkHttpClient client = HttpClients.createDefault(auth);

// Send the batch request content to the /$batch endpoint
final String batchContent = batchRequestContent.getBatchRequestContent();
final Request batchRequest = new Request.Builder()
    .url("https://graph.microsoft.com/v1.0/$batch")
    .post(RequestBody.create(MediaType.parse("application/json"), batchContent))
    .build();

final Response batchResponse = client.newCall(batchRequest).execute();

final ISerializer graphSerializer = graphClient.getSerializer();

// Create an MSBatchResponseContent object to parse the response
final MSBatchResponseContent batchResponseContent = new MSBatchResponseContent(batchResponse);
// Get the user response using the id assigned to the request
final Response addEventResponse = batchResponseContent.getResponseById(addEventRequestId);

// For a single entity, the JSON payload can be deserialized
// into the expected type
  if (addEventResponse.isSuccessful()) {
    final Event event = graphSerializer.deserializeObject(addEventResponse.body().string(), Event.class);
    System.out.println(String.format("New event created with ID: %s", event.id));
} else {
    GraphErrorResponse error = graphSerializer
        .deserializeObject(addEventResponse.body().string(), GraphErrorResponse.class);
    System.out.println(
        String.format("Error creating event: %s - %s", error.error.code, error.error.message));
}

// Get the calendar view response by id
final Response calendarViewResponse = batchResponseContent.getResponseById(calendarViewRequestStepId);

// For a collection of entities, the JSON payload can be deserialized
// into a *CollectionResponse object. The collection can then be
// accessed via the value property
if (calendarViewResponse.isSuccessful()) {
    final EventCollectionResponse events = graphSerializer
        .deserializeObject(calendarViewResponse.body().string(), EventCollectionResponse.class);
    System.out.println(
        String.format("You have %d events on your calendar today", events.value.size()));
} else {
    GraphErrorResponse error = graphSerializer
        .deserializeObject(calendarViewResponse.body().string(), GraphErrorResponse.class);
    System.out.println(
        String.format("Error getting calendar view: %s - %s", error.error.code, error.error.message));
}
```

---
<!-- markdownlint-enable MD024 -->
