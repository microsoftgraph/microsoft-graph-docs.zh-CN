# <a name="grouplifecyclepolicy-removegroup"></a><span data-ttu-id="99eba-101">groupLifecyclePolicy: removeGroup</span><span class="sxs-lookup"><span data-stu-id="99eba-101">groupLifecyclePolicy: removeGroup</span></span>

<span data-ttu-id="99eba-102">从生命周期策略中删除组。</span><span class="sxs-lookup"><span data-stu-id="99eba-102">Removes a group from a web.</span></span>

## <a name="permissions"></a><span data-ttu-id="99eba-103">权限</span><span class="sxs-lookup"><span data-stu-id="99eba-103">Permissions</span></span>

<span data-ttu-id="99eba-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="99eba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="99eba-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="99eba-106">Permission type</span></span>      | <span data-ttu-id="99eba-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="99eba-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="99eba-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="99eba-108">Delegated (work or school account)</span></span> | <span data-ttu-id="99eba-109">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99eba-109">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="99eba-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="99eba-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="99eba-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="99eba-111">Not supported.</span></span>    |
|<span data-ttu-id="99eba-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="99eba-112">Application</span></span> | <span data-ttu-id="99eba-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99eba-113">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="99eba-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="99eba-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies/{id}/removeGroup
```

## <a name="request-headers"></a><span data-ttu-id="99eba-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="99eba-115">Request headers</span></span>

| <span data-ttu-id="99eba-116">名称</span><span class="sxs-lookup"><span data-stu-id="99eba-116">Name</span></span> | <span data-ttu-id="99eba-117">说明</span><span class="sxs-lookup"><span data-stu-id="99eba-117">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="99eba-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="99eba-118">Authorization</span></span> | <span data-ttu-id="99eba-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="99eba-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="99eba-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="99eba-121">Content-Type</span></span>  | <span data-ttu-id="99eba-122">application/json</span><span class="sxs-lookup"><span data-stu-id="99eba-122">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="99eba-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="99eba-123">Request body</span></span>
<span data-ttu-id="99eba-124">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="99eba-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="99eba-125">参数</span><span class="sxs-lookup"><span data-stu-id="99eba-125">Parameter</span></span> | <span data-ttu-id="99eba-126">类型</span><span class="sxs-lookup"><span data-stu-id="99eba-126">Type</span></span> | <span data-ttu-id="99eba-127">说明</span><span class="sxs-lookup"><span data-stu-id="99eba-127">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="99eba-128">groupId</span><span class="sxs-lookup"><span data-stu-id="99eba-128">groupId</span></span>|<span data-ttu-id="99eba-129">Guid</span><span class="sxs-lookup"><span data-stu-id="99eba-129">Guid</span></span>| <span data-ttu-id="99eba-130">要从策略中删除的组的 ID。</span><span class="sxs-lookup"><span data-stu-id="99eba-130">The id of the group to remove from the policy.</span></span>|

## <a name="response"></a><span data-ttu-id="99eba-131">响应</span><span class="sxs-lookup"><span data-stu-id="99eba-131">Response</span></span>

<span data-ttu-id="99eba-132">如果成功，此方法返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="99eba-132">If successful, this method returns `200 OK` response code.</span></span> <span data-ttu-id="99eba-133">如果已从策略中删除组，响应正文中返回 **true** 值。</span><span class="sxs-lookup"><span data-stu-id="99eba-133">If the group is removed from the policy, a **true** value is returned in the response body.</span></span> <span data-ttu-id="99eba-134">否则，响应正文中返回 **false** 值。</span><span class="sxs-lookup"><span data-stu-id="99eba-134">Otherwise, a **false** value is returned in the reponse body.</span></span>

## <a name="example"></a><span data-ttu-id="99eba-135">示例</span><span class="sxs-lookup"><span data-stu-id="99eba-135">Example</span></span>

##### <a name="request"></a><span data-ttu-id="99eba-136">请求</span><span class="sxs-lookup"><span data-stu-id="99eba-136">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "grouplifecyclepolicy_removegroup"
} -->
```http
POST https://graph.microsoft.com/v1.0/groupLifecyclePolicies/{id}/removeGroup
Content-type: application/json
Content-length: 57

{
  "groupId": "ffffffff-ffff-ffff-ffff-ffffffffffff"
}
```

##### <a name="response"></a><span data-ttu-id="99eba-137">响应</span><span class="sxs-lookup"><span data-stu-id="99eba-137">Response</span></span>
<!-- { "blockType": "ignored" } -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 21

{
  "value": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "groupLifecyclePolicy: removegroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->