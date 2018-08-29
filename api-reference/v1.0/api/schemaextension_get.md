# <a name="get-schemaextension"></a><span data-ttu-id="c4f0e-101">获取 schemaExtension</span><span class="sxs-lookup"><span data-stu-id="c4f0e-101">Get schemaExtension</span></span>
<span data-ttu-id="c4f0e-102">获取指定的 [schemaExtension](../resources/schemaextension.md) 定义的属性。</span><span class="sxs-lookup"><span data-stu-id="c4f0e-102">Get the properties of the specified [schemaExtension](../resources/schemaextension.md) definition.</span></span>

## <a name="permissions"></a><span data-ttu-id="c4f0e-103">权限</span><span class="sxs-lookup"><span data-stu-id="c4f0e-103">Permissions</span></span>
<span data-ttu-id="c4f0e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="c4f0e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="c4f0e-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="c4f0e-106">Permission type</span></span>      | <span data-ttu-id="c4f0e-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c4f0e-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c4f0e-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c4f0e-108">Delegated (work or school account)</span></span> | <span data-ttu-id="c4f0e-109">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c4f0e-109">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c4f0e-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c4f0e-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c4f0e-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="c4f0e-111">Not supported.</span></span>    |
|<span data-ttu-id="c4f0e-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="c4f0e-112">Application</span></span> | <span data-ttu-id="c4f0e-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="c4f0e-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c4f0e-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c4f0e-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /schemaExtensions/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c4f0e-115">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c4f0e-115">Optional query parameters</span></span>
<span data-ttu-id="c4f0e-116">此方法支持 [OData 查询参数](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c4f0e-116">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c4f0e-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="c4f0e-117">Request headers</span></span>
| <span data-ttu-id="c4f0e-118">名称</span><span class="sxs-lookup"><span data-stu-id="c4f0e-118">Name</span></span>      |<span data-ttu-id="c4f0e-119">说明</span><span class="sxs-lookup"><span data-stu-id="c4f0e-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c4f0e-120">授权</span><span class="sxs-lookup"><span data-stu-id="c4f0e-120">Authorization</span></span>  | <span data-ttu-id="c4f0e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c4f0e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c4f0e-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c4f0e-123">Content-Type</span></span>   | <span data-ttu-id="c4f0e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="c4f0e-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="c4f0e-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="c4f0e-125">Request body</span></span>
<span data-ttu-id="c4f0e-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c4f0e-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c4f0e-127">响应</span><span class="sxs-lookup"><span data-stu-id="c4f0e-127">Response</span></span>

<span data-ttu-id="c4f0e-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [schemaExtension](../resources/schemaextension.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c4f0e-128">If successful, this method returns a `200 OK` response code and [schemaExtension](../resources/schemaextension.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c4f0e-129">示例</span><span class="sxs-lookup"><span data-stu-id="c4f0e-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c4f0e-130">请求</span><span class="sxs-lookup"><span data-stu-id="c4f0e-130">Request</span></span>
<span data-ttu-id="c4f0e-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c4f0e-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_schemaextension"
}-->
```http
GET https://graph.microsoft.com/v1.0/schemaExtensions/graphlearn_test
```
##### <a name="response"></a><span data-ttu-id="c4f0e-132">响应</span><span class="sxs-lookup"><span data-stu-id="c4f0e-132">Response</span></span>
<span data-ttu-id="c4f0e-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c4f0e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.schemaExtension"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
    "id":"graphlearn_test",
    "description": "Yet another test schema",
    "targetTypes": [
        "User", "Group"
    ],
    "status": "InDevelopment",
    "owner": "24d3b144-21ae-4080-943f-7067b395b913",
    "properties": [
        {
            "name": "testName",
            "type": "String"
        }
    ]
}
```

## <a name="see-also"></a><span data-ttu-id="c4f0e-136">另请参阅</span><span class="sxs-lookup"><span data-stu-id="c4f0e-136">See also</span></span>

- [<span data-ttu-id="c4f0e-137">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="c4f0e-137">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="c4f0e-138">使用架构扩展向组添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="c4f0e-138">Add custom data to groups using schema extensions</span></span>](../../../concepts/extensibility_schema_groups.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get schemaExtension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->