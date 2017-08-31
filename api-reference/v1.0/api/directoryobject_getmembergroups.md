# <a name="get-member-groups"></a><span data-ttu-id="7488c-101">获取成员组</span><span class="sxs-lookup"><span data-stu-id="7488c-101">Get member groups</span></span>

<span data-ttu-id="7488c-p101">返回指定的 user、group 或 directory 对象所属的所有组。此函数是可传递的。</span><span class="sxs-lookup"><span data-stu-id="7488c-p101">Return all the groups that the specified user, group, or directory object is a member of. This function is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="7488c-104">权限</span><span class="sxs-lookup"><span data-stu-id="7488c-104">Permissions</span></span>
<span data-ttu-id="7488c-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="7488c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="7488c-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="7488c-107">Permission type</span></span>      | <span data-ttu-id="7488c-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7488c-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7488c-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7488c-109">Delegated (work or school account)</span></span> | <span data-ttu-id="7488c-110">User.Read.All 和 Group.Read.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="7488c-110">User.ReadBasic.All and Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="7488c-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7488c-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7488c-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="7488c-112">Not supported.</span></span>    |
|<span data-ttu-id="7488c-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="7488c-113">Application</span></span> | <span data-ttu-id="7488c-114">User.Read.All 和 Group.Read.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="7488c-114">User.ReadBasic.All and Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7488c-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7488c-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/getMemberGroups
POST /users/{id | userPrincipalName}/getMemberGroups
POST /groups/{id}/getMemberGroups
POST /directoryObjects/{id}/getMemberGroups
```
## <a name="request-headers"></a><span data-ttu-id="7488c-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="7488c-116">Request headers</span></span>
| <span data-ttu-id="7488c-117">名称</span><span class="sxs-lookup"><span data-stu-id="7488c-117">Name</span></span>       | <span data-ttu-id="7488c-118">类型</span><span class="sxs-lookup"><span data-stu-id="7488c-118">Type</span></span> | <span data-ttu-id="7488c-119">说明</span><span class="sxs-lookup"><span data-stu-id="7488c-119">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7488c-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="7488c-120">Authorization</span></span>  | <span data-ttu-id="7488c-121">string</span><span class="sxs-lookup"><span data-stu-id="7488c-121">string</span></span>  | <span data-ttu-id="7488c-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7488c-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7488c-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7488c-124">Content-Type</span></span>  | <span data-ttu-id="7488c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7488c-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7488c-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="7488c-126">Request body</span></span>
<span data-ttu-id="7488c-127">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="7488c-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="7488c-128">参数</span><span class="sxs-lookup"><span data-stu-id="7488c-128">Parameter</span></span>    | <span data-ttu-id="7488c-129">类型</span><span class="sxs-lookup"><span data-stu-id="7488c-129">Type</span></span>   |<span data-ttu-id="7488c-130">说明</span><span class="sxs-lookup"><span data-stu-id="7488c-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7488c-131">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="7488c-131">securityEnabledOnly</span></span>|<span data-ttu-id="7488c-132">Boolean</span><span class="sxs-lookup"><span data-stu-id="7488c-132">Boolean</span></span>| <span data-ttu-id="7488c-p104">**true** 指定仅应返回包含实体的安全组；**false** 指定应返回包含实体的所有组和目录角色。**注意**：如果参数为 **true**，只能对一位用户调用此函数。</span><span class="sxs-lookup"><span data-stu-id="7488c-p104">**true** to specify that only security groups that the entity is a member of should be returned; **false** to specify that all groups and directory roles that the entity is a member of should be returned. **Note**: The function can only be called on a user if the parameter is **true**.</span></span> |

## <a name="response"></a><span data-ttu-id="7488c-135">响应</span><span class="sxs-lookup"><span data-stu-id="7488c-135">Response</span></span>

<span data-ttu-id="7488c-136">如果成功，此方法在响应正文中返回 `200, OK` 响应代码和 String 集合对象。</span><span class="sxs-lookup"><span data-stu-id="7488c-136">If successful, this method returns `200, OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7488c-137">示例</span><span class="sxs-lookup"><span data-stu-id="7488c-137">Example</span></span>

##### <a name="request"></a><span data-ttu-id="7488c-138">请求</span><span class="sxs-lookup"><span data-stu-id="7488c-138">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "directoryobject_getmembergroups"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/getMemberGroups
Content-type: application/json

{
  "securityEnabledOnly": true
}
```

##### <a name="response"></a><span data-ttu-id="7488c-139">响应</span><span class="sxs-lookup"><span data-stu-id="7488c-139">Response</span></span>
<span data-ttu-id="7488c-p105">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7488c-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
