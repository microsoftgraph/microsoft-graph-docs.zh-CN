# <a name="tablerowcollection-add"></a><span data-ttu-id="49ccd-101">TableRowCollection: 添加</span><span class="sxs-lookup"><span data-stu-id="49ccd-101">TableRowCollection: add</span></span>

<span data-ttu-id="49ccd-102">添加行至表末尾。</span><span class="sxs-lookup"><span data-stu-id="49ccd-102">Adds a row to the end of the table.</span></span> <span data-ttu-id="49ccd-103">请注意 API 可以接受使用此 API 的多个行数据。</span><span class="sxs-lookup"><span data-stu-id="49ccd-103">Note that the API can accept multiple rows data using this API.</span></span> <span data-ttu-id="49ccd-104">一次添加一行可能导致性能下降。</span><span class="sxs-lookup"><span data-stu-id="49ccd-104">Adding one row at a time could lead to performance degradation.</span></span> <span data-ttu-id="49ccd-105">推荐方法是在单个调用中执行行批处理操作，而不是执行单个行插入操作。</span><span class="sxs-lookup"><span data-stu-id="49ccd-105">The recommended approach would be to batch the rows together in a single call rather than doing single row insertion.</span></span> <span data-ttu-id="49ccd-106">为了获得最佳结果，收集要插入的应用程序侧的h行，并执行单个行的添加操作。</span><span class="sxs-lookup"><span data-stu-id="49ccd-106">For best results, collect the rows to be inserted on the application side and perform single rows add operation.</span></span> <span data-ttu-id="49ccd-107">试验一定数量的行插入试验，明确在单个 API 调用中理想的行数。</span><span class="sxs-lookup"><span data-stu-id="49ccd-107">Experiment with the number of rows to determine the ideal number of rows to use in single API call.</span></span> 

## <a name="error-handling"></a><span data-ttu-id="49ccd-108">错误处理</span><span class="sxs-lookup"><span data-stu-id="49ccd-108">Error Handling</span></span>

<span data-ttu-id="49ccd-109">此请求有时可能会收到 504 HTTP 错误。</span><span class="sxs-lookup"><span data-stu-id="49ccd-109">This request might occasionally receive a 504 HTTP error.</span></span> <span data-ttu-id="49ccd-110">此错误的适当响应做法是重复发出请求。</span><span class="sxs-lookup"><span data-stu-id="49ccd-110">The appropriate response to this error is to repeat the request.</span></span>

## <a name="permissions"></a><span data-ttu-id="49ccd-111">权限</span><span class="sxs-lookup"><span data-stu-id="49ccd-111">Permissions</span></span>
<span data-ttu-id="49ccd-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="49ccd-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="49ccd-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="49ccd-114">Permission type</span></span>      | <span data-ttu-id="49ccd-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="49ccd-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="49ccd-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="49ccd-116">Delegated (work or school account)</span></span> | <span data-ttu-id="49ccd-117">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="49ccd-117">Files.ReadWrite</span></span>    |
|<span data-ttu-id="49ccd-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="49ccd-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="49ccd-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="49ccd-119">Not supported.</span></span>    |
|<span data-ttu-id="49ccd-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="49ccd-120">Application</span></span> | <span data-ttu-id="49ccd-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="49ccd-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="49ccd-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="49ccd-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/rows/add
POST /workbook/worksheets/{id|name}/tables/{id|name}/rows/add

```
## <a name="request-headers"></a><span data-ttu-id="49ccd-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="49ccd-123">Request headers</span></span>
| <span data-ttu-id="49ccd-124">名称</span><span class="sxs-lookup"><span data-stu-id="49ccd-124">Name</span></span>       | <span data-ttu-id="49ccd-125">说明</span><span class="sxs-lookup"><span data-stu-id="49ccd-125">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="49ccd-126">授权</span><span class="sxs-lookup"><span data-stu-id="49ccd-126">Authorization</span></span>  | <span data-ttu-id="49ccd-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="49ccd-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="49ccd-129">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="49ccd-129">Workbook-Session-Id</span></span>  | <span data-ttu-id="49ccd-p105">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="49ccd-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="49ccd-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="49ccd-132">Request body</span></span>
<span data-ttu-id="49ccd-133">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="49ccd-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="49ccd-134">参数</span><span class="sxs-lookup"><span data-stu-id="49ccd-134">Parameter</span></span>    | <span data-ttu-id="49ccd-135">类型</span><span class="sxs-lookup"><span data-stu-id="49ccd-135">Type</span></span>   |<span data-ttu-id="49ccd-136">说明</span><span class="sxs-lookup"><span data-stu-id="49ccd-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="49ccd-137">索引</span><span class="sxs-lookup"><span data-stu-id="49ccd-137">index</span></span>|<span data-ttu-id="49ccd-138">Int32</span><span class="sxs-lookup"><span data-stu-id="49ccd-138">Int32</span></span>|<span data-ttu-id="49ccd-p106">可选。指定新行的相对位置。如果为空，将在末尾进行添加。插入的行下方的任何行将向下移动。从零开始编制索引。</span><span class="sxs-lookup"><span data-stu-id="49ccd-p106">Optional. Specifies the relative position of the new row. If null, the addition happens at the end. Any rows below the inserted row are shifted downwards. Zero-indexed.</span></span>|
|<span data-ttu-id="49ccd-144">值</span><span class="sxs-lookup"><span data-stu-id="49ccd-144">values</span></span>|<span data-ttu-id="49ccd-145">Json</span><span class="sxs-lookup"><span data-stu-id="49ccd-145">Json</span></span>|<span data-ttu-id="49ccd-p107">可选。未设置格式的表行值的二维数组。</span><span class="sxs-lookup"><span data-stu-id="49ccd-p107">Optional. A 2-dimensional array of unformatted values of the table row.</span></span>|

## <a name="response"></a><span data-ttu-id="49ccd-148">响应</span><span class="sxs-lookup"><span data-stu-id="49ccd-148">Response</span></span>

<span data-ttu-id="49ccd-149">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [WorkbookTableRow](../resources/tablerow.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="49ccd-149">If successful, this method returns `200 OK` response code and [groupSetting](../resources/tablerow.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="49ccd-150">示例</span><span class="sxs-lookup"><span data-stu-id="49ccd-150">Example</span></span>
<span data-ttu-id="49ccd-151">在此示例中表的末尾插入两行数据。</span><span class="sxs-lookup"><span data-stu-id="49ccd-151">In this example two rows of data are inserted at the end of the table.</span></span> 

##### <a name="request"></a><span data-ttu-id="49ccd-152">请求</span><span class="sxs-lookup"><span data-stu-id="49ccd-152">Request</span></span>
<span data-ttu-id="49ccd-153">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="49ccd-153">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablerowcollection_add"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/rows/add
Content-type: application/json
Content-length: 51

{
  "index": 5,
  "values": [
    [1, 2, 3],
    [4, 5, 6]
  ]
}
```

##### <a name="response"></a><span data-ttu-id="49ccd-154">响应</span><span class="sxs-lookup"><span data-stu-id="49ccd-154">Response</span></span>
<span data-ttu-id="49ccd-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="49ccd-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableRow"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 45

{
  "index": 99,
  "values": "values-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableRowCollection: add",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/api/tablerowcollection_add.md/tablerowcollection_add/values:
      Inconsistent types between parameter (Collection) and table (None)",
    "Error: /api-reference/v1.0/api/tablerowcollection_add.md/tablerowcollection_add/values:
      Type mismatch between example and table. Parameter name: values; example type (Collection(Collection)) is a collection, while the table description type (microsoft.graph.Json) is not."
  ],
  "tocPath": ""
}-->
