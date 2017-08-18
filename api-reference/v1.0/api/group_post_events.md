# <a name="create-event"></a><span data-ttu-id="bbe4c-101">创建事件</span><span class="sxs-lookup"><span data-stu-id="bbe4c-101">Create Event</span></span>

<span data-ttu-id="bbe4c-102">使用此 API 新建 [事件](../resources/event.md)。</span><span class="sxs-lookup"><span data-stu-id="bbe4c-102">Use this API to create a new [event](../resources/event.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bbe4c-103">先决条件</span><span class="sxs-lookup"><span data-stu-id="bbe4c-103">Prerequisites</span></span>
<span data-ttu-id="bbe4c-104">要执行此 API，需要以下**范围**之一：*Group.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="bbe4c-104">One of the following **scopes** is required to execute this API: *Group.ReadWrite.All*</span></span>
## <a name="http-request"></a><span data-ttu-id="bbe4c-105">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bbe4c-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/events
POST /groups/{id}/calendar/events
```
## <a name="request-headers"></a><span data-ttu-id="bbe4c-106">请求标头</span><span class="sxs-lookup"><span data-stu-id="bbe4c-106">Request headers</span></span>
| <span data-ttu-id="bbe4c-107">标头</span><span class="sxs-lookup"><span data-stu-id="bbe4c-107">Header</span></span>       | <span data-ttu-id="bbe4c-108">值</span><span class="sxs-lookup"><span data-stu-id="bbe4c-108">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="bbe4c-109">Authorization</span><span class="sxs-lookup"><span data-stu-id="bbe4c-109">Authorization</span></span>  | <span data-ttu-id="bbe4c-p101">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bbe4c-p101">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="bbe4c-112">请求正文</span><span class="sxs-lookup"><span data-stu-id="bbe4c-112">Request body</span></span>
<span data-ttu-id="bbe4c-113">在请求正文中，提供 [Event](../resources/event.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bbe4c-113">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="bbe4c-114">响应</span><span class="sxs-lookup"><span data-stu-id="bbe4c-114">Response</span></span>

<span data-ttu-id="bbe4c-115">如果成功，此方法在响应正文中返回 `201, Created` 响应代码和 [Event](../resources/event.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bbe4c-115">If successful, this method returns `201, Created` response code and [event](../resources/event.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bbe4c-116">示例</span><span class="sxs-lookup"><span data-stu-id="bbe4c-116">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bbe4c-117">请求</span><span class="sxs-lookup"><span data-stu-id="bbe4c-117">Request</span></span>
<span data-ttu-id="bbe4c-118">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bbe4c-118">Here is an example of the request.</span></span>
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
<span data-ttu-id="bbe4c-119">在请求正文中，提供 [Event](../resources/event.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bbe4c-119">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="bbe4c-120">响应</span><span class="sxs-lookup"><span data-stu-id="bbe4c-120">Response</span></span>
<span data-ttu-id="bbe4c-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bbe4c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
