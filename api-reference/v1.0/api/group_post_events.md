# <a name="create-event"></a><span data-ttu-id="950db-101">创建事件</span><span class="sxs-lookup"><span data-stu-id="950db-101">Create Event</span></span>
<span data-ttu-id="950db-102">使用此 API 新建[事件](../resources/event.md)。</span><span class="sxs-lookup"><span data-stu-id="950db-102">Use this API to create a new [event](../resources/event.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="950db-103">权限</span><span class="sxs-lookup"><span data-stu-id="950db-103">Permissions</span></span>
<span data-ttu-id="950db-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="950db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="950db-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="950db-106">Permission type</span></span>      | <span data-ttu-id="950db-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="950db-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="950db-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="950db-108">Delegated (work or school account)</span></span> | <span data-ttu-id="950db-109">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="950db-109">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="950db-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="950db-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="950db-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="950db-111">Not supported.</span></span>    |
|<span data-ttu-id="950db-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="950db-112">Application</span></span> | <span data-ttu-id="950db-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="950db-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="950db-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="950db-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/events
POST /groups/{id}/calendar/events
```

## <a name="request-headers"></a><span data-ttu-id="950db-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="950db-115">Request headers</span></span>
| <span data-ttu-id="950db-116">标头</span><span class="sxs-lookup"><span data-stu-id="950db-116">Header</span></span>       | <span data-ttu-id="950db-117">值</span><span class="sxs-lookup"><span data-stu-id="950db-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="950db-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="950db-118">Authorization</span></span>  | <span data-ttu-id="950db-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="950db-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="950db-121">请求正文</span><span class="sxs-lookup"><span data-stu-id="950db-121">Request body</span></span>
<span data-ttu-id="950db-122">在请求正文中，提供 [event](../resources/event.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="950db-122">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="950db-123">响应</span><span class="sxs-lookup"><span data-stu-id="950db-123">Response</span></span>
<span data-ttu-id="950db-124">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [event](../resources/event.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="950db-124">If successful, this method returns `201 Created` response code and [event](../resources/event.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="950db-125">示例</span><span class="sxs-lookup"><span data-stu-id="950db-125">Example</span></span>
#### <a name="request"></a><span data-ttu-id="950db-126">请求</span><span class="sxs-lookup"><span data-stu-id="950db-126">Request</span></span>
<span data-ttu-id="950db-127">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="950db-127">The following is an example of the request body.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_event_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/events
Content-type: application/json
Content-length: 285

{
  "originalStartTimeZone": "originalStartTimeZone-value",
  "originalEndTimeZone": "originalEndTimeZone-value",
  "responseStatus": {
    "response": "",
    "time": "datetime-value"
  },
  "iCalUId": "iCalUId-value",
  "reminderMinutesBeforeStart": 99,
  "isReminderOn": true
}
```
<span data-ttu-id="950db-128">在请求正文中，提供 [event](../resources/event.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="950db-128">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

#### <a name="response"></a><span data-ttu-id="950db-129">响应</span><span class="sxs-lookup"><span data-stu-id="950db-129">Response</span></span>
<span data-ttu-id="950db-130">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="950db-130">Here is an example of the response.</span></span>
><span data-ttu-id="950db-131">**注意：**为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="950db-131">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="950db-132">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="950db-132">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 285

{
  "originalStartTimeZone": "originalStartTimeZone-value",
  "originalEndTimeZone": "originalEndTimeZone-value",
  "responseStatus": {
    "response": "",
    "time": "datetime-value"
  },
  "iCalUId": "iCalUId-value",
  "reminderMinutesBeforeStart": 99,
  "isReminderOn": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Event",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
