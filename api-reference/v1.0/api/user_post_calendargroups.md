# <a name="create-calendargroup"></a><span data-ttu-id="44744-101">创建 CalendarGroup</span><span class="sxs-lookup"><span data-stu-id="44744-101">Create CalendarGroup</span></span>

<span data-ttu-id="44744-102">使用此 API 创建新的 CalendarGroup。</span><span class="sxs-lookup"><span data-stu-id="44744-102">Use this API to create a new CalendarGroup.</span></span>
## <a name="permissions"></a><span data-ttu-id="44744-103">权限</span><span class="sxs-lookup"><span data-stu-id="44744-103">Permissions</span></span>
<span data-ttu-id="44744-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="44744-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="44744-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="44744-106">Permission type</span></span>      | <span data-ttu-id="44744-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="44744-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="44744-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="44744-108">Delegated (work or school account)</span></span> | <span data-ttu-id="44744-109">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="44744-109">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="44744-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="44744-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="44744-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="44744-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="44744-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="44744-112">Application</span></span> | <span data-ttu-id="44744-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="44744-113">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="44744-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="44744-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/calendarGroups
```
## <a name="request-headers"></a><span data-ttu-id="44744-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="44744-115">Request headers</span></span>
| <span data-ttu-id="44744-116">标头</span><span class="sxs-lookup"><span data-stu-id="44744-116">Header</span></span>       | <span data-ttu-id="44744-117">值</span><span class="sxs-lookup"><span data-stu-id="44744-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="44744-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="44744-118">Authorization</span></span>  | <span data-ttu-id="44744-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="44744-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="44744-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="44744-121">Content-Type</span></span>  | <span data-ttu-id="44744-122">application/json</span><span class="sxs-lookup"><span data-stu-id="44744-122">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="44744-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="44744-123">Request body</span></span>
<span data-ttu-id="44744-124">在请求正文中，提供 [CalendarGroup](../resources/calendargroup.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="44744-124">In the request body, supply a JSON representation of [CalendarGroup](../resources/calendargroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="44744-125">响应</span><span class="sxs-lookup"><span data-stu-id="44744-125">Response</span></span>

<span data-ttu-id="44744-126">如果成功，此方法在响应正文中返回 `201, Created` 响应代码和 [CalendarGroup](../resources/calendargroup.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="44744-126">If successful, this method returns `201, Created` response code and [CalendarGroup](../resources/calendargroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="44744-127">示例</span><span class="sxs-lookup"><span data-stu-id="44744-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="44744-128">请求</span><span class="sxs-lookup"><span data-stu-id="44744-128">Request</span></span>
<span data-ttu-id="44744-129">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="44744-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_calendargroup_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/calendarGroups
Content-type: application/json
Content-length: 90

{
  "name": "name-value",
  "classId": "classId-value",
  "changeKey": "changeKey-value"
}
```
<span data-ttu-id="44744-130">在请求正文中，提供 [CalendarGroup](../resources/calendargroup.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="44744-130">In the request body, supply a JSON representation of [calendarGroup](../resources/calendargroup.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="44744-131">响应</span><span class="sxs-lookup"><span data-stu-id="44744-131">Response</span></span>
<span data-ttu-id="44744-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="44744-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendarGroup"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 110

{
  "name": "name-value",
  "classId": "classId-value",
  "changeKey": "changeKey-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create CalendarGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
