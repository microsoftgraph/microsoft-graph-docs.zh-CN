# <a name="create-calendar"></a><span data-ttu-id="d654c-101">创建日历</span><span class="sxs-lookup"><span data-stu-id="d654c-101">Create Calendar</span></span>

<span data-ttu-id="d654c-102">使用此 API 新建日历。</span><span class="sxs-lookup"><span data-stu-id="d654c-102">Use this API to create a new calendar.</span></span>
## <a name="permissions"></a><span data-ttu-id="d654c-103">权限</span><span class="sxs-lookup"><span data-stu-id="d654c-103">Permissions</span></span>
<span data-ttu-id="d654c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="d654c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d654c-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="d654c-106">Permission type</span></span>      | <span data-ttu-id="d654c-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d654c-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d654c-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d654c-108">Delegated (work or school account)</span></span> | <span data-ttu-id="d654c-109">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d654c-109">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="d654c-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d654c-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d654c-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d654c-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="d654c-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="d654c-112">Application</span></span> | <span data-ttu-id="d654c-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d654c-113">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="d654c-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d654c-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/calendars
```
## <a name="request-headers"></a><span data-ttu-id="d654c-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="d654c-115">Request headers</span></span>
| <span data-ttu-id="d654c-116">标头</span><span class="sxs-lookup"><span data-stu-id="d654c-116">Header</span></span>       | <span data-ttu-id="d654c-117">值</span><span class="sxs-lookup"><span data-stu-id="d654c-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d654c-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="d654c-118">Authorization</span></span>  | <span data-ttu-id="d654c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d654c-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d654c-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d654c-121">Content-Type</span></span>  | <span data-ttu-id="d654c-122">application/json</span><span class="sxs-lookup"><span data-stu-id="d654c-122">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d654c-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="d654c-123">Request body</span></span>
<span data-ttu-id="d654c-124">在请求正文中，提供 [calendar](../resources/calendar.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d654c-124">In the request body, supply a JSON representation of [calendar](../resources/calendar.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="d654c-125">响应</span><span class="sxs-lookup"><span data-stu-id="d654c-125">Response</span></span>

<span data-ttu-id="d654c-126">如果成功，此方法在响应正文中返回 `201, Created` 响应代码和 [calendar](../resources/calendar.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d654c-126">If successful, this method returns `201, Created` response code and [calendar](../resources/calendar.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d654c-127">示例</span><span class="sxs-lookup"><span data-stu-id="d654c-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d654c-128">请求</span><span class="sxs-lookup"><span data-stu-id="d654c-128">Request</span></span>
<span data-ttu-id="d654c-129">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d654c-129">Here is an example of the request.</span></span>
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
<span data-ttu-id="d654c-130">在请求正文中，提供 [calendar](../resources/calendar.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d654c-130">In the request body, supply a JSON representation of [calendar](../resources/calendar.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="d654c-131">响应</span><span class="sxs-lookup"><span data-stu-id="d654c-131">Response</span></span>
<span data-ttu-id="d654c-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d654c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
        "name":"Samantha Booth",
        "address":"samanthab@adatum.onmicrosoft.com"
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
