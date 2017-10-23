# <a name="get-member-objects"></a><span data-ttu-id="2c9c9-101">获取成员对象</span><span class="sxs-lookup"><span data-stu-id="2c9c9-101">Get member objects</span></span>

 <span data-ttu-id="2c9c9-p101">返回 user、group 或 directory 对象所属的所有组和目录角色。此函数是可传递的。</span><span class="sxs-lookup"><span data-stu-id="2c9c9-p101">Returns all the groups and directory roles that a user, group, or directory object is a member of. This function is transitive.</span></span> 
 > <span data-ttu-id="2c9c9-104">注意：只有用户可以是目录角色的成员。</span><span class="sxs-lookup"><span data-stu-id="2c9c9-104">Note: Only users can be members of directory roles.</span></span>

## <a name="permissions"></a><span data-ttu-id="2c9c9-105">权限</span><span class="sxs-lookup"><span data-stu-id="2c9c9-105">Permissions</span></span>
<span data-ttu-id="2c9c9-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="2c9c9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2c9c9-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="2c9c9-108">Permission type</span></span>      | <span data-ttu-id="2c9c9-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2c9c9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2c9c9-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2c9c9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2c9c9-111">User.Read.All 和 Group.Read.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="2c9c9-111">User.Read.All and Group.Read.All, Directory.Read.All</span></span>    |
|<span data-ttu-id="2c9c9-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2c9c9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2c9c9-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="2c9c9-113">Not supported.</span></span>    |
|<span data-ttu-id="2c9c9-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="2c9c9-114">Application</span></span> | <span data-ttu-id="2c9c9-115">User.Read.All 和 Group.Read.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="2c9c9-115">User.Read.All and Group.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2c9c9-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2c9c9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/getMemberObjects
POST /users/{id | userPrincipalName}/getMemberObjects
POST /groups/{id}/getMemberGroups
POST /directoryObjects/{id}/getMemberObjects

```
## <a name="request-headers"></a><span data-ttu-id="2c9c9-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="2c9c9-117">Request headers</span></span>
| <span data-ttu-id="2c9c9-118">名称</span><span class="sxs-lookup"><span data-stu-id="2c9c9-118">Name</span></span>       | <span data-ttu-id="2c9c9-119">类型</span><span class="sxs-lookup"><span data-stu-id="2c9c9-119">Type</span></span> | <span data-ttu-id="2c9c9-120">说明</span><span class="sxs-lookup"><span data-stu-id="2c9c9-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2c9c9-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2c9c9-121">Authorization</span></span>  | <span data-ttu-id="2c9c9-122">string</span><span class="sxs-lookup"><span data-stu-id="2c9c9-122">string</span></span>  | <span data-ttu-id="2c9c9-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2c9c9-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2c9c9-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2c9c9-125">Content-Type</span></span>  | <span data-ttu-id="2c9c9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2c9c9-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2c9c9-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="2c9c9-127">Request body</span></span>
<span data-ttu-id="2c9c9-128">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="2c9c9-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2c9c9-129">参数</span><span class="sxs-lookup"><span data-stu-id="2c9c9-129">Parameter</span></span>    | <span data-ttu-id="2c9c9-130">类型</span><span class="sxs-lookup"><span data-stu-id="2c9c9-130">Type</span></span>   |<span data-ttu-id="2c9c9-131">说明</span><span class="sxs-lookup"><span data-stu-id="2c9c9-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2c9c9-132">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="2c9c9-132">securityEnabledOnly</span></span>|<span data-ttu-id="2c9c9-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c9c9-133">Boolean</span></span>| <span data-ttu-id="2c9c9-p104">**true** 指定仅应返回包含实体的安全组；**false** 指定应返回包含实体的所有组和目录角色。**注意**：如果参数为 **true**，只能对一位用户调用此函数。</span><span class="sxs-lookup"><span data-stu-id="2c9c9-p104">**true** to specify that only security groups that the entity is a member of should be returned; **false** to specify that all groups and directory roles that the entity is a member of should be returned. **Note**: The function can only be called on a user if the parameter is **true**.</span></span> |

## <a name="response"></a><span data-ttu-id="2c9c9-136">响应</span><span class="sxs-lookup"><span data-stu-id="2c9c9-136">Response</span></span>

<span data-ttu-id="2c9c9-137">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 String 集合对象。</span><span class="sxs-lookup"><span data-stu-id="2c9c9-137">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2c9c9-138">示例</span><span class="sxs-lookup"><span data-stu-id="2c9c9-138">Example</span></span>

##### <a name="request"></a><span data-ttu-id="2c9c9-139">请求</span><span class="sxs-lookup"><span data-stu-id="2c9c9-139">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "directoryobject_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/getMemberObjects
Content-type: application/json

{
  "securityEnabledOnly": true
}
```

##### <a name="response"></a><span data-ttu-id="2c9c9-140">响应</span><span class="sxs-lookup"><span data-stu-id="2c9c9-140">Response</span></span>
<span data-ttu-id="2c9c9-p105">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2c9c9-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
        "c9ee2d50-9e8a-4352-b97c-4c2c99557c22",
        "e0c3beaf-eeb4-43d8-abc5-94f037a65697"
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject: getMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
