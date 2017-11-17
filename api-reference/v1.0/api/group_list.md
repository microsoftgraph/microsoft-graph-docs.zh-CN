# <a name="list-groups"></a><span data-ttu-id="5da03-101">列出组</span><span class="sxs-lookup"><span data-stu-id="5da03-101">List groups</span></span>

<span data-ttu-id="5da03-p101">列出组织中所有可用的组，包括但不限于 Office 365 组。返回每个组的[默认属性](../api/group_get.md#default-properties)。</span><span class="sxs-lookup"><span data-stu-id="5da03-p101">List all the groups available in an organization, including but not limited to Office 365 Groups. The [default properties](../api/group_get.md#default-properties) of each group are returned.</span></span>

<span data-ttu-id="5da03-104">若要仅列出 Office 365 组（亦称为“统一组”），请对 **groupTypes** 应用筛选器：</span><span class="sxs-lookup"><span data-stu-id="5da03-104">To list only Office 365 Groups (aka unified groups), apply a filter on **groupTypes**:</span></span>
```
GET https://graph.microsoft.com/v1.0/groups?$filter=groupTypes/any(c:c+eq+'Unified')
```

<span data-ttu-id="5da03-105">可以使用 OData 查询选项 `$orderby`，按 **displayName** 值对组织中的组进行排序，如下面的示例所示：</span><span class="sxs-lookup"><span data-stu-id="5da03-105">You can use the OData query option `$orderby` to sort groups in an organization by the **displayName** values, as shown in the following example:</span></span>
```
GET https://graph.microsoft.com/v1.0/groups?$orderby=displayName
```


## <a name="permissions"></a><span data-ttu-id="5da03-106">权限</span><span class="sxs-lookup"><span data-stu-id="5da03-106">Permissions</span></span>
<span data-ttu-id="5da03-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="5da03-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5da03-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5da03-109">Permission type</span></span>      | <span data-ttu-id="5da03-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5da03-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5da03-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5da03-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5da03-112">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5da03-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="5da03-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5da03-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5da03-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="5da03-114">Not supported.</span></span>    |
|<span data-ttu-id="5da03-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="5da03-115">Application</span></span> | <span data-ttu-id="5da03-116">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5da03-116">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5da03-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5da03-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5da03-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="5da03-118">Optional query parameters</span></span>
<span data-ttu-id="5da03-119">此方法支持 [OData 查询参数](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="5da03-119">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="5da03-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="5da03-120">Request headers</span></span>
| <span data-ttu-id="5da03-121">名称</span><span class="sxs-lookup"><span data-stu-id="5da03-121">Name</span></span>       | <span data-ttu-id="5da03-122">类型</span><span class="sxs-lookup"><span data-stu-id="5da03-122">Type</span></span> | <span data-ttu-id="5da03-123">说明</span><span class="sxs-lookup"><span data-stu-id="5da03-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="5da03-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="5da03-124">Authorization</span></span>  | <span data-ttu-id="5da03-125">string</span><span class="sxs-lookup"><span data-stu-id="5da03-125">string</span></span>  | <span data-ttu-id="5da03-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5da03-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5da03-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="5da03-128">Request body</span></span>
<span data-ttu-id="5da03-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5da03-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5da03-130">响应</span><span class="sxs-lookup"><span data-stu-id="5da03-130">Response</span></span>

<span data-ttu-id="5da03-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [group](../resources/group.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="5da03-131">If successful, this method returns a `200 OK` response code and collection of [group](../resources/group.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5da03-132">示例</span><span class="sxs-lookup"><span data-stu-id="5da03-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5da03-133">请求</span><span class="sxs-lookup"><span data-stu-id="5da03-133">Request</span></span>
<span data-ttu-id="5da03-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5da03-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_groups"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups
```
##### <a name="response"></a><span data-ttu-id="5da03-135">响应</span><span class="sxs-lookup"><span data-stu-id="5da03-135">Response</span></span>
<span data-ttu-id="5da03-136">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="5da03-136">Here is an example of the response.</span></span>

<span data-ttu-id="5da03-p104">注意：为简洁起见，可能会截断此处展示的响应对象。实际调用会返回[默认属性](../api/group_get.md#default-properties)。</span><span class="sxs-lookup"><span data-stu-id="5da03-p104">Note: The response object shown here may be truncated for brevity. The [default properties](../api/group_get.md#default-properties) will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: xxx

 {
  "value": [
    {
      "id": "id-value",
      "description": "description-value",
      "displayName": "displayName-value",
      "groupTypes": [
        "groupTypes-value"
      ],
      "mail": "mail-value",
      "mailEnabled": true,
      "mailNickname": "mailNickname-value",
      "onPremisesLastSyncDateTime": "onPremisesLastSyncDateTime-value",
      "onPremisesSecurityIdentifier": "onPremisesSecurityIdentifier-value",
      "onPremisesSyncEnabled": true,
      "proxyAddresses": [
        "proxyAddresses-value"
      ],
      "securityEnabled": true,
      "visibility": "visibility-value"
    }
  ]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List groups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
