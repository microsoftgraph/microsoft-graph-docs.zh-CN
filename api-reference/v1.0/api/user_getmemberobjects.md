# <a name="user-getmemberobjects"></a><span data-ttu-id="a13fa-101">user: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="a13fa-101">user: getMemberObjects</span></span>
<span data-ttu-id="a13fa-p101">返回用户所属的所有组、目录角色和管理单元。检查是可传递的。</span><span class="sxs-lookup"><span data-stu-id="a13fa-p101">Return all of the groups, directory roles and administrative units that the user is a member of. The check is transitive.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a13fa-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="a13fa-104">Prerequisites</span></span>
<span data-ttu-id="a13fa-105">若要执行此 API，必须有以下**范围**之一：*Directory.Read.All；Directory.ReadWrite.All；Directory.AccessAsUser.All*</span><span class="sxs-lookup"><span data-stu-id="a13fa-105">One of the following **scopes** is required to execute this API: *Directory.Read.All; Directory.ReadWrite.All; Directory.AccessAsUser.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="a13fa-106">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a13fa-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/getMemberObjects
```
## <a name="request-headers"></a><span data-ttu-id="a13fa-107">请求标头</span><span class="sxs-lookup"><span data-stu-id="a13fa-107">Request headers</span></span>
| <span data-ttu-id="a13fa-108">标头</span><span class="sxs-lookup"><span data-stu-id="a13fa-108">Header</span></span>       | <span data-ttu-id="a13fa-109">值</span><span class="sxs-lookup"><span data-stu-id="a13fa-109">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a13fa-110">Authorization</span><span class="sxs-lookup"><span data-stu-id="a13fa-110">Authorization</span></span>  | <span data-ttu-id="a13fa-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a13fa-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a13fa-113">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a13fa-113">Content-Type</span></span>  | <span data-ttu-id="a13fa-114">application/json</span><span class="sxs-lookup"><span data-stu-id="a13fa-114">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a13fa-115">请求正文</span><span class="sxs-lookup"><span data-stu-id="a13fa-115">Request body</span></span>
<span data-ttu-id="a13fa-116">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="a13fa-116">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a13fa-117">参数</span><span class="sxs-lookup"><span data-stu-id="a13fa-117">Parameter</span></span>    | <span data-ttu-id="a13fa-118">类型</span><span class="sxs-lookup"><span data-stu-id="a13fa-118">Type</span></span>   |<span data-ttu-id="a13fa-119">说明</span><span class="sxs-lookup"><span data-stu-id="a13fa-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a13fa-120">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="a13fa-120">securityEnabledOnly</span></span>|<span data-ttu-id="a13fa-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="a13fa-121">Boolean</span></span>|<span data-ttu-id="a13fa-p103">**true** 指定仅应返回用户所属的安全组；**false** 指定应返回用户所属的所有组和目录角色。注意：仅当对用户调用这个方法时，才支持将此参数设置为 **true**。</span><span class="sxs-lookup"><span data-stu-id="a13fa-p103">**true** to specify that only security groups that the user is a member of should be returned; **false** to specify that all groups and directory roles that the user is a member of should be returned. Note: Setting this parameter to **true** is only supported when calling this method on a user.</span></span>|

## <a name="response"></a><span data-ttu-id="a13fa-124">响应</span><span class="sxs-lookup"><span data-stu-id="a13fa-124">Response</span></span>

<span data-ttu-id="a13fa-125">如果成功，此方法将在包含该用户所属组和目录角色 ID 的响应正文中返回 `200, OK` 响应代码和 String 集合。</span><span class="sxs-lookup"><span data-stu-id="a13fa-125">If successful, this method returns `200, OK` response code and String collection in the response body that contains the IDs of the groups and directory roles that the user is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="a13fa-126">示例</span><span class="sxs-lookup"><span data-stu-id="a13fa-126">Example</span></span>
<span data-ttu-id="a13fa-127">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="a13fa-127">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="a13fa-128">请求</span><span class="sxs-lookup"><span data-stu-id="a13fa-128">Request</span></span>
<span data-ttu-id="a13fa-129">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a13fa-129">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="a13fa-130">响应</span><span class="sxs-lookup"><span data-stu-id="a13fa-130">Response</span></span>
<span data-ttu-id="a13fa-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a13fa-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
