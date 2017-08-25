# <a name="create-calendar"></a><span data-ttu-id="2b0da-101">创建日历</span><span class="sxs-lookup"><span data-stu-id="2b0da-101">Create Calendar</span></span>

<span data-ttu-id="2b0da-102">使用此 API 在日历组中创建新日历。</span><span class="sxs-lookup"><span data-stu-id="2b0da-102">Use this API to create a new Calendar in a calendar group.</span></span>
## <a name="permissions"></a><span data-ttu-id="2b0da-103">权限</span><span class="sxs-lookup"><span data-stu-id="2b0da-103">Permissions</span></span>
<span data-ttu-id="2b0da-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="2b0da-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2b0da-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="2b0da-106">Permission type</span></span>      | <span data-ttu-id="2b0da-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2b0da-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="2b0da-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2b0da-108">Delegated (work or school account)</span></span> | <span data-ttu-id="2b0da-109">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2b0da-109">Calendars.ReadWrite</span></span>    | 
|<span data-ttu-id="2b0da-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2b0da-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2b0da-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2b0da-111">Calendars.ReadWrite</span></span>    | 
|<span data-ttu-id="2b0da-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="2b0da-112">Application</span></span> | <span data-ttu-id="2b0da-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2b0da-113">Calendars.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="2b0da-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2b0da-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="2b0da-115">用户的默认 [calendarGroup](../resources/calendargroup.md)。</span><span class="sxs-lookup"><span data-stu-id="2b0da-115">A user's default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
POST /me/calendarGroup/calendars
POST /users/{id | userPrincipalName}/calendarGroup/calendars
```
<span data-ttu-id="2b0da-116">用户的任意 [calendarGroup](../resources/calendargroup.md)。</span><span class="sxs-lookup"><span data-stu-id="2b0da-116">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>
```http
POST /me/calendarGroups/{id}/calendars
POST /users/{id | userPrincipalName}/calendarGroups/{id}/calendars
```
## <a name="request-headers"></a><span data-ttu-id="2b0da-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="2b0da-117">Request headers</span></span>
| <span data-ttu-id="2b0da-118">标头</span><span class="sxs-lookup"><span data-stu-id="2b0da-118">Header</span></span>       | <span data-ttu-id="2b0da-119">值</span><span class="sxs-lookup"><span data-stu-id="2b0da-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2b0da-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="2b0da-120">Authorization</span></span>  | <span data-ttu-id="2b0da-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2b0da-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="2b0da-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2b0da-123">Content-Type</span></span>  | <span data-ttu-id="2b0da-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="2b0da-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2b0da-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="2b0da-126">Request body</span></span>
<span data-ttu-id="2b0da-127">在请求正文中，提供 [Calendar](../resources/calendar.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2b0da-127">In the request body, supply a JSON representation of [Calendar](../resources/calendar.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="2b0da-128">响应</span><span class="sxs-lookup"><span data-stu-id="2b0da-128">Response</span></span>

<span data-ttu-id="2b0da-129">如果成功，此方法在响应正文中返回 `201, Created` 响应代码和 [Calendar](../resources/calendar.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2b0da-129">If successful, this method returns `201, Created` response code and [Calendar](../resources/calendar.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2b0da-130">示例</span><span class="sxs-lookup"><span data-stu-id="2b0da-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2b0da-131">请求</span><span class="sxs-lookup"><span data-stu-id="2b0da-131">Request</span></span>
<span data-ttu-id="2b0da-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2b0da-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_calendar_from_calendargroup"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/calendarGroups/{id}/calendars
Content-type: application/json
Content-length: 78

{
  "name": "name-value",
  "color": {
  }
}
```
<span data-ttu-id="2b0da-133">在请求正文中，提供 [calendar](../resources/calendar.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2b0da-133">In the request body, supply a JSON representation of [calendar](../resources/calendar.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="2b0da-134">响应</span><span class="sxs-lookup"><span data-stu-id="2b0da-134">Response</span></span>
<span data-ttu-id="2b0da-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2b0da-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 98

{
  "name": "name-value",
  "color": {
  },
  "changeKey": "changeKey-value",
  "id": "id-value"
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
