# <a name="create-calendar"></a><span data-ttu-id="d9d47-101">创建日历</span><span class="sxs-lookup"><span data-stu-id="d9d47-101">Create Calendar</span></span>

<span data-ttu-id="d9d47-102">使用此 API 创建新的日历。</span><span class="sxs-lookup"><span data-stu-id="d9d47-102">Use this API to create a new calendar.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d9d47-103">先决条件</span><span class="sxs-lookup"><span data-stu-id="d9d47-103">Prerequisites</span></span>
<span data-ttu-id="d9d47-104">要执行此 API，需要以下**范围**之一：*Calendars.ReadWrite*</span><span class="sxs-lookup"><span data-stu-id="d9d47-104">One of the following **scopes** is required to execute this API: *Calendars.ReadWrite*</span></span>
## <a name="http-request"></a><span data-ttu-id="d9d47-105">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d9d47-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/calendars
```
## <a name="request-headers"></a><span data-ttu-id="d9d47-106">请求标头</span><span class="sxs-lookup"><span data-stu-id="d9d47-106">Request headers</span></span>
| <span data-ttu-id="d9d47-107">标头</span><span class="sxs-lookup"><span data-stu-id="d9d47-107">Header</span></span>       | <span data-ttu-id="d9d47-108">值</span><span class="sxs-lookup"><span data-stu-id="d9d47-108">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d9d47-109">Authorization</span><span class="sxs-lookup"><span data-stu-id="d9d47-109">Authorization</span></span>  | <span data-ttu-id="d9d47-p101">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d9d47-p101">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d9d47-112">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d9d47-112">Content-Type</span></span>  | <span data-ttu-id="d9d47-113">application/json</span><span class="sxs-lookup"><span data-stu-id="d9d47-113">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d9d47-114">请求正文</span><span class="sxs-lookup"><span data-stu-id="d9d47-114">Request body</span></span>
<span data-ttu-id="d9d47-115">在请求正文中，提供 [calendar](../resources/calendar.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d9d47-115">In the request body, supply a JSON representation of [calendar](../resources/calendar.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="d9d47-116">响应</span><span class="sxs-lookup"><span data-stu-id="d9d47-116">Response</span></span>

<span data-ttu-id="d9d47-117">如果成功，此方法在响应正文中返回 `201, Created` 响应代码和 [calendar](../resources/calendar.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d9d47-117">If successful, this method returns `201, Created` response code and [calendar](../resources/calendar.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d9d47-118">示例</span><span class="sxs-lookup"><span data-stu-id="d9d47-118">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d9d47-119">请求</span><span class="sxs-lookup"><span data-stu-id="d9d47-119">Request</span></span>
<span data-ttu-id="d9d47-120">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d9d47-120">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_calendar_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/calendars
Content-type: application/json

{
  "name": "Volunteer"
}
```
<span data-ttu-id="d9d47-121">在请求正文中，提供 [calendar](../resources/calendar.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d9d47-121">In the request body, supply a JSON representation of [calendar](../resources/calendar.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="d9d47-122">响应</span><span class="sxs-lookup"><span data-stu-id="d9d47-122">Response</span></span>
<span data-ttu-id="d9d47-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d9d47-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#me/calendars/$entity",
    "@odata.id":"https://graph.microsoft.com/v1.0/users('266efe5a-0fd7-4edd-877b-b2d1e561f193@ae01a323-3934-4475-a32d-af1274312bb0')/calendars('AAMkADJmMVAAA=')",
    "id":"AAMkADJmMVAAA=",
    "name":"Volunteer",
    "color":"auto",
    "changeKey":"DxYSthXJXEWwAQSYQnXvIgAAIxGttg==",
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
  "description": "Create Calendar",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
