# <a name="check-member-groups"></a><span data-ttu-id="3808c-101">检查成员组</span><span class="sxs-lookup"><span data-stu-id="3808c-101">Check member groups</span></span>

<span data-ttu-id="3808c-p101">检查特定组列表中的成员资格，并从该列表返回成员为指定的 user、group 或 directory 对象的组。此函数是可传递的。</span><span class="sxs-lookup"><span data-stu-id="3808c-p101">Check for membership in a specified list of groups, and returns from that list those groups of which the specified user, group, or directory object is a member. This function is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="3808c-104">权限</span><span class="sxs-lookup"><span data-stu-id="3808c-104">Permissions</span></span>
<span data-ttu-id="3808c-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="3808c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="3808c-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="3808c-107">Permission type</span></span>      | <span data-ttu-id="3808c-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3808c-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3808c-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3808c-109">Delegated (work or school account)</span></span> | <span data-ttu-id="3808c-110">User.Read.All 和 Group.Read.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="3808c-110">User.Read.All and Group.Read.All, Directory.Read.All</span></span>    |
|<span data-ttu-id="3808c-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3808c-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3808c-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="3808c-112">Not supported.</span></span>    |
|<span data-ttu-id="3808c-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="3808c-113">Application</span></span> | <span data-ttu-id="3808c-114">User.Read.All 和 Group.Read.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="3808c-114">User.Read.All and Group.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3808c-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3808c-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/checkMemberGroups
POST /users/{id | userPrincipalName}/checkMemberGroups
POST /groups/{id}/checkMemberGroups
POST /directoryObjects/{id}/checkMemberGroups
```
## <a name="request-headers"></a><span data-ttu-id="3808c-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="3808c-116">Request headers</span></span>
| <span data-ttu-id="3808c-117">名称</span><span class="sxs-lookup"><span data-stu-id="3808c-117">Name</span></span>       | <span data-ttu-id="3808c-118">类型</span><span class="sxs-lookup"><span data-stu-id="3808c-118">Type</span></span> | <span data-ttu-id="3808c-119">说明</span><span class="sxs-lookup"><span data-stu-id="3808c-119">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="3808c-120">授权</span><span class="sxs-lookup"><span data-stu-id="3808c-120">Authorization</span></span>  | <span data-ttu-id="3808c-121">字符串</span><span class="sxs-lookup"><span data-stu-id="3808c-121">string</span></span>  | <span data-ttu-id="3808c-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3808c-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3808c-124">内容类型</span><span class="sxs-lookup"><span data-stu-id="3808c-124">Content-Type</span></span>  | <span data-ttu-id="3808c-125">字符串</span><span class="sxs-lookup"><span data-stu-id="3808c-125">string</span></span> | <span data-ttu-id="3808c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3808c-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3808c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="3808c-127">Request body</span></span>
<span data-ttu-id="3808c-128">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="3808c-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="3808c-129">参数</span><span class="sxs-lookup"><span data-stu-id="3808c-129">Parameter</span></span>    | <span data-ttu-id="3808c-130">类型</span><span class="sxs-lookup"><span data-stu-id="3808c-130">Type</span></span>   |<span data-ttu-id="3808c-131">说明</span><span class="sxs-lookup"><span data-stu-id="3808c-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3808c-132">groupIds</span><span class="sxs-lookup"><span data-stu-id="3808c-132">groupIds</span></span>|<span data-ttu-id="3808c-133">字符串集合</span><span class="sxs-lookup"><span data-stu-id="3808c-133">String collection</span></span>|<span data-ttu-id="3808c-p104">包含检查成员身份的组中的对象 ID 的集合。可以指定多达 20 个组。</span><span class="sxs-lookup"><span data-stu-id="3808c-p104">A collection that contains the object IDs of the groups in which to check membership. Up to 20 groups may be specified.</span></span>|

## <a name="response"></a><span data-ttu-id="3808c-136">响应</span><span class="sxs-lookup"><span data-stu-id="3808c-136">Response</span></span>

<span data-ttu-id="3808c-137">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 String 集合对象。</span><span class="sxs-lookup"><span data-stu-id="3808c-137">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3808c-138">示例</span><span class="sxs-lookup"><span data-stu-id="3808c-138">Example</span></span>

##### <a name="request"></a><span data-ttu-id="3808c-139">请求</span><span class="sxs-lookup"><span data-stu-id="3808c-139">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "directoryobject_checkmembergroups"
}-->
```http
POST https://graph.microsoft.com/v1.0/directoryObjects/{id}/checkMemberGroups
Content-type: application/json

{
  "groupIds": [
        "fee2c45b-915a-4a64b130f4eb9e75525e",
        "4fe90ae065a-478b9400e0a0e1cbd540"
  ]
}
```

##### <a name="response"></a><span data-ttu-id="3808c-140">响应</span><span class="sxs-lookup"><span data-stu-id="3808c-140">Response</span></span>
<span data-ttu-id="3808c-p105">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3808c-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
        "fee2c45b-915a-4a64-b130-f4eb9e75525e"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
