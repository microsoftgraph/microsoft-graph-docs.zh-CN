# <a name="tablecolumncollection-add"></a><span data-ttu-id="cb516-101">TableColumnCollection: add</span><span class="sxs-lookup"><span data-stu-id="cb516-101">TableColumnCollection: add</span></span>

<span data-ttu-id="cb516-102">向表中添加新列。</span><span class="sxs-lookup"><span data-stu-id="cb516-102">Adds a new column to the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="cb516-103">权限</span><span class="sxs-lookup"><span data-stu-id="cb516-103">Permissions</span></span>
<span data-ttu-id="cb516-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="cb516-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="cb516-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="cb516-106">Permission type</span></span>      | <span data-ttu-id="cb516-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cb516-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cb516-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cb516-108">Delegated (work or school account)</span></span> | <span data-ttu-id="cb516-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cb516-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="cb516-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cb516-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cb516-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="cb516-111">Not supported.</span></span>    |
|<span data-ttu-id="cb516-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="cb516-112">Application</span></span> | <span data-ttu-id="cb516-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="cb516-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cb516-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cb516-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/add
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/add

```
## <a name="request-headers"></a><span data-ttu-id="cb516-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="cb516-115">Request headers</span></span>
| <span data-ttu-id="cb516-116">名称</span><span class="sxs-lookup"><span data-stu-id="cb516-116">Name</span></span>       | <span data-ttu-id="cb516-117">说明</span><span class="sxs-lookup"><span data-stu-id="cb516-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="cb516-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="cb516-118">Authorization</span></span>  | <span data-ttu-id="cb516-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cb516-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cb516-121">请求正文</span><span class="sxs-lookup"><span data-stu-id="cb516-121">Request body</span></span>
<span data-ttu-id="cb516-122">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="cb516-122">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="cb516-123">参数</span><span class="sxs-lookup"><span data-stu-id="cb516-123">Parameter</span></span>    | <span data-ttu-id="cb516-124">类型</span><span class="sxs-lookup"><span data-stu-id="cb516-124">Type</span></span>   |<span data-ttu-id="cb516-125">说明</span><span class="sxs-lookup"><span data-stu-id="cb516-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cb516-126">index</span><span class="sxs-lookup"><span data-stu-id="cb516-126">index</span></span>|<span data-ttu-id="cb516-127">number</span><span class="sxs-lookup"><span data-stu-id="cb516-127">number</span></span>|<span data-ttu-id="cb516-p103">指定新列的相对位置。之前位于此位置的列向右移动。索引值应等于或小于最后一列的索引值，因此不能用于在表末尾附加列。从零开始编制索引。</span><span class="sxs-lookup"><span data-stu-id="cb516-p103">Specifies the relative position of the new column. The previous column at this position is shifted to the right. The index value should be equal to or less than the last column's index value, so it cannot be used to append a column at the end of the table. Zero-indexed.</span></span>|
|<span data-ttu-id="cb516-132">values</span><span class="sxs-lookup"><span data-stu-id="cb516-132">values</span></span>|<span data-ttu-id="cb516-133">（布尔值、字符串或数字）</span><span class="sxs-lookup"><span data-stu-id="cb516-133">(boolean or string or number)</span></span>|<span data-ttu-id="cb516-p104">可选。未设置格式的表列值的二维数组。</span><span class="sxs-lookup"><span data-stu-id="cb516-p104">Optional. A 2-dimensional array of unformatted values of the table column.</span></span>|

## <a name="response"></a><span data-ttu-id="cb516-136">响应</span><span class="sxs-lookup"><span data-stu-id="cb516-136">Response</span></span>

<span data-ttu-id="cb516-137">如果成功，此方法在响应正文中返回 `200, OK` 响应代码和 [TableColumn](../resources/tablecolumn.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cb516-137">If successful, this method returns `200, OK` response code and [TableColumn](../resources/tablecolumn.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cb516-138">示例</span><span class="sxs-lookup"><span data-stu-id="cb516-138">Example</span></span>
<span data-ttu-id="cb516-139">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="cb516-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="cb516-140">请求</span><span class="sxs-lookup"><span data-stu-id="cb516-140">Request</span></span>
<span data-ttu-id="cb516-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cb516-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablecolumncollection_add"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns/add
Content-type: application/json
Content-length: 51

{
  "index": {
  },
  "values": [
    {
    }
  ]
}
```

##### <a name="response"></a><span data-ttu-id="cb516-142">响应</span><span class="sxs-lookup"><span data-stu-id="cb516-142">Response</span></span>
<span data-ttu-id="cb516-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cb516-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tableColumn"
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
  "tocPath": ""
}-->