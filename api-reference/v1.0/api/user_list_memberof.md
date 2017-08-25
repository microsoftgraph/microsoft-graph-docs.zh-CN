# <a name="list-memberof"></a><span data-ttu-id="36b5e-101">列出 memberOf</span><span class="sxs-lookup"><span data-stu-id="36b5e-101">List memberOf</span></span>

<span data-ttu-id="36b5e-102">获取用户是其直接成员的[组](../resources/group.md)和[目录角色](../resources/directoryrole.md)。</span><span class="sxs-lookup"><span data-stu-id="36b5e-102">Get [groups](../resources/group.md) and [directory roles](../resources/directoryrole.md) that the user is a direct member of.</span></span> 

## <a name="permissions"></a><span data-ttu-id="36b5e-103">权限</span><span class="sxs-lookup"><span data-stu-id="36b5e-103">Permissions</span></span>
<span data-ttu-id="36b5e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="36b5e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="36b5e-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="36b5e-106">Permission type</span></span>      | <span data-ttu-id="36b5e-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="36b5e-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="36b5e-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="36b5e-108">Delegated (work or school account)</span></span> | <span data-ttu-id="36b5e-109">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="36b5e-109">One of the following scopes is required to execute this API: Directory.Read.All; Directory.ReadWrite.All; Directory.AccessAsUser.All</span></span>    | 
|<span data-ttu-id="36b5e-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="36b5e-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="36b5e-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="36b5e-111">Not supported.</span></span>    | 
|<span data-ttu-id="36b5e-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="36b5e-112">Application</span></span> | <span data-ttu-id="36b5e-113">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36b5e-113">Directory.Read.All, Directory.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="36b5e-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="36b5e-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/memberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="36b5e-115">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="36b5e-115">Optional query parameters</span></span>
<span data-ttu-id="36b5e-p102">此方法支持 [OData 查询参数](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)来帮助自定义响应。$filter 不受支持。</span><span class="sxs-lookup"><span data-stu-id="36b5e-p102">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response. $filter is not supported.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="36b5e-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="36b5e-118">Request headers</span></span>
| <span data-ttu-id="36b5e-119">标头</span><span class="sxs-lookup"><span data-stu-id="36b5e-119">Header</span></span>       | <span data-ttu-id="36b5e-120">值</span><span class="sxs-lookup"><span data-stu-id="36b5e-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="36b5e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="36b5e-121">Authorization</span></span>  | <span data-ttu-id="36b5e-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="36b5e-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="36b5e-124">接受</span><span class="sxs-lookup"><span data-stu-id="36b5e-124">Accept</span></span>  | <span data-ttu-id="36b5e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="36b5e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="36b5e-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="36b5e-126">Request body</span></span>
<span data-ttu-id="36b5e-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="36b5e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="36b5e-128">响应</span><span class="sxs-lookup"><span data-stu-id="36b5e-128">Response</span></span>

<span data-ttu-id="36b5e-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="36b5e-129">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="36b5e-130">示例</span><span class="sxs-lookup"><span data-stu-id="36b5e-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="36b5e-131">请求</span><span class="sxs-lookup"><span data-stu-id="36b5e-131">Request</span></span>
<span data-ttu-id="36b5e-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="36b5e-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_memberof"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/memberOf
```
##### <a name="response"></a><span data-ttu-id="36b5e-133">响应</span><span class="sxs-lookup"><span data-stu-id="36b5e-133">Response</span></span>
<span data-ttu-id="36b5e-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="36b5e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "id-value",
      "createdDateTime": null,
      "description": "All users at the company",
      "displayName": "All Users",
      "groupTypes": [],
      "mailEnabled": false,
      "securityEnabled": true,
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
