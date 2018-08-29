# <a name="get-member-groups"></a><span data-ttu-id="a54bb-101">获取成员组</span><span class="sxs-lookup"><span data-stu-id="a54bb-101">Get member groups</span></span>

<span data-ttu-id="a54bb-p101">返回指定的 user、group 或 directory 对象所属的所有组。此函数是可传递的。</span><span class="sxs-lookup"><span data-stu-id="a54bb-p101">Return all the groups that the specified user, group, or directory object is a member of. This function is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="a54bb-104">权限</span><span class="sxs-lookup"><span data-stu-id="a54bb-104">Permissions</span></span>
<span data-ttu-id="a54bb-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="a54bb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a54bb-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="a54bb-107">Permission type</span></span>      | <span data-ttu-id="a54bb-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a54bb-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a54bb-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a54bb-109">Delegated (work or school account)</span></span> | <span data-ttu-id="a54bb-110">User.Read.All 和 Group.Read.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="a54bb-110">User.Read.All and Group.Read.All, Directory.Read.All</span></span>    |
|<span data-ttu-id="a54bb-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a54bb-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a54bb-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="a54bb-112">Not supported.</span></span>    |
|<span data-ttu-id="a54bb-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="a54bb-113">Application</span></span> | <span data-ttu-id="a54bb-114">User.Read.All 和 Group.Read.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="a54bb-114">User.Read.All and Group.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a54bb-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a54bb-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/getMemberGroups
POST /users/{id | userPrincipalName}/getMemberGroups
POST /groups/{id}/getMemberGroups
POST /directoryObjects/{id}/getMemberGroups
```
## <a name="request-headers"></a><span data-ttu-id="a54bb-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="a54bb-116">Request headers</span></span>
| <span data-ttu-id="a54bb-117">名称</span><span class="sxs-lookup"><span data-stu-id="a54bb-117">Name</span></span>       | <span data-ttu-id="a54bb-118">类型</span><span class="sxs-lookup"><span data-stu-id="a54bb-118">Type</span></span> | <span data-ttu-id="a54bb-119">说明</span><span class="sxs-lookup"><span data-stu-id="a54bb-119">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a54bb-120">授权</span><span class="sxs-lookup"><span data-stu-id="a54bb-120">Authorization</span></span>  | <span data-ttu-id="a54bb-121">字符串</span><span class="sxs-lookup"><span data-stu-id="a54bb-121">string</span></span>  | <span data-ttu-id="a54bb-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a54bb-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a54bb-124">内容类型</span><span class="sxs-lookup"><span data-stu-id="a54bb-124">Content-Type</span></span>   | <span data-ttu-id="a54bb-125">string</span><span class="sxs-lookup"><span data-stu-id="a54bb-125">string</span></span>  | <span data-ttu-id="a54bb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a54bb-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a54bb-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a54bb-127">Request body</span></span>
<span data-ttu-id="a54bb-128">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="a54bb-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a54bb-129">参数</span><span class="sxs-lookup"><span data-stu-id="a54bb-129">Parameter</span></span>    | <span data-ttu-id="a54bb-130">类型</span><span class="sxs-lookup"><span data-stu-id="a54bb-130">Type</span></span>   |<span data-ttu-id="a54bb-131">说明</span><span class="sxs-lookup"><span data-stu-id="a54bb-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a54bb-132">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="a54bb-132">securityEnabledOnly</span></span>|<span data-ttu-id="a54bb-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="a54bb-133">Boolean</span></span>| <span data-ttu-id="a54bb-p104">**true** 指定仅应返回包含实体的安全组；**false** 指定应返回包含实体的所有组和目录角色。**注意**：如果参数为 **true**，只能对一位用户调用此函数。</span><span class="sxs-lookup"><span data-stu-id="a54bb-p104">**true** to specify that only security groups that the entity is a member of should be returned; **false** to specify that all groups and directory roles that the entity is a member of should be returned. **Note**: The function can only be called on a user if the parameter is **true**.</span></span> |

## <a name="response"></a><span data-ttu-id="a54bb-136">响应</span><span class="sxs-lookup"><span data-stu-id="a54bb-136">Response</span></span>

<span data-ttu-id="a54bb-137">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 String 集合对象。</span><span class="sxs-lookup"><span data-stu-id="a54bb-137">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a54bb-138">示例</span><span class="sxs-lookup"><span data-stu-id="a54bb-138">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a54bb-139">请求</span><span class="sxs-lookup"><span data-stu-id="a54bb-139">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "directoryobject_getmembergroups"
}-->
```http
POST https://graph.microsoft.com/v1.0/directoryObjects/{object-id}/getMemberGroups
Content-type: application/json

{
  "securityEnabledOnly": true
}
```

##### <a name="response"></a><span data-ttu-id="a54bb-140">响应</span><span class="sxs-lookup"><span data-stu-id="a54bb-140">Response</span></span>
<span data-ttu-id="a54bb-p105">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a54bb-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(Edm.String)",
    "value": [
        "fee2c45b-915a-4a64-b130-f4eb9e75525e",
        "4fe90ae7-065a-478b-9400-e0a0e1cbd540",
        "e0c3beaf-eeb4-43d8-abc5-94f037a65697"
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject: getMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
