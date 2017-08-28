# <a name="list-calendars"></a><span data-ttu-id="cc857-101">列出日历</span><span class="sxs-lookup"><span data-stu-id="cc857-101">List calendars</span></span>

<span data-ttu-id="cc857-102">获取用户的所有日历（`/calendars` 导航属性），从默认日历组或特定日历组中获取日历。</span><span class="sxs-lookup"><span data-stu-id="cc857-102">Get all the user's calendars (`/calendars` navigation property), get the calendars from the default calendar group or from a specific calendar group.</span></span> 
## <a name="permissions"></a><span data-ttu-id="cc857-103">权限</span><span class="sxs-lookup"><span data-stu-id="cc857-103">Permissions</span></span>
<span data-ttu-id="cc857-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="cc857-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="cc857-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="cc857-106">Permission type</span></span>      | <span data-ttu-id="cc857-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cc857-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cc857-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cc857-108">Delegated (work or school account)</span></span> | <span data-ttu-id="cc857-109">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cc857-109">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="cc857-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cc857-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cc857-111">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cc857-111">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="cc857-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="cc857-112">Application</span></span> | <span data-ttu-id="cc857-113">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cc857-113">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="cc857-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cc857-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

<span data-ttu-id="cc857-115">用户的所有日历。</span><span class="sxs-lookup"><span data-stu-id="cc857-115">All the user's calendars.</span></span>
```http
GET /me/calendars
GET /users/{id | userPrincipalName}/calendars
```

<span data-ttu-id="cc857-116">默认 [calendarGroup](../resources/calendarGroup.md) 中的用户日历。</span><span class="sxs-lookup"><span data-stu-id="cc857-116">The user's calendars in the default [calendarGroup](../resources/calendarGroup.md).</span></span>
```http
GET /me/calendargroups/{calendar_group_id}/calendars
GET /users/{id | userPrincipalName}/calendarGroup/calendars
```

<span data-ttu-id="cc857-117">特定 [calendarGroup](../resources/calendarGroup.md) 中的用户日历。</span><span class="sxs-lookup"><span data-stu-id="cc857-117">The user's calendars in a specific [calendarGroup](../resources/calendarGroup.md).</span></span>
```http
GET /me/calendarGroups/{calendar_group_id}/calendars
GET /users/{id | userPrincipalName}/calendarGroups/{calendar_group_id}/calendars
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cc857-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="cc857-118">Optional query parameters</span></span>
<span data-ttu-id="cc857-119">此方法支持 [OData 查询参数](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="cc857-119">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="cc857-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="cc857-120">Request headers</span></span>
| <span data-ttu-id="cc857-121">标头</span><span class="sxs-lookup"><span data-stu-id="cc857-121">Header</span></span>       | <span data-ttu-id="cc857-122">值</span><span class="sxs-lookup"><span data-stu-id="cc857-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cc857-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cc857-123">Authorization</span></span>  | <span data-ttu-id="cc857-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cc857-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="cc857-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cc857-126">Content-Type</span></span>   | <span data-ttu-id="cc857-127">application/json</span><span class="sxs-lookup"><span data-stu-id="cc857-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="cc857-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="cc857-128">Request body</span></span>
<span data-ttu-id="cc857-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cc857-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cc857-130">响应</span><span class="sxs-lookup"><span data-stu-id="cc857-130">Response</span></span>

<span data-ttu-id="cc857-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Calendar](../resources/calendar.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="cc857-131">If successful, this method returns a `200 OK` response code and collection of [Calendar](../resources/calendar.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="cc857-132">示例</span><span class="sxs-lookup"><span data-stu-id="cc857-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cc857-133">请求</span><span class="sxs-lookup"><span data-stu-id="cc857-133">Request</span></span>
<span data-ttu-id="cc857-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cc857-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendars"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendars
```
##### <a name="response"></a><span data-ttu-id="cc857-135">响应</span><span class="sxs-lookup"><span data-stu-id="cc857-135">Response</span></span>
<span data-ttu-id="cc857-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cc857-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#me/calendars",
    "value": [
        {
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
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List calendars",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->