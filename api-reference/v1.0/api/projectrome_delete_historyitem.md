# <a name="delete-a-historyitem"></a><span data-ttu-id="98d06-101">删除 historyItem</span><span class="sxs-lookup"><span data-stu-id="98d06-101">Delete a historyItem</span></span>

<span data-ttu-id="98d06-102">删除现有用户活动的现有历史记录项。</span><span class="sxs-lookup"><span data-stu-id="98d06-102">Delete an existing history item for an existing user activity.</span></span>

## <a name="permissions"></a><span data-ttu-id="98d06-103">权限</span><span class="sxs-lookup"><span data-stu-id="98d06-103">Permissions</span></span>

<span data-ttu-id="98d06-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="98d06-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="98d06-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="98d06-106">Permission type</span></span>      | <span data-ttu-id="98d06-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="98d06-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="98d06-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="98d06-108">Delegated (work or school account)</span></span> | <span data-ttu-id="98d06-109">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="98d06-109">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="98d06-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="98d06-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="98d06-111">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="98d06-111">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="98d06-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="98d06-112">Application</span></span> | <span data-ttu-id="98d06-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="98d06-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="98d06-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="98d06-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/activities/{id}/historyItems/{id}
```

## <a name="request-headers"></a><span data-ttu-id="98d06-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="98d06-115">Request headers</span></span>

|<span data-ttu-id="98d06-116">名称</span><span class="sxs-lookup"><span data-stu-id="98d06-116">Name</span></span> | <span data-ttu-id="98d06-117">类型</span><span class="sxs-lookup"><span data-stu-id="98d06-117">Type</span></span> | <span data-ttu-id="98d06-118">说明</span><span class="sxs-lookup"><span data-stu-id="98d06-118">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="98d06-119">授权</span><span class="sxs-lookup"><span data-stu-id="98d06-119">Authorization</span></span> | <span data-ttu-id="98d06-120">字符串</span><span class="sxs-lookup"><span data-stu-id="98d06-120">string</span></span> | <span data-ttu-id="98d06-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="98d06-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="98d06-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="98d06-123">Request body</span></span>

<span data-ttu-id="98d06-124">无请求正文。</span><span class="sxs-lookup"><span data-stu-id="98d06-124">No request body is required.</span></span>

## <a name="response"></a><span data-ttu-id="98d06-125">响应</span><span class="sxs-lookup"><span data-stu-id="98d06-125">Response</span></span>

<span data-ttu-id="98d06-126">如果成功，此方法返回 `204 No Content` 如果历史记录项已删除的响应代码。</span><span class="sxs-lookup"><span data-stu-id="98d06-126">If successful, this method returns the `204 No Content` response code if the history item was deleted.</span></span>

## <a name="example"></a><span data-ttu-id="98d06-127">示例</span><span class="sxs-lookup"><span data-stu-id="98d06-127">Example</span></span>

##### <a name="request"></a><span data-ttu-id="98d06-128">请求</span><span class="sxs-lookup"><span data-stu-id="98d06-128">Request</span></span>

<span data-ttu-id="98d06-129">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="98d06-129">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_historyItem"
}-->

```http
PUT https://graph.microsoft.com/v1.0/me/activities/{activity-id}/historyItems/{item-id}
```

##### <a name="response"></a><span data-ttu-id="98d06-130">响应</span><span class="sxs-lookup"><span data-stu-id="98d06-130">Response</span></span>

<span data-ttu-id="98d06-131">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="98d06-131">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete historyitem",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->