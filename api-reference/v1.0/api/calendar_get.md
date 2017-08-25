# <a name="get-calendar"></a><span data-ttu-id="6b9cd-101">获取日历</span><span class="sxs-lookup"><span data-stu-id="6b9cd-101">Get calendar</span></span>

<span data-ttu-id="6b9cd-102">检索 calendar 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6b9cd-102">Retrieve the properties and relationships of calendar object.</span></span>
## <a name="permissions"></a><span data-ttu-id="6b9cd-103">权限</span><span class="sxs-lookup"><span data-stu-id="6b9cd-103">Permissions</span></span>
<span data-ttu-id="6b9cd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="6b9cd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="6b9cd-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="6b9cd-106">Permission type</span></span>      | <span data-ttu-id="6b9cd-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6b9cd-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="6b9cd-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6b9cd-108">Delegated (work or school account)</span></span> | <span data-ttu-id="6b9cd-109">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="6b9cd-109">Calendars.Read</span></span>    | 
|<span data-ttu-id="6b9cd-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6b9cd-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6b9cd-111">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="6b9cd-111">Calendars.Read</span></span>    | 
|<span data-ttu-id="6b9cd-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="6b9cd-112">Application</span></span> | <span data-ttu-id="6b9cd-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="6b9cd-113">Calendars.Read</span></span> | 

## <a name="http-request"></a><span data-ttu-id="6b9cd-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6b9cd-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="6b9cd-115">用户或组的默认 [日历](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="6b9cd-115">A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
GET /me/calendar
GET /users/{id | userPrincipalName}/calendar
GET /groups/{id}/calendar
```
<span data-ttu-id="6b9cd-116">默认 [calendarGroup](../resources/calendargroup.md) 中用户的 [日历](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="6b9cd-116">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendars/{id}
GET /users/{id | userPrincipalName}/calendars/{id}

GET /me/calendarGroup/calendars/{id}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}
```
<span data-ttu-id="6b9cd-117">指定 [calendarGroup](../resources/calendargroup.md) 中用户的 [日历](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="6b9cd-117">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{id}/calendars/{id}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6b9cd-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="6b9cd-118">Optional query parameters</span></span>
<span data-ttu-id="6b9cd-119">此方法支持 [OData 查询参数](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="6b9cd-119">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="6b9cd-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6b9cd-120">Request headers</span></span>
| <span data-ttu-id="6b9cd-121">名称</span><span class="sxs-lookup"><span data-stu-id="6b9cd-121">Name</span></span>       | <span data-ttu-id="6b9cd-122">类型</span><span class="sxs-lookup"><span data-stu-id="6b9cd-122">Type</span></span> | <span data-ttu-id="6b9cd-123">说明</span><span class="sxs-lookup"><span data-stu-id="6b9cd-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="6b9cd-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="6b9cd-124">Authorization</span></span>  | <span data-ttu-id="6b9cd-125">string</span><span class="sxs-lookup"><span data-stu-id="6b9cd-125">string</span></span>  | <span data-ttu-id="6b9cd-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6b9cd-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6b9cd-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="6b9cd-128">Request body</span></span>
<span data-ttu-id="6b9cd-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6b9cd-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6b9cd-130">响应</span><span class="sxs-lookup"><span data-stu-id="6b9cd-130">Response</span></span>

<span data-ttu-id="6b9cd-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [calendar](../resources/calendar.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6b9cd-131">If successful, this method returns a `200 OK` response code and [calendar](../resources/calendar.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6b9cd-132">示例</span><span class="sxs-lookup"><span data-stu-id="6b9cd-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6b9cd-133">请求</span><span class="sxs-lookup"><span data-stu-id="6b9cd-133">Request</span></span>
<span data-ttu-id="6b9cd-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6b9cd-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendar"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendar
```
##### <a name="response"></a><span data-ttu-id="6b9cd-135">响应</span><span class="sxs-lookup"><span data-stu-id="6b9cd-135">Response</span></span>
<span data-ttu-id="6b9cd-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6b9cd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
        "name":"Fanny Downs",
        "address":"fannyd@adatum.onmicrosoft.com"
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
