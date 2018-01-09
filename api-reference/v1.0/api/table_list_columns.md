# <a name="list-columns"></a><span data-ttu-id="82421-101">列出列</span><span class="sxs-lookup"><span data-stu-id="82421-101">List columns</span></span>

<span data-ttu-id="82421-102">检索 tablecolumn 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="82421-102">Retrieve a list of tablecolumn objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="82421-103">权限</span><span class="sxs-lookup"><span data-stu-id="82421-103">Permissions</span></span>
<span data-ttu-id="82421-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="82421-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="82421-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="82421-106">Permission type</span></span>      | <span data-ttu-id="82421-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="82421-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="82421-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="82421-108">Delegated (work or school account)</span></span> | <span data-ttu-id="82421-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="82421-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="82421-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="82421-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="82421-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="82421-111">Not supported.</span></span>    |
|<span data-ttu-id="82421-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="82421-112">Application</span></span> | <span data-ttu-id="82421-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="82421-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="82421-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="82421-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}/columns
GET /workbook/worksheets/{id|name}/tables/{id|name}/columns
```
## <a name="optional-query-parameters"></a><span data-ttu-id="82421-115">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="82421-115">Optional query parameters</span></span>
<span data-ttu-id="82421-116">此方法支持使用 [OData 查询参数]((http://developer.microsoft.com/zh-CN/graph/docs/overview/query_parameters)) 自定义响应。</span><span class="sxs-lookup"><span data-stu-id="82421-116">This method supports the [OData Query Parameters]((http://developer.microsoft.com/zh-CN/graph/docs/overview/query_parameters)) to help customize the response.</span></span>  <span data-ttu-id="82421-117">为了获得可靠结果，请使用 [$top](https://developer.microsoft.com/en-us/graph/docs/concepts/query_parameters#top) 和 [$skip](https://developer.microsoft.com/en-us/graph/docs/concepts/query_parameters#skip-parameter) 查询参数逐个浏览结果。</span><span class="sxs-lookup"><span data-stu-id="82421-117">For reliable results, use the [$top](https://developer.microsoft.com/en-us/graph/docs/concepts/query_parameters#top) and [$skip](https://developer.microsoft.com/en-us/graph/docs/concepts/query_parameters#skip-parameter) query parameters to page through the results.</span></span> <span data-ttu-id="82421-118">这有助于避免较大的结果集带来的性能问题。</span><span class="sxs-lookup"><span data-stu-id="82421-118">This will help avoid performance problems related to large result sets.</span></span>

## <a name="request-headers"></a><span data-ttu-id="82421-119">请求头</span><span class="sxs-lookup"><span data-stu-id="82421-119">Request headers</span></span>
| <span data-ttu-id="82421-120">名称</span><span class="sxs-lookup"><span data-stu-id="82421-120">Name</span></span>      |<span data-ttu-id="82421-121">说明</span><span class="sxs-lookup"><span data-stu-id="82421-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="82421-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="82421-122">Authorization</span></span>  | <span data-ttu-id="82421-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="82421-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="82421-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="82421-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="82421-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="82421-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="82421-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="82421-128">Request body</span></span>
<span data-ttu-id="82421-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="82421-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="82421-130">响应</span><span class="sxs-lookup"><span data-stu-id="82421-130">Response</span></span>

<span data-ttu-id="82421-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [TableColumn](../resources/tablecolumn.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="82421-131">If successful, this method returns a `200 OK` response code and collection of [TableColumn](../resources/tablecolumn.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="82421-132">示例</span><span class="sxs-lookup"><span data-stu-id="82421-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="82421-133">请求</span><span class="sxs-lookup"><span data-stu-id="82421-133">Request</span></span>
<span data-ttu-id="82421-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="82421-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_columns"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns?$top=5&$skip=5
```
##### <a name="response"></a><span data-ttu-id="82421-135">响应</span><span class="sxs-lookup"><span data-stu-id="82421-135">Response</span></span>
<span data-ttu-id="82421-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="82421-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tableColumn",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 126

{
  "value": [
    {
      "id": 99,
      "name": "name-value",
      "index": 99,
      "values": "values-value"
    }
  ]
}
```

> <span data-ttu-id="82421-139">
  **注意：**使用 [$top](https://developer.microsoft.com/en-us/graph/docs/concepts/query_parameters#top) 和 [$skip](https://developer.microsoft.com/en-us/graph/docs/concepts/query_parameters#skip-parameter) 查询参数可逐个浏览许多列。</span><span class="sxs-lookup"><span data-stu-id="82421-139">**Note:** Use the [$top](https://developer.microsoft.com/en-us/graph/docs/concepts/query_parameters#top) and [$skip](https://developer.microsoft.com/en-us/graph/docs/concepts/query_parameters#skip-parameter) query parameters to page through large numbers of columns.</span></span>

<span data-ttu-id="82421-140">示例：</span><span class="sxs-lookup"><span data-stu-id="82421-140">Example:</span></span> 

`https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns?$top=5`
`https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns?$top=5&$skip=5`

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List columns",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->