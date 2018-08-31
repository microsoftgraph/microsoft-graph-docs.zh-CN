# <a name="create-or-replace-a-historyitem"></a><span data-ttu-id="c5d40-101">创建或替换 historyItem</span><span class="sxs-lookup"><span data-stu-id="c5d40-101">Create or replace a history item</span></span>

<span data-ttu-id="c5d40-102">为现有用户活动创建新或替换现有的历史记录项。</span><span class="sxs-lookup"><span data-stu-id="c5d40-102">Create a new or replace an existing history item for an existing user activity.</span></span>

## <a name="permissions"></a><span data-ttu-id="c5d40-103">权限</span><span class="sxs-lookup"><span data-stu-id="c5d40-103">Permissions</span></span>

<span data-ttu-id="c5d40-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="c5d40-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="c5d40-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="c5d40-106">Permission type</span></span>      | <span data-ttu-id="c5d40-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c5d40-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c5d40-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c5d40-108">Delegated (work or school account)</span></span> | <span data-ttu-id="c5d40-109">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="c5d40-109">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="c5d40-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c5d40-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c5d40-111">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="c5d40-111">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="c5d40-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="c5d40-112">Application</span></span> | <span data-ttu-id="c5d40-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="c5d40-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c5d40-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c5d40-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /me/activities/{id}/historyItems/{id}
```

<span data-ttu-id="c5d40-115">Id 需要是 GUID。</span><span class="sxs-lookup"><span data-stu-id="c5d40-115">Id needs to be a GUID.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c5d40-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="c5d40-116">Request headers</span></span>

|<span data-ttu-id="c5d40-117">名称</span><span class="sxs-lookup"><span data-stu-id="c5d40-117">Name</span></span> | <span data-ttu-id="c5d40-118">类型</span><span class="sxs-lookup"><span data-stu-id="c5d40-118">Type</span></span> | <span data-ttu-id="c5d40-119">说明</span><span class="sxs-lookup"><span data-stu-id="c5d40-119">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="c5d40-120">授权</span><span class="sxs-lookup"><span data-stu-id="c5d40-120">Authorization</span></span> | <span data-ttu-id="c5d40-121">字符串</span><span class="sxs-lookup"><span data-stu-id="c5d40-121">string</span></span> | <span data-ttu-id="c5d40-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c5d40-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c5d40-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="c5d40-124">Request body</span></span>

<span data-ttu-id="c5d40-125">在请求正文中，提供 [historyItem](../resources/projectrome_historyitem.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c5d40-125">In the request body, supply a JSON representation of [directoryObject](../resources/projectrome_historyitem.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="c5d40-126">响应</span><span class="sxs-lookup"><span data-stu-id="c5d40-126">Response</span></span>

<span data-ttu-id="c5d40-127">如果成功，此方法将在创建了 historyItem 或替换 historyItem 的情况下，返回 `201 Created` 响应代码`200 OK`。</span><span class="sxs-lookup"><span data-stu-id="c5d40-127">If successful, this method returns the `201 Created` response code if the historyItem was created or `200 OK` if the historyItem was replaced.</span></span>

## <a name="example"></a><span data-ttu-id="c5d40-128">示例</span><span class="sxs-lookup"><span data-stu-id="c5d40-128">Example</span></span>

#### <a name="request"></a><span data-ttu-id="c5d40-129">请求</span><span class="sxs-lookup"><span data-stu-id="c5d40-129">Request</span></span>

<span data-ttu-id="c5d40-130">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c5d40-130">Here is an example of the request.</span></span>

<!-- {
    "blockType": "ignored",
    "name": "upsert_historyItem"
} -->

```http
PUT https://graph.microsoft.com/v1.0/me/activities/{activity-id}/historyItems/{item-id}
Content-type: application/json
Content-length: 364

{
    "startedDateTime": "2015-02-11T20:54:04.3457274+00:00",
    "userTimezone": "Africa/Casablanca",
    "lastActiveDateTime": "2015-02-11T20:54:04.3457274+00:00"
}
```

#### <a name="response"></a><span data-ttu-id="c5d40-131">响应</span><span class="sxs-lookup"><span data-stu-id="c5d40-131">Response</span></span>

<span data-ttu-id="c5d40-132">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="c5d40-132">Here is an example of the response.</span></span>

<!-- {
    "blockType": "ignored",
    "truncated": true,
    "@odata.type": "microsoft.graph.activityHistoryItem"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('user%40contoso.com')/activities('13881113971988980728')/historyItems/$entity",
    "status": "updated",
    "userTimezone": "Africa/Casablanca",
    "createdDateTime": "2018-02-26T20:28:22.14Z",
    "lastModifiedDateTime": "2018-02-26T20:28:22.155Z",
    "id": "9d0b74e4-4b41-43ea-b34d-f9c1bf9f809c",
    "startedDateTime": "2018-02-26T20:54:04.345Z",
    "lastActiveDateTime": "2018-02-26T20:54:24.345Z",
    "expirationDateTime": "2018-03-28T20:28:22.14Z",
    "activeDurationSeconds": 20
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Upsert historyitem",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->