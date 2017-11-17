# <a name="tablerowcollection-add"></a><span data-ttu-id="2e8c4-101">TableRowCollection: add</span><span class="sxs-lookup"><span data-stu-id="2e8c4-101">TableRowCollection: add</span></span>

<span data-ttu-id="2e8c4-102">向表中添加新行。</span><span class="sxs-lookup"><span data-stu-id="2e8c4-102">Adds a new row to the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="2e8c4-103">权限</span><span class="sxs-lookup"><span data-stu-id="2e8c4-103">Permissions</span></span>
<span data-ttu-id="2e8c4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="2e8c4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2e8c4-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="2e8c4-106">Permission type</span></span>      | <span data-ttu-id="2e8c4-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2e8c4-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2e8c4-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2e8c4-108">Delegated (work or school account)</span></span> | <span data-ttu-id="2e8c4-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2e8c4-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2e8c4-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2e8c4-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2e8c4-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="2e8c4-111">Not supported.</span></span>    |
|<span data-ttu-id="2e8c4-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="2e8c4-112">Application</span></span> | <span data-ttu-id="2e8c4-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="2e8c4-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2e8c4-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2e8c4-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/rows/add
POST /workbook/worksheets/{id|name}/tables/{id|name}/rows/add

```
## <a name="request-headers"></a><span data-ttu-id="2e8c4-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="2e8c4-115">Request headers</span></span>
| <span data-ttu-id="2e8c4-116">名称</span><span class="sxs-lookup"><span data-stu-id="2e8c4-116">Name</span></span>       | <span data-ttu-id="2e8c4-117">说明</span><span class="sxs-lookup"><span data-stu-id="2e8c4-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2e8c4-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="2e8c4-118">Authorization</span></span>  | <span data-ttu-id="2e8c4-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2e8c4-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2e8c4-121">请求正文</span><span class="sxs-lookup"><span data-stu-id="2e8c4-121">Request body</span></span>
<span data-ttu-id="2e8c4-122">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="2e8c4-122">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2e8c4-123">参数</span><span class="sxs-lookup"><span data-stu-id="2e8c4-123">Parameter</span></span>    | <span data-ttu-id="2e8c4-124">类型</span><span class="sxs-lookup"><span data-stu-id="2e8c4-124">Type</span></span>   |<span data-ttu-id="2e8c4-125">说明</span><span class="sxs-lookup"><span data-stu-id="2e8c4-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2e8c4-126">index</span><span class="sxs-lookup"><span data-stu-id="2e8c4-126">index</span></span>|<span data-ttu-id="2e8c4-127">number</span><span class="sxs-lookup"><span data-stu-id="2e8c4-127">number</span></span>|<span data-ttu-id="2e8c4-p103">可选。指定新行的相对位置。如果为空，将在末尾进行添加。插入的行下方的任何行将向下移动。从零开始编制索引。</span><span class="sxs-lookup"><span data-stu-id="2e8c4-p103">Optional. Specifies the relative position of the new row. If null, the addition happens at the end. Any rows below the inserted row are shifted downwards. Zero-indexed.</span></span>|
|<span data-ttu-id="2e8c4-133">values</span><span class="sxs-lookup"><span data-stu-id="2e8c4-133">values</span></span>|<span data-ttu-id="2e8c4-134">（布尔值、字符串或数字）</span><span class="sxs-lookup"><span data-stu-id="2e8c4-134">(boolean or string or number)</span></span>|<span data-ttu-id="2e8c4-p104">可选。未设置格式的表行值的二维数组。</span><span class="sxs-lookup"><span data-stu-id="2e8c4-p104">Optional. A 2-dimensional array of unformatted values of the table row.</span></span>|

## <a name="response"></a><span data-ttu-id="2e8c4-137">响应</span><span class="sxs-lookup"><span data-stu-id="2e8c4-137">Response</span></span>

<span data-ttu-id="2e8c4-138">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [TableRow](../resources/tablerow.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2e8c4-138">If successful, this method returns `200 OK` response code and [TableRow](../resources/tablerow.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2e8c4-139">示例</span><span class="sxs-lookup"><span data-stu-id="2e8c4-139">Example</span></span>
<span data-ttu-id="2e8c4-140">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="2e8c4-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="2e8c4-141">请求</span><span class="sxs-lookup"><span data-stu-id="2e8c4-141">Request</span></span>
<span data-ttu-id="2e8c4-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2e8c4-142">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="2e8c4-143">响应</span><span class="sxs-lookup"><span data-stu-id="2e8c4-143">Response</span></span>
<span data-ttu-id="2e8c4-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2e8c4-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
