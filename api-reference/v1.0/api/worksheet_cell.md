# <a name="worksheet-cell"></a><span data-ttu-id="e36f9-101">Worksheet:Cell</span><span class="sxs-lookup"><span data-stu-id="e36f9-101">Worksheet: Cell</span></span>

<span data-ttu-id="e36f9-p101">根据行和列编号获取包含单个单元格的 range 对象。单元格可以位于父区域外部，只要其保持在工作表网格内即可。</span><span class="sxs-lookup"><span data-stu-id="e36f9-p101">Gets the range object containing the single cell based on row and column numbers. The cell can be outside the bounds of its parent range, so long as it's stays within the worksheet grid.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e36f9-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="e36f9-104">Prerequisites</span></span>
<span data-ttu-id="e36f9-105">要执行此 API，需要以下**范围**：</span><span class="sxs-lookup"><span data-stu-id="e36f9-105">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="e36f9-106">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e36f9-106">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="e36f9-107">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e36f9-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/Cell(row=<row>,column=<column>)

```
## <a name="request-headers"></a><span data-ttu-id="e36f9-108">请求标头</span><span class="sxs-lookup"><span data-stu-id="e36f9-108">Request headers</span></span>
| <span data-ttu-id="e36f9-109">名称</span><span class="sxs-lookup"><span data-stu-id="e36f9-109">Name</span></span>       | <span data-ttu-id="e36f9-110">说明</span><span class="sxs-lookup"><span data-stu-id="e36f9-110">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e36f9-111">Authorization</span><span class="sxs-lookup"><span data-stu-id="e36f9-111">Authorization</span></span>  | <span data-ttu-id="e36f9-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e36f9-p102">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="e36f9-114">响应</span><span class="sxs-lookup"><span data-stu-id="e36f9-114">Response</span></span>

<span data-ttu-id="e36f9-115">如果成功，此方法在响应正文中返回 `200, OK` 响应代码和 [Range](../resources/range.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e36f9-115">If successful, this method returns `200, OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e36f9-116">示例</span><span class="sxs-lookup"><span data-stu-id="e36f9-116">Example</span></span>
<span data-ttu-id="e36f9-117">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="e36f9-117">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e36f9-118">请求</span><span class="sxs-lookup"><span data-stu-id="e36f9-118">Request</span></span>
<span data-ttu-id="e36f9-119">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e36f9-119">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheet_cell"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/Cell(row=<row>,column=<column>)
```

##### <a name="response"></a><span data-ttu-id="e36f9-120">响应</span><span class="sxs-lookup"><span data-stu-id="e36f9-120">Response</span></span>
<span data-ttu-id="e36f9-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e36f9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.range"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 1,
  "columnCount": 1,
  "columnIndex": 3,
  "valueTypes": "valueTypes-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Worksheet: Cell",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
