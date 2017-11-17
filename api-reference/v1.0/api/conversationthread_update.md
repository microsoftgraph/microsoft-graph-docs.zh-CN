# <a name="update-conversationthread"></a><span data-ttu-id="ca2be-101">更新 conversationthread</span><span class="sxs-lookup"><span data-stu-id="ca2be-101">Update conversationthread</span></span>

<span data-ttu-id="ca2be-102">锁定或解锁线程，以允许或避免进一步向线程发布。</span><span class="sxs-lookup"><span data-stu-id="ca2be-102">Lock or unlock a thread, to allow or avoid further posting to the thread.</span></span>
## <a name="permissions"></a><span data-ttu-id="ca2be-103">权限</span><span class="sxs-lookup"><span data-stu-id="ca2be-103">Permissions</span></span>
<span data-ttu-id="ca2be-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="ca2be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ca2be-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="ca2be-106">Permission type</span></span>      | <span data-ttu-id="ca2be-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ca2be-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ca2be-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ca2be-108">Delegated (work or school account)</span></span> | <span data-ttu-id="ca2be-109">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca2be-109">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="ca2be-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ca2be-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ca2be-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="ca2be-111">Not supported.</span></span>    |
|<span data-ttu-id="ca2be-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="ca2be-112">Application</span></span> | <span data-ttu-id="ca2be-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca2be-113">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ca2be-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ca2be-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groups/{id}/threads/{id}
PATCH /groups/{id}/conversations/{id}/threads/{id}

```
## <a name="request-headers"></a><span data-ttu-id="ca2be-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="ca2be-115">Request headers</span></span>
| <span data-ttu-id="ca2be-116">标头</span><span class="sxs-lookup"><span data-stu-id="ca2be-116">Header</span></span>       | <span data-ttu-id="ca2be-117">值</span><span class="sxs-lookup"><span data-stu-id="ca2be-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ca2be-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="ca2be-118">Authorization</span></span>  | <span data-ttu-id="ca2be-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ca2be-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ca2be-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ca2be-121">Content-Type</span></span>  | <span data-ttu-id="ca2be-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="ca2be-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ca2be-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="ca2be-124">Request body</span></span>
<span data-ttu-id="ca2be-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="ca2be-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="ca2be-128">属性</span><span class="sxs-lookup"><span data-stu-id="ca2be-128">Property</span></span>     | <span data-ttu-id="ca2be-129">类型</span><span class="sxs-lookup"><span data-stu-id="ca2be-129">Type</span></span>   |<span data-ttu-id="ca2be-130">说明</span><span class="sxs-lookup"><span data-stu-id="ca2be-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ca2be-131">isLocked</span><span class="sxs-lookup"><span data-stu-id="ca2be-131">isLocked</span></span>|<span data-ttu-id="ca2be-132">Boolean</span><span class="sxs-lookup"><span data-stu-id="ca2be-132">Boolean</span></span>|<span data-ttu-id="ca2be-p105">指示线程是否已锁定。设置为 `true` 以禁止发布。</span><span class="sxs-lookup"><span data-stu-id="ca2be-p105">Indicates if the thread is locked. Set to `true` to disallow posting.</span></span>|

## <a name="response"></a><span data-ttu-id="ca2be-135">响应</span><span class="sxs-lookup"><span data-stu-id="ca2be-135">Response</span></span>

<span data-ttu-id="ca2be-136">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [conversationThread](../resources/conversationthread.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ca2be-136">If successful, this method returns a `200 OK` response code and updated [conversationThread](../resources/conversationthread.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ca2be-137">示例</span><span class="sxs-lookup"><span data-stu-id="ca2be-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ca2be-138">请求</span><span class="sxs-lookup"><span data-stu-id="ca2be-138">Request</span></span>
<span data-ttu-id="ca2be-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ca2be-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_conversationthread"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}
Content-type: application/json
Content-length: 419

{
  "@odata.type":"#Microsoft.OutlookServices.ConversationThread",
  "isLocked": true
}
```
##### <a name="response"></a><span data-ttu-id="ca2be-140">响应</span><span class="sxs-lookup"><span data-stu-id="ca2be-140">Response</span></span>
<span data-ttu-id="ca2be-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ca2be-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationThread"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 419

{
  "toRecipients": [
    {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    }
  ],
  "topic": "topic-value",
  "hasAttachments": true,
  "lastDeliveredDateTime": "datetime-value",
  "uniqueSenders": [
    "uniqueSenders-value"
  ],
  "ccRecipients": [
    {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    }
  ],
  "isLocked": true 
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update conversationthread",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
