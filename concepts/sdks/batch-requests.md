---
title: 使用 Microsoft Graph SDK 批处理请求
description: 提供有关使用 Microsoft Graph SDK 创建一批 API 请求的说明。
localization_priority: Normal
author: DarrelMiller
ms.openlocfilehash: 2f9caf9ad7f20dd2b6601501fa8c6a8fb1541bde
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51509007"
---
# <a name="use-the-microsoft-graph-sdks-to-batch-requests"></a><span data-ttu-id="2da34-103">使用 Microsoft Graph SDK 批处理请求</span><span class="sxs-lookup"><span data-stu-id="2da34-103">Use the Microsoft Graph SDKs to batch requests</span></span>

<span data-ttu-id="2da34-104">[批处理](../json-batching.md) 是一种将多个请求合并到单个 HTTP 请求中的方法。</span><span class="sxs-lookup"><span data-stu-id="2da34-104">[Batching](../json-batching.md) is a way of combining multiple requests into a single HTTP request.</span></span> <span data-ttu-id="2da34-105">请求组合在单个 JSON 有效负载中，该负载通过 POST 发送到 `\$batch` 终结点。</span><span class="sxs-lookup"><span data-stu-id="2da34-105">The requests are combined in a single JSON payload, which is sent via POST to the `\$batch` endpoint.</span></span> <span data-ttu-id="2da34-106">Microsoft Graph SDK 具有一组类，用于简化如何创建批处理有效负载和分析批处理响应有效负载。</span><span class="sxs-lookup"><span data-stu-id="2da34-106">Microsoft Graph SDKs have a set of classes to simplify how you create batch payloads and parse batch response payloads.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="2da34-107">有关 Microsoft Graph 中 JSON 批处理的当前限制，请参阅 [已知问题](../known-issues.md#json-batching)。</span><span class="sxs-lookup"><span data-stu-id="2da34-107">For current limitations with JSON batching in Microsoft Graph, see [Known Issues](../known-issues.md#json-batching).</span></span>

## <a name="create-a-batch-request"></a><span data-ttu-id="2da34-108">创建批处理请求</span><span class="sxs-lookup"><span data-stu-id="2da34-108">Create a batch request</span></span>

<span data-ttu-id="2da34-109">Microsoft Graph SDK 提供了三个类，用于处理批处理请求和响应。</span><span class="sxs-lookup"><span data-stu-id="2da34-109">The Microsoft Graph SDKs provide three classes to work with batch requests and responses.</span></span>

- <span data-ttu-id="2da34-110">**BatchRequestStep** - 表示单个请求 (，) `GET /me` 批处理中的请求。</span><span class="sxs-lookup"><span data-stu-id="2da34-110">**BatchRequestStep** - Represents a single request (such as `GET /me`) within a batch.</span></span> <span data-ttu-id="2da34-111">它支持为请求分配唯一标识符并指定请求之间的依赖关系。</span><span class="sxs-lookup"><span data-stu-id="2da34-111">It enables assigning a unique identifier to the request and specifying dependencies between requests.</span></span>
- <span data-ttu-id="2da34-112">**BatchRequestContent** - 简化批处理请求有效负载的创建。</span><span class="sxs-lookup"><span data-stu-id="2da34-112">**BatchRequestContent** - Simplifies creating the batch request payload.</span></span> <span data-ttu-id="2da34-113">它包含多个 **BatchRequestStep** 对象。</span><span class="sxs-lookup"><span data-stu-id="2da34-113">It contains multiple **BatchRequestStep** objects.</span></span>
- <span data-ttu-id="2da34-114">**BatchResponseContent** - 简化了分析来自批处理请求的响应。</span><span class="sxs-lookup"><span data-stu-id="2da34-114">**BatchResponseContent** - Simplifies parsing the response from a batch request.</span></span> <span data-ttu-id="2da34-115">它提供获取所有响应、按 ID 获取特定响应以及获取 `@odata.nextLink` 属性（如果存在）的能力。</span><span class="sxs-lookup"><span data-stu-id="2da34-115">It provides the ability to get all responses, get a specific response by ID, and get the `@odata.nextLink` property if present.</span></span>

## <a name="simple-batching-example"></a><span data-ttu-id="2da34-116">简单批处理示例</span><span class="sxs-lookup"><span data-stu-id="2da34-116">Simple batching example</span></span>

<span data-ttu-id="2da34-117">此示例演示如何在一个批处理中发送多个不彼此依赖的请求。</span><span class="sxs-lookup"><span data-stu-id="2da34-117">This example shows how to send multiple requests in a batch that are not dependent on each other.</span></span> <span data-ttu-id="2da34-118">服务可以按任意顺序运行请求。</span><span class="sxs-lookup"><span data-stu-id="2da34-118">The requests can be run by the service in any order.</span></span> <span data-ttu-id="2da34-119">此示例获取用户并获取当前日期的用户日历视图。</span><span class="sxs-lookup"><span data-stu-id="2da34-119">This example gets the user and gets the user's calendar view for the current day.</span></span>

### <a name="c"></a>[<span data-ttu-id="2da34-120">C#</span><span class="sxs-lookup"><span data-stu-id="2da34-120">C#</span></span>](#tab/csharp)

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

### <a name="typescript"></a>[<span data-ttu-id="2da34-121">TypeScript</span><span class="sxs-lookup"><span data-stu-id="2da34-121">TypeScript</span></span>](#tab/typescript)

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

### <a name="java"></a>[<span data-ttu-id="2da34-122">Java</span><span class="sxs-lookup"><span data-stu-id="2da34-122">Java</span></span>](#tab/java)

```java
// Create the batch request content with the steps
final BatchRequestContent batchRequestContent = new BatchRequestContent();

// Use the Graph client to generate the request for GET /me
final String meGetId = batchRequestContent
                        .addBatchRequestStep(graphClient
                                              .me()
                                              .buildRequest());

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
                                          .buildRequest(calendarViewOptions));

// Send the batch request content to the /$batch endpoint
final BatchResponseContent batchResponseContent = graphClient.batch().buildRequest().post(batchRequestContent);
// Get the user response using the id assigned to the request
final User user = batchResponseContent.getResponseById(meGetId).getDeserializedBody(User.class);
System.out.println(String.format("Hello %s!", user.displayName));

// Get the calendar view response by id
final EventCollectionResponse events = batchResponseContent.getResponseById(calendarViewRequestStepId).getDeserializedBody(EventCollectionResponse.class);
System.out.println(String.format("You have %d events on your calendar today", events.value.size()));
```

---

## <a name="batches-with-dependent-requests"></a><span data-ttu-id="2da34-123">具有相关请求的批处理</span><span class="sxs-lookup"><span data-stu-id="2da34-123">Batches with dependent requests</span></span>

<span data-ttu-id="2da34-124">此示例演示如何在批处理中发送多个相互依赖的请求。</span><span class="sxs-lookup"><span data-stu-id="2da34-124">This example shows how to send multiple requests in a batch that are dependent on each other.</span></span> <span data-ttu-id="2da34-125">请求将按依赖项指定的顺序由服务运行。</span><span class="sxs-lookup"><span data-stu-id="2da34-125">The requests will be run by the service in the order specified by the dependencies.</span></span> <span data-ttu-id="2da34-126">本示例向用户的日历添加一个事件，其开始时间为当前日期，并获取当前日期的用户日历视图。</span><span class="sxs-lookup"><span data-stu-id="2da34-126">This example adds an event with a start time during the current day to the user's calendar and gets the user's calendar view for the current day.</span></span> <span data-ttu-id="2da34-127">若要确保返回的日历审阅包含创建的新事件，将日历视图请求配置为依赖于添加新事件的请求。</span><span class="sxs-lookup"><span data-stu-id="2da34-127">To make sure that the calendar review returned includes the new event created, the request for the calendar view is configured as dependent on the request to add the new event.</span></span> <span data-ttu-id="2da34-128">这将确保首先执行添加事件请求。</span><span class="sxs-lookup"><span data-stu-id="2da34-128">This ensures that the add event request will execute first.</span></span>

> [!NOTE]
> <span data-ttu-id="2da34-129">如果添加事件请求失败，则获取日历视图请求将失败并出现错误 `424 Failed Dependency` 。</span><span class="sxs-lookup"><span data-stu-id="2da34-129">If the add event request fails, the get calendar view request will fail with a `424 Failed Dependency` error.</span></span>

<!-- markdownlint-disable MD024 -->
### <a name="c"></a>[<span data-ttu-id="2da34-130">C#</span><span class="sxs-lookup"><span data-stu-id="2da34-130">C#</span></span>](#tab/csharp)

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

### <a name="typescript"></a>[<span data-ttu-id="2da34-131">TypeScript</span><span class="sxs-lookup"><span data-stu-id="2da34-131">TypeScript</span></span>](#tab/typescript)

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

### <a name="java"></a>[<span data-ttu-id="2da34-132">Java</span><span class="sxs-lookup"><span data-stu-id="2da34-132">Java</span></span>](#tab/java)

```java
// Create the batch request content with the steps
final BatchRequestContent batchRequestContent = new BatchRequestContent(batchSteps);

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
                                                .buildRequest(), HttpMethod.POST, newEvent);

// Use the Graph client to generate the request URL for
// GET /me/calendarview?startDateTime="start"&endDateTime="end"
final List<Option> calendarViewOptions = Arrays.asList(new QueryOption("startDateTime", today.toString()),
                                                      new QueryOption("endDateTime", tomorrow.toString()));
final String calendarViewRequestStepId = batchRequestContent
                                        .addBatchRequestStep(graphClient
                                          .me()
                                          .calendarView()
                                          .buildRequest(calendarViewOptions),
                                          HttpMethod.GET,
                                          null,
                                          addEventRequestId);

// Send the batch request content to the /$batch endpoint
final BatchResponseContent batchResponseContent = client.batch().buildRequest().post(batchRequestContent);
// Get the user response using the id assigned to the request
final Event event = batchResponseContent.getResponseById(addEventRequestId).getDeserializedBody(Event.class);
System.out.println(String.format("New event created with ID: %s", event.id));

// Get the calendar view response by id
final EventCollectionResponse events = batchResponseContent.getResponseById(calendarViewRequestStepId).getDeserializedBody(EventCollectionResponse.class);
System.out.println(String.format("You have %d events on your calendar today", events.value.size()));
```

---
<!-- markdownlint-enable MD024 -->
