# <a name="tablecolumncollection-add"></a><span data-ttu-id="3a2cd-101">TableColumnCollection: add</span><span class="sxs-lookup"><span data-stu-id="3a2cd-101">TableColumnCollection: add</span></span>

<span data-ttu-id="3a2cd-102">向表中添加新列。</span><span class="sxs-lookup"><span data-stu-id="3a2cd-102">Adds a new column to the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="3a2cd-103">权限</span><span class="sxs-lookup"><span data-stu-id="3a2cd-103">Permissions</span></span>
<span data-ttu-id="3a2cd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="3a2cd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="3a2cd-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="3a2cd-106">Permission type</span></span>      | <span data-ttu-id="3a2cd-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3a2cd-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3a2cd-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3a2cd-108">Delegated (work or school account)</span></span> | <span data-ttu-id="3a2cd-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3a2cd-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3a2cd-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3a2cd-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3a2cd-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="3a2cd-111">Not supported.</span></span>    |
|<span data-ttu-id="3a2cd-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="3a2cd-112">Application</span></span> | <span data-ttu-id="3a2cd-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="3a2cd-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3a2cd-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3a2cd-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/add
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/add

```
## <a name="request-headers"></a><span data-ttu-id="3a2cd-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="3a2cd-115">Request headers</span></span>
| <span data-ttu-id="3a2cd-116">名称</span><span class="sxs-lookup"><span data-stu-id="3a2cd-116">Name</span></span>       | <span data-ttu-id="3a2cd-117">说明</span><span class="sxs-lookup"><span data-stu-id="3a2cd-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3a2cd-118">授权</span><span class="sxs-lookup"><span data-stu-id="3a2cd-118">Authorization</span></span>  | <span data-ttu-id="3a2cd-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3a2cd-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3a2cd-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="3a2cd-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="3a2cd-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="3a2cd-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3a2cd-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="3a2cd-124">Request body</span></span>
<span data-ttu-id="3a2cd-125">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="3a2cd-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="3a2cd-126">参数</span><span class="sxs-lookup"><span data-stu-id="3a2cd-126">Parameter</span></span>    | <span data-ttu-id="3a2cd-127">类型</span><span class="sxs-lookup"><span data-stu-id="3a2cd-127">Type</span></span>   |<span data-ttu-id="3a2cd-128">说明</span><span class="sxs-lookup"><span data-stu-id="3a2cd-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3a2cd-129">index</span><span class="sxs-lookup"><span data-stu-id="3a2cd-129">index</span></span>|<span data-ttu-id="3a2cd-130">Int32</span><span class="sxs-lookup"><span data-stu-id="3a2cd-130">Int32</span></span>|<span data-ttu-id="3a2cd-p104">指定新列的相对位置。之前位于此位置的列向右移动。索引值应等于或小于最后一列的索引值，因此不能用于在表末尾附加列。从零开始编制索引。</span><span class="sxs-lookup"><span data-stu-id="3a2cd-p104">Specifies the relative position of the new column. The previous column at this position is shifted to the right. The index value should be equal to or less than the last column's index value, so it cannot be used to append a column at the end of the table. Zero-indexed.</span></span>|
|<span data-ttu-id="3a2cd-135">values</span><span class="sxs-lookup"><span data-stu-id="3a2cd-135">values</span></span>|<span data-ttu-id="3a2cd-136">Json</span><span class="sxs-lookup"><span data-stu-id="3a2cd-136">Json</span></span>|<span data-ttu-id="3a2cd-p105">可选。未设置格式的表列值的二维数组。</span><span class="sxs-lookup"><span data-stu-id="3a2cd-p105">Optional. A 2-dimensional array of unformatted values of the table column.</span></span>|
|<span data-ttu-id="3a2cd-139">name</span><span class="sxs-lookup"><span data-stu-id="3a2cd-139">name</span></span>|<span data-ttu-id="3a2cd-140">字符串</span><span class="sxs-lookup"><span data-stu-id="3a2cd-140">string</span></span>|<span data-ttu-id="3a2cd-141">name</span><span class="sxs-lookup"><span data-stu-id="3a2cd-141">name</span></span>
## <a name="response"></a><span data-ttu-id="3a2cd-142">响应</span><span class="sxs-lookup"><span data-stu-id="3a2cd-142">Response</span></span>

<span data-ttu-id="3a2cd-143">如果成功，此方法在响应正文中返回  响应代码和 WorkbookTableColumn 对象。`200 OK` [ ](../resources/tablecolumn.md)</span><span class="sxs-lookup"><span data-stu-id="3a2cd-143">If successful, this method returns `200 OK` response code and [groupSetting](../resources/tablecolumn.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3a2cd-144">示例</span><span class="sxs-lookup"><span data-stu-id="3a2cd-144">Example</span></span>
<span data-ttu-id="3a2cd-145">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="3a2cd-145">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="3a2cd-146">请求</span><span class="sxs-lookup"><span data-stu-id="3a2cd-146">Request</span></span>
<span data-ttu-id="3a2cd-147">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3a2cd-147">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablecolumncollection_add"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns/add
Content-type: application/json
Content-length: 51

{
  "index": 3,
  "values": [
    {
    }
  ]
}
```

##### <a name="response"></a><span data-ttu-id="3a2cd-148">响应</span><span class="sxs-lookup"><span data-stu-id="3a2cd-148">Response</span></span>
<span data-ttu-id="3a2cd-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3a2cd-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableColumn"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 81

{
  "id": 99,
  "name": "name-value",
  "index": 99,
  "values": "values-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableColumnCollection: add",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/api/tablecolumncollection_add.md/tablecolumncollection_add/values:
      Inconsistent types between parameter (Object) and table (None)",
    "Error: /api-reference/v1.0/api/tablecolumncollection_add.md/tablecolumncollection_add/values:
      Type mismatch between example and table. Parameter name: values; example type (Collection(Object)) is a collection, while the table description type (microsoft.graph.Json) is not."
  ],
  "tocPath": ""
}-->