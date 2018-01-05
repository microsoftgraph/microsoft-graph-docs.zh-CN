# <a name="update-event"></a><span data-ttu-id="5daa3-101">更新事件</span><span class="sxs-lookup"><span data-stu-id="5daa3-101">Update event</span></span>
<span data-ttu-id="5daa3-102">更新 [event](../resources/event.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5daa3-102">Update an [event](../resources/event.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5daa3-103">权限</span><span class="sxs-lookup"><span data-stu-id="5daa3-103">Permissions</span></span>
<span data-ttu-id="5daa3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="5daa3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5daa3-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="5daa3-106">Permission type</span></span>      | <span data-ttu-id="5daa3-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5daa3-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5daa3-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5daa3-108">Delegated (work or school account)</span></span> | <span data-ttu-id="5daa3-109">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5daa3-109">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="5daa3-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5daa3-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5daa3-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="5daa3-111">Not supported.</span></span>    |
|<span data-ttu-id="5daa3-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="5daa3-112">Application</span></span> | <span data-ttu-id="5daa3-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="5daa3-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5daa3-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5daa3-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groups/{id}/events/{id}
PATCH /groups/{id}/calendar/events/{id}
```

## <a name="request-headers"></a><span data-ttu-id="5daa3-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="5daa3-115">Request headers</span></span>
| <span data-ttu-id="5daa3-116">名称</span><span class="sxs-lookup"><span data-stu-id="5daa3-116">Name</span></span>       | <span data-ttu-id="5daa3-117">类型</span><span class="sxs-lookup"><span data-stu-id="5daa3-117">Type</span></span> | <span data-ttu-id="5daa3-118">说明</span><span class="sxs-lookup"><span data-stu-id="5daa3-118">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="5daa3-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="5daa3-119">Authorization</span></span>  | <span data-ttu-id="5daa3-120">string</span><span class="sxs-lookup"><span data-stu-id="5daa3-120">string</span></span>  | <span data-ttu-id="5daa3-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5daa3-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5daa3-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="5daa3-123">Request body</span></span>
<span data-ttu-id="5daa3-p103">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="5daa3-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="5daa3-127">响应</span><span class="sxs-lookup"><span data-stu-id="5daa3-127">Response</span></span>
<span data-ttu-id="5daa3-128">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="5daa3-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="5daa3-129">示例</span><span class="sxs-lookup"><span data-stu-id="5daa3-129">Example</span></span>
#### <a name="request"></a><span data-ttu-id="5daa3-130">请求</span><span class="sxs-lookup"><span data-stu-id="5daa3-130">Request</span></span>
<span data-ttu-id="5daa3-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="5daa3-131">The following is an example of the request body.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_group_event"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/groups/{id}/events/{id}
Content-type: application/json
Content-length: 211

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

#### <a name="response"></a><span data-ttu-id="5daa3-132">响应</span><span class="sxs-lookup"><span data-stu-id="5daa3-132">Response</span></span>
<span data-ttu-id="5daa3-133">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="5daa3-133">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update event",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->