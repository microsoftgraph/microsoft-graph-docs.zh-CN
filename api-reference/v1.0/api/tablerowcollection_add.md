# <a name="tablerowcollection-add"></a><span data-ttu-id="53397-101">TableRowCollection: add</span><span class="sxs-lookup"><span data-stu-id="53397-101">TableRowCollection: add</span></span>

<span data-ttu-id="53397-102">向表中添加新行。</span><span class="sxs-lookup"><span data-stu-id="53397-102">Adds a new row to the table.</span></span>

## <a name="error-handling"></a><span data-ttu-id="53397-103">错误处理</span><span class="sxs-lookup"><span data-stu-id="53397-103">Error Handling</span></span>

<span data-ttu-id="53397-104">此请求有时可能会收到 504 HTTP 错误。</span><span class="sxs-lookup"><span data-stu-id="53397-104">This request might occasionally receive a 504 HTTP error.</span></span> <span data-ttu-id="53397-105">此错误的适当响应做法是重复发出请求。</span><span class="sxs-lookup"><span data-stu-id="53397-105">The appropriate response to this error is to repeat the request.</span></span>

## <a name="permissions"></a><span data-ttu-id="53397-106">权限</span><span class="sxs-lookup"><span data-stu-id="53397-106">Permissions</span></span>
<span data-ttu-id="53397-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="53397-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="53397-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="53397-109">Permission type</span></span>      | <span data-ttu-id="53397-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="53397-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="53397-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="53397-111">Delegated (work or school account)</span></span> | <span data-ttu-id="53397-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="53397-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="53397-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="53397-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="53397-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="53397-114">Not supported.</span></span>    |
|<span data-ttu-id="53397-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="53397-115">Application</span></span> | <span data-ttu-id="53397-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="53397-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="53397-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="53397-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/rows/add
POST /workbook/worksheets/{id|name}/tables/{id|name}/rows/add

```
## <a name="request-headers"></a><span data-ttu-id="53397-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="53397-118">Request headers</span></span>
| <span data-ttu-id="53397-119">名称</span><span class="sxs-lookup"><span data-stu-id="53397-119">Name</span></span>       | <span data-ttu-id="53397-120">说明</span><span class="sxs-lookup"><span data-stu-id="53397-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="53397-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="53397-121">Authorization</span></span>  | <span data-ttu-id="53397-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="53397-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="53397-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="53397-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="53397-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="53397-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="53397-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="53397-127">Request body</span></span>
<span data-ttu-id="53397-128">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="53397-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="53397-129">参数</span><span class="sxs-lookup"><span data-stu-id="53397-129">Parameter</span></span>    | <span data-ttu-id="53397-130">类型</span><span class="sxs-lookup"><span data-stu-id="53397-130">Type</span></span>   |<span data-ttu-id="53397-131">说明</span><span class="sxs-lookup"><span data-stu-id="53397-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="53397-132">index</span><span class="sxs-lookup"><span data-stu-id="53397-132">index</span></span>|<span data-ttu-id="53397-133">number</span><span class="sxs-lookup"><span data-stu-id="53397-133">number</span></span>|<span data-ttu-id="53397-p105">可选。指定新行的相对位置。如果为空，将在末尾进行添加。插入的行下方的任何行将向下移动。从零开始编制索引。</span><span class="sxs-lookup"><span data-stu-id="53397-p105">Optional. Specifies the relative position of the new row. If null, the addition happens at the end. Any rows below the inserted row are shifted downwards. Zero-indexed.</span></span>|
|<span data-ttu-id="53397-139">values</span><span class="sxs-lookup"><span data-stu-id="53397-139">values</span></span>|<span data-ttu-id="53397-140">（布尔值、字符串或数字）</span><span class="sxs-lookup"><span data-stu-id="53397-140">(boolean or string or number)</span></span>|<span data-ttu-id="53397-p106">可选。未设置格式的表行值的二维数组。</span><span class="sxs-lookup"><span data-stu-id="53397-p106">Optional. A 2-dimensional array of unformatted values of the table row.</span></span>|

## <a name="response"></a><span data-ttu-id="53397-143">响应</span><span class="sxs-lookup"><span data-stu-id="53397-143">Response</span></span>

<span data-ttu-id="53397-144">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [TableRow](../resources/tablerow.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="53397-144">If successful, this method returns `200 OK` response code and [TableRow](../resources/tablerow.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53397-145">示例</span><span class="sxs-lookup"><span data-stu-id="53397-145">Example</span></span>
<span data-ttu-id="53397-146">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="53397-146">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="53397-147">请求</span><span class="sxs-lookup"><span data-stu-id="53397-147">Request</span></span>
<span data-ttu-id="53397-148">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="53397-148">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablerowcollection_add"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/rows/add
Content-type: application/json
Content-length: 51

{
  "index": null,
  "values": [
    [1, 2, 3],
    [4, 5, 6]
  ]
}
```

##### <a name="response"></a><span data-ttu-id="53397-149">响应</span><span class="sxs-lookup"><span data-stu-id="53397-149">Response</span></span>
<span data-ttu-id="53397-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="53397-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tableRow"
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
  "tocPath": ""
}-->
