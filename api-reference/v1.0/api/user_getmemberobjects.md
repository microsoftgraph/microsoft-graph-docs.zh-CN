# <a name="user-getmemberobjects"></a><span data-ttu-id="90566-101">user: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="90566-101">user: getMemberObjects</span></span>
<span data-ttu-id="90566-p101">返回用户所属的所有组、目录角色和管理单元。检查是可传递的。</span><span class="sxs-lookup"><span data-stu-id="90566-p101">Return all of the groups, directory roles and administrative units that the user is a member of. The check is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="90566-104">权限</span><span class="sxs-lookup"><span data-stu-id="90566-104">Permissions</span></span>
<span data-ttu-id="90566-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="90566-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="90566-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="90566-107">Permission type</span></span>      | <span data-ttu-id="90566-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="90566-108">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="90566-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="90566-109">Delegated (work or school account)</span></span> | <span data-ttu-id="90566-110">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="90566-110">One of the following scopes is required to execute this API: Directory.Read.All; Directory.ReadWrite.All; Directory.AccessAsUser.All</span></span>    | 
|<span data-ttu-id="90566-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="90566-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="90566-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="90566-112">Not supported.</span></span>    | 
|<span data-ttu-id="90566-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="90566-113">Application</span></span> | <span data-ttu-id="90566-114">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90566-114">Directory.Read.All, Directory.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="90566-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="90566-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/getMemberObjects
```
## <a name="request-headers"></a><span data-ttu-id="90566-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="90566-116">Request headers</span></span>
| <span data-ttu-id="90566-117">标头</span><span class="sxs-lookup"><span data-stu-id="90566-117">Header</span></span>       | <span data-ttu-id="90566-118">值</span><span class="sxs-lookup"><span data-stu-id="90566-118">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="90566-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="90566-119">Authorization</span></span>  | <span data-ttu-id="90566-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="90566-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="90566-122">Content-Type</span><span class="sxs-lookup"><span data-stu-id="90566-122">Content-Type</span></span>  | <span data-ttu-id="90566-123">application/json</span><span class="sxs-lookup"><span data-stu-id="90566-123">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="90566-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="90566-124">Request body</span></span>
<span data-ttu-id="90566-125">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="90566-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="90566-126">参数</span><span class="sxs-lookup"><span data-stu-id="90566-126">Parameter</span></span>    | <span data-ttu-id="90566-127">类型</span><span class="sxs-lookup"><span data-stu-id="90566-127">Type</span></span>   |<span data-ttu-id="90566-128">说明</span><span class="sxs-lookup"><span data-stu-id="90566-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="90566-129">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="90566-129">securityEnabledOnly</span></span>|<span data-ttu-id="90566-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="90566-130">Boolean</span></span>|<span data-ttu-id="90566-p104">**true** 指定仅应返回用户所属的安全组；**false** 指定应返回用户所属的所有组和目录角色。注意：仅当对用户调用这个方法时，才支持将此参数设置为 **true**。</span><span class="sxs-lookup"><span data-stu-id="90566-p104">**true** to specify that only security groups that the user is a member of should be returned; **false** to specify that all groups and directory roles that the user is a member of should be returned. Note: Setting this parameter to **true** is only supported when calling this method on a user.</span></span>|

## <a name="response"></a><span data-ttu-id="90566-133">响应</span><span class="sxs-lookup"><span data-stu-id="90566-133">Response</span></span>

<span data-ttu-id="90566-134">如果成功，此方法将在包含该用户所属组和目录角色 ID 的响应正文中返回 `200, OK` 响应代码和 String 集合。</span><span class="sxs-lookup"><span data-stu-id="90566-134">If successful, this method returns `200, OK` response code and String collection in the response body that contains the IDs of the groups and directory roles that the user is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="90566-135">示例</span><span class="sxs-lookup"><span data-stu-id="90566-135">Example</span></span>
<span data-ttu-id="90566-136">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="90566-136">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="90566-137">请求</span><span class="sxs-lookup"><span data-stu-id="90566-137">Request</span></span>
<span data-ttu-id="90566-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="90566-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/getMemberObjects
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": true
}
```

##### <a name="response"></a><span data-ttu-id="90566-139">响应</span><span class="sxs-lookup"><span data-stu-id="90566-139">Response</span></span>
<span data-ttu-id="90566-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="90566-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "user: getMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
