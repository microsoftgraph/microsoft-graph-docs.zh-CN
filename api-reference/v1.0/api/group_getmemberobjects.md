# <a name="group-getmemberobjects"></a><span data-ttu-id="504ad-101">group: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="504ad-101">group: getMemberObjects</span></span>
<span data-ttu-id="504ad-p101">返回此组所属的全部组。检查是可传递的。注意：组不能是目录角色的成员，因此不会返回任何目录角色。</span><span class="sxs-lookup"><span data-stu-id="504ad-p101">Return all of the groups that this group is a member of. The check is transitive. Note: Groups cannot be members of directory roles, so no directory roles will be returned.</span></span>

## <a name="permissions"></a><span data-ttu-id="504ad-105">权限</span><span class="sxs-lookup"><span data-stu-id="504ad-105">Permissions</span></span>
<span data-ttu-id="504ad-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="504ad-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="504ad-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="504ad-108">Permission type</span></span>      | <span data-ttu-id="504ad-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="504ad-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="504ad-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="504ad-110">Delegated (work or school account)</span></span> | <span data-ttu-id="504ad-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="504ad-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="504ad-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="504ad-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="504ad-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="504ad-113">Not supported.</span></span>    |
|<span data-ttu-id="504ad-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="504ad-114">Application</span></span> | <span data-ttu-id="504ad-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="504ad-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="504ad-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="504ad-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/getMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="504ad-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="504ad-117">Request headers</span></span>
| <span data-ttu-id="504ad-118">名称</span><span class="sxs-lookup"><span data-stu-id="504ad-118">Name</span></span>       | <span data-ttu-id="504ad-119">类型</span><span class="sxs-lookup"><span data-stu-id="504ad-119">Type</span></span> | <span data-ttu-id="504ad-120">说明</span><span class="sxs-lookup"><span data-stu-id="504ad-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="504ad-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="504ad-121">Authorization</span></span>  | <span data-ttu-id="504ad-122">string</span><span class="sxs-lookup"><span data-stu-id="504ad-122">string</span></span>  | <span data-ttu-id="504ad-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="504ad-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="504ad-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="504ad-125">Request body</span></span>
<span data-ttu-id="504ad-126">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="504ad-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="504ad-127">参数</span><span class="sxs-lookup"><span data-stu-id="504ad-127">Parameter</span></span>    | <span data-ttu-id="504ad-128">类型</span><span class="sxs-lookup"><span data-stu-id="504ad-128">Type</span></span>   |<span data-ttu-id="504ad-129">说明</span><span class="sxs-lookup"><span data-stu-id="504ad-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="504ad-130">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="504ad-130">securityEnabledOnly</span></span>|<span data-ttu-id="504ad-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="504ad-131">Boolean</span></span>| <span data-ttu-id="504ad-p104">设置为 **false**。只支持对用户仅返回启用安全机制的组。</span><span class="sxs-lookup"><span data-stu-id="504ad-p104">Set to **false**. Returning only security-enabled groups is supported for users only.</span></span>|

## <a name="response"></a><span data-ttu-id="504ad-134">响应</span><span class="sxs-lookup"><span data-stu-id="504ad-134">Response</span></span>
<span data-ttu-id="504ad-135">如果成功，此方法将在包含该组所属组 ID 的响应正文中返回 `200 OK` 响应代码和字符串集合。</span><span class="sxs-lookup"><span data-stu-id="504ad-135">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups that the group is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="504ad-136">示例</span><span class="sxs-lookup"><span data-stu-id="504ad-136">Example</span></span>
#### <a name="request"></a><span data-ttu-id="504ad-137">请求</span><span class="sxs-lookup"><span data-stu-id="504ad-137">Request</span></span>
<span data-ttu-id="504ad-138">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="504ad-138">The following is an example of the request body.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/getMemberObjects
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": false
}
```

#### <a name="response"></a><span data-ttu-id="504ad-139">响应</span><span class="sxs-lookup"><span data-stu-id="504ad-139">Response</span></span>
<span data-ttu-id="504ad-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="504ad-140">Here is an example of the response.</span></span>
><span data-ttu-id="504ad-141">**注意：**为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="504ad-141">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="504ad-142">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="504ad-142">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 39

{
  "value": [
    "string-value"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: getMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
