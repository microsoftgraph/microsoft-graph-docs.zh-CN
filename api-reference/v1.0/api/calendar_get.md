# <a name="get-calendar"></a><span data-ttu-id="f0841-101">获取 calendar</span><span class="sxs-lookup"><span data-stu-id="f0841-101">Get calendar</span></span>

<span data-ttu-id="f0841-102">获取 [calendar](../resources/calendar.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f0841-102">Get the properties and relationships of a [calendar](../resources/calendar.md) object.</span></span> <span data-ttu-id="f0841-103">可以是[用户](../resources/user.md)的日历，也可以是 Office 365 [组](../resources/group.md)的默认日历。</span><span class="sxs-lookup"><span data-stu-id="f0841-103">The calendar can be one for a [user](../resources/user.md), or the default calendar of an Office 365 [group](../resources/group.md).</span></span>

<span data-ttu-id="f0841-104">有两种应用程序可以获取另一个用户的日历的情景：</span><span class="sxs-lookup"><span data-stu-id="f0841-104">There are two scenarios where an app can get another user's calendar:</span></span>

* <span data-ttu-id="f0841-105">如果应用拥有应用程序权限，或者，</span><span class="sxs-lookup"><span data-stu-id="f0841-105">If the app has application permissions, or,</span></span>
* <span data-ttu-id="f0841-106">如果应用拥有来自一个用户的适当的委派[权限](#permissions)，而另一个用户与该用户共享了日历，或者已授予该用户委派访问权限。</span><span class="sxs-lookup"><span data-stu-id="f0841-106">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a calendar with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="f0841-107">请参阅[详细信息和示例](../../../concepts/outlook-get-shared-events-calendars.md)。</span><span class="sxs-lookup"><span data-stu-id="f0841-107">See [details and an example](../../../concepts/outlook-get-shared-events-calendars.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f0841-108">权限</span><span class="sxs-lookup"><span data-stu-id="f0841-108">Permissions</span></span>
<span data-ttu-id="f0841-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="f0841-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f0841-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f0841-111">Permission type</span></span>      | <span data-ttu-id="f0841-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f0841-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f0841-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f0841-113">Delegated (work or school account)</span></span> | <span data-ttu-id="f0841-114">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="f0841-114">Calendars.Read</span></span>    |
|<span data-ttu-id="f0841-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f0841-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f0841-116">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="f0841-116">Calendars.Read</span></span>    |
|<span data-ttu-id="f0841-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f0841-117">Application</span></span> | <span data-ttu-id="f0841-118">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="f0841-118">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="f0841-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f0841-119">HTTP request</span></span>
<span data-ttu-id="f0841-120"><!-- { "blockType": "ignored" } --> 用户或组的默认[日历](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="f0841-120">A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
GET /me/calendar
GET /users/{id | userPrincipalName}/calendar
GET /groups/{id}/calendar
```
<span data-ttu-id="f0841-121">默认 [calendarGroup](../resources/calendargroup.md) 中的用户 [calendar](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="f0841-121">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendars/{id}
GET /users/{id | userPrincipalName}/calendars/{id}

GET /me/calendarGroup/calendars/{id}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}
```
<span data-ttu-id="f0841-122">指定 [calendarGroup](../resources/calendargroup.md) 中用户的 [日历](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="f0841-122">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{id}/calendars/{id}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f0841-123">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f0841-123">Optional query parameters</span></span>
<span data-ttu-id="f0841-124">此方法支持 [OData 查询参数](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f0841-124">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="f0841-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="f0841-125">Request headers</span></span>
| <span data-ttu-id="f0841-126">名称</span><span class="sxs-lookup"><span data-stu-id="f0841-126">Name</span></span>       | <span data-ttu-id="f0841-127">类型</span><span class="sxs-lookup"><span data-stu-id="f0841-127">Type</span></span> | <span data-ttu-id="f0841-128">说明</span><span class="sxs-lookup"><span data-stu-id="f0841-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f0841-129">授权</span><span class="sxs-lookup"><span data-stu-id="f0841-129">Authorization</span></span>  | <span data-ttu-id="f0841-130">字符串</span><span class="sxs-lookup"><span data-stu-id="f0841-130">string</span></span>  | <span data-ttu-id="f0841-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f0841-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f0841-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="f0841-133">Request body</span></span>
<span data-ttu-id="f0841-134">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f0841-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f0841-135">响应</span><span class="sxs-lookup"><span data-stu-id="f0841-135">Response</span></span>

<span data-ttu-id="f0841-136">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [calendar](../resources/calendar.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f0841-136">If successful, this method returns a `200 OK` response code and [calendar](../resources/calendar.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f0841-137">示例</span><span class="sxs-lookup"><span data-stu-id="f0841-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f0841-138">请求</span><span class="sxs-lookup"><span data-stu-id="f0841-138">Request</span></span>
<span data-ttu-id="f0841-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f0841-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendar"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendar
```
##### <a name="response"></a><span data-ttu-id="f0841-140">响应</span><span class="sxs-lookup"><span data-stu-id="f0841-140">Response</span></span>
<span data-ttu-id="f0841-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f0841-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#me/calendars/$entity",
    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfcd489-628b-40d7-b48b-57002df800e5@1717622f-1d94-4d0c-9d74-709fad664b77')/calendars('AAMkAGI2TGuLAAA=')",
    "id": "AAMkAGI2TGuLAAA=",
    "name": "Calendar",
    "color": "auto",
    "changeKey": "nfZyf7VcrEKLNoU37KWlkQAAA0x0+w==",
    "canShare":true,
    "canViewPrivateItems":true,
    "canEdit":true,
    "owner":{
        "name":"Samantha Booth",
        "address":"samanthab@adatum.onmicrosoft.com"
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get calendar",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
