# <a name="list-schemaextensions"></a><span data-ttu-id="417ca-101">列出 schemaExtensions</span><span class="sxs-lookup"><span data-stu-id="417ca-101">List schemaExtensions</span></span>

<span data-ttu-id="417ca-102">获取你在当前租户中所拥有的任何应用创建的 [schemaExtension](../resources/schemaextension.md) 对象（可以是 **InDevelopment**、**Available**、或 **Deprecated** 状态）及其他应用拥有的标记为 **Available** 的所有其他架构扩展的列表。</span><span class="sxs-lookup"><span data-stu-id="417ca-102">Get a list of [schemaExtension](../resources/schemaextension.md) objects created by any apps you own in the current tenant (that can be **InDevelopment**, **Available**, or **Deprecated**), and all other schema extensions owned by other apps that are marked as **Available**.</span></span> 

## <a name="permissions"></a><span data-ttu-id="417ca-103">权限</span><span class="sxs-lookup"><span data-stu-id="417ca-103">Permissions</span></span>
<span data-ttu-id="417ca-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="417ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="417ca-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="417ca-106">Permission type</span></span>      | <span data-ttu-id="417ca-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="417ca-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="417ca-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="417ca-108">Delegated (work or school account)</span></span> | <span data-ttu-id="417ca-109">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="417ca-109">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="417ca-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="417ca-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="417ca-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="417ca-111">Not supported.</span></span>    |
|<span data-ttu-id="417ca-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="417ca-112">Application</span></span> | <span data-ttu-id="417ca-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="417ca-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="417ca-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="417ca-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /schemaExtensions
```
## <a name="optional-query-parameters"></a><span data-ttu-id="417ca-115">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="417ca-115">Optional query parameters</span></span>
<span data-ttu-id="417ca-116">此方法支持 [OData 查询参数](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="417ca-116">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="417ca-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="417ca-117">Request headers</span></span>
| <span data-ttu-id="417ca-118">名称</span><span class="sxs-lookup"><span data-stu-id="417ca-118">Name</span></span>      |<span data-ttu-id="417ca-119">说明</span><span class="sxs-lookup"><span data-stu-id="417ca-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="417ca-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="417ca-120">Authorization</span></span>  | <span data-ttu-id="417ca-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="417ca-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="417ca-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="417ca-123">Content-Type</span></span>   | <span data-ttu-id="417ca-124">application/json</span><span class="sxs-lookup"><span data-stu-id="417ca-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="417ca-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="417ca-125">Request body</span></span>
<span data-ttu-id="417ca-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="417ca-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="417ca-127">响应</span><span class="sxs-lookup"><span data-stu-id="417ca-127">Response</span></span>

<span data-ttu-id="417ca-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [schemaExtension](../resources/schemaextension.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="417ca-128">If successful, this method returns a `200 OK` response code and collection of [schemaExtension](../resources/schemaextension.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="417ca-129">示例</span><span class="sxs-lookup"><span data-stu-id="417ca-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="417ca-130">请求</span><span class="sxs-lookup"><span data-stu-id="417ca-130">Request</span></span>
<span data-ttu-id="417ca-131">以下示例演示了如何通过筛选扩展的唯一 **ID** 在所有可访问的扩展中查找特定的扩展。</span><span class="sxs-lookup"><span data-stu-id="417ca-131">The following example shows how to look among all the accessible extensions for a specific one by filtering on its unique **id**.</span></span> 
<!-- {
  "blockType": "request",
  "name": "get_schemaextensions"
}-->
```http
GET https://graph.microsoft.com/v1.0/schemaExtensions?$filter=id%20eq%20'graphlearn_test'
```
##### <a name="response"></a><span data-ttu-id="417ca-132">响应</span><span class="sxs-lookup"><span data-stu-id="417ca-132">Response</span></span>
<span data-ttu-id="417ca-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="417ca-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schemaExtension",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 274

{
  "value": [
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
  ]
}
```

## <a name="see-also"></a><span data-ttu-id="417ca-136">另请参阅</span><span class="sxs-lookup"><span data-stu-id="417ca-136">See also</span></span>

- [<span data-ttu-id="417ca-137">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="417ca-137">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="417ca-138">使用架构扩展向组添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="417ca-138">Add custom data to groups using schema extensions</span></span>](../../../concepts/extensibility_schema_groups.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List schemaExtensions",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->